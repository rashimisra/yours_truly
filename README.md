# Yours Truly

A hyperlocal community news site, rebuilt from a static HTML/CSS mockup into an interactive React app.

**Live site:** https://rashimisra.github.io/yours_truly/

## What this is

Yours Truly started as a static HTML page — a mockup of a local news and civic engagement site with a featured story, a news grid, council contact info, and expert commentary. The goal was to turn it into something people could actually use: search, filter by category, page through stories, and read full articles without a page reload.


## Features built

- **Live search** across article titles, summaries, and categories
- **Category filter pills**, generated dynamically from the actual data set rather than hardcoded
- **Click-to-feature**: clicking "Continue reading" on any card promotes that story into the featured slot with full body copy, and returns the previous featured story to the grid
- **Pagination** that recalculates against whatever's currently filtered, not the full data set
- **Expert Analysis carousel** with prev/next arrows and dot indicators, replacing the original static stack of three quotes
- Working `tel:` and `mailto:` links for council contacts

## Issues faced and how I fixed them

### 1. GitHub Pages served the raw source code instead of the built app
The very first deploy attempt showed literal JSX source text in the browser instead of a rendered page. The cause: GitHub Pages only serves static files as-is — it doesn't compile JSX. A `.jsx` file needs to go through a bundler (Vite) first to become plain JS the browser can execute. The fix was setting up a proper Vite project (`package.json`, `vite.config.js`, `index.html`, `src/main.jsx`, `src/App.jsx`) so there was an actual build step producing a `dist/` folder, instead of pushing raw source straight to Pages.

### 2. Missing/mis-cased entry file
`main.jsx` imports `App` from `./App.jsx`. At one point that file didn't exist in the repo (it had been created at the repo root instead of inside `src/`, and with the wrong case — `app.jsx` instead of `App.jsx`). Since builds run on a case-sensitive filesystem, that mismatch alone broke the import. Fixed by recreating `App.jsx` in the correct location with the correct capitalization.

### 3. Node/npm not installed
Deploying locally requires Node.js, which wasn't installed at all (`command not found: npm`). Installed the LTS build from nodejs.org, then had to fully quit and reopen Terminal for the new PATH to take effect.

### 4. Git authentication failures
Several stacked issues here:
- A typo in the saved remote URL (`rashimishhra` instead of `rashimisra`) meant every push was targeting a nonexistent repo path, caught by checking `git remote -v` and fixing it with `git remote set-url`
- GitHub no longer accepts account passwords for git operations over HTTPS — pushing requires a **Personal Access Token** instead, generated from Settings → Developer settings → Tokens with `repo` scope
- A leftover local `gh-pages` branch from a failed run blocked a fresh deploy attempt (`git branch -D gh-pages` cleared it)

### 5. Local deploy kept hitting a 403
Even after fixing the remote URL, `npm run deploy` (via the `gh-pages` npm package) returned a 403 from GitHub. Rather than keep debugging local token/credential state, I switched to a **GitHub Actions** workflow instead — it builds and deploys entirely on GitHub's servers on every push to `main`, with no local token or `git push` step required at all. This turned out to be the more reliable long-term setup: any future edit made directly on github.com or pushed from any machine deploys automatically.

```yaml
# .github/workflows/deploy.yml
on:
  push:
    branches: [main]
jobs:
  build:
    steps:
      - run: npm install
      - run: npm run build
      - uses: actions/upload-pages-artifact@v3
        with:
          path: ./dist
  deploy:
    needs: build
    steps:
      - uses: actions/deploy-pages@v4
```

Once the Pages **Source** setting was switched from "Deploy from a branch" to **"GitHub Actions,"** every push to `main` triggers an automatic build and deploy.

## Stack

- React (useState, useMemo)
- Vite (build tooling)
- lucide-react (icons)
- GitHub Actions + GitHub Pages (hosting and CI/CD)

## Possible next steps

- Real article data instead of the hardcoded `ARTICLES` array — likely a small Flask or similar API backend
- A D3 chart in the sidebar (e.g. stories per category)
- Mobile layout refinements
