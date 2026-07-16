import { useState, useMemo } from "react";
import {
  Search,
  Mail,
  Phone,
  ChevronLeft,
  ChevronRight,
  X,
  Image as ImageIcon,
} from "lucide-react";

const COLORS = {
  primary: "#37474f",
  secondary: "#263238",
  light: "#f5f5f5",
  dark: "#212121",
  accent: "#546e7a",
  border: "#e0e0e0",
  muted: "#757575",
  body: "#424242",
};

const ARTICLES = [
  {
    id: 1,
    title: "Council Initiates Proposal to Ban Synthetic Turfs Across the City",
    category: "Community and Climate",
    date: "March 5, 2025",
    author: "Editorial Staff",
    summary:
      "The city council further pushed the proposal to ban the installation of synthetic turfs in the city. Parks Department to present evidence on PFAS levels Tuesday.",
    content:
      "The city council further pushed the proposal to ban the installation of synthetic turfs in the city. The Parks Department is set to present evidence on PFAS levels found in existing installations at Tuesday's session. Community groups on both sides of the issue are expected to testify, with sports leagues citing maintenance costs and environmental advocates pointing to runoff concerns near waterways. A final vote is expected by the end of the month.",
  },
  {
    id: 2,
    title: "Music Hall Renovation in Harlem Begins Next Week",
    category: "Community",
    date: "March 4, 2025",
    author: "Editorial Staff",
    summary:
      "The renovation of Harlem Hall will start Monday with the first phase focusing on floor tiling.",
    content:
      "The renovation of Harlem Hall will start Monday with the first phase focusing on floor tiling and structural repairs to the stage. The venue, closed since December, is expected to reopen in early summer with an updated sound system and accessible seating.",
  },
  {
    id: 3,
    title: "Annual Budget Review Focuses on Infrastructure",
    category: "Government",
    date: "March 3, 2025",
    author: "Editorial Staff",
    summary:
      "Council members debated road repair priorities and water system upgrades during yesterday's session.",
    content:
      "Council members debated road repair priorities and water system upgrades during yesterday's session. Roughly a third of the proposed capital budget is earmarked for aging water infrastructure, with the remainder split between road resurfacing and sidewalk accessibility projects.",
  },
  {
    id: 4,
    title: "Local Business Recognized for Community Impact",
    category: "Business",
    date: "March 2, 2025",
    author: "Editorial Staff",
    summary:
      "Greenfield Market received the annual Chamber of Commerce award for their community initiatives.",
    content:
      "Greenfield Market received the annual Chamber of Commerce award for their community initiatives, including a weekly free produce stand for seniors and a paid apprenticeship program for local high schoolers.",
  },
  {
    id: 5,
    title: "New Education Initiative Launches at Local Schools",
    category: "Education",
    date: "March 1, 2025",
    author: "Editorial Staff",
    summary:
      "The program aims to improve science education through hands-on learning and mentorship.",
    content:
      "The program aims to improve science education through hands-on learning and mentorship, pairing students with volunteer engineers from nearby universities for a semester-long project culminating in a district-wide science fair.",
  },
  {
    id: 6,
    title: "Bike Lane Expansion Approved for Riverside Avenue",
    category: "Government",
    date: "February 27, 2025",
    author: "Editorial Staff",
    summary:
      "A protected bike lane will replace one lane of street parking along an eight-block stretch.",
    content:
      "A protected bike lane will replace one lane of street parking along an eight-block stretch of Riverside Avenue. Merchants had raised concerns about lost parking, and the final plan includes a loading-zone compromise at three intersections.",
  },
  {
    id: 7,
    title: "Community Garden Waitlist Reaches Record Length",
    category: "Community",
    date: "February 25, 2025",
    author: "Editorial Staff",
    summary:
      "Demand for plots has tripled since 2022, prompting calls for a second garden site.",
    content:
      "Demand for plots has tripled since 2022, prompting calls for a second garden site on the vacant lot behind the library. The Parks Department says a feasibility study will begin this spring.",
  },
  {
    id: 8,
    title: "Small Business Grants Open for Application",
    category: "Business",
    date: "February 22, 2025",
    author: "Editorial Staff",
    summary:
      "Up to fifty storefronts will receive facade improvement grants this cycle.",
    content:
      "Up to fifty storefronts will receive facade improvement grants this cycle, part of a broader push to revitalize the commercial corridor ahead of next year's transit expansion.",
  },
  {
    id: 9,
    title: "After-School Robotics Program Expands to Three More Schools",
    category: "Education",
    date: "February 20, 2025",
    author: "Editorial Staff",
    summary: "The program will now reach over 600 students citywide.",
    content:
      "The program will now reach over 600 students citywide, funded in part by a partnership with a local manufacturing firm that donates retired equipment for teams to refurbish.",
  },
  {
    id: 10,
    title: "Heat Wave Prompts Extended Cooling Center Hours",
    category: "Community and Climate",
    date: "February 18, 2025",
    author: "Editorial Staff",
    summary: "Five city facilities will stay open until 9 p.m. through the weekend.",
    content:
      "Five city facilities will stay open until 9 p.m. through the weekend as temperatures are expected to climb past seasonal norms. Officials urged residents to check on elderly neighbors.",
  },
  {
    id: 11,
    title: "Council Debates Rezoning Near Transit Hub",
    category: "Government",
    date: "February 15, 2025",
    author: "Editorial Staff",
    summary: "A proposal would allow taller residential buildings within a quarter mile of the station.",
    content:
      "A proposal would allow taller residential buildings within a quarter mile of the station. Supporters cite housing shortages; opponents worry about strain on aging sewer lines.",
  },
  {
    id: 12,
    title: "Farmers Market Season Opens Early This Year",
    category: "Community",
    date: "February 12, 2025",
    author: "Editorial Staff",
    summary: "A mild winter allowed vendors to start three weeks ahead of schedule.",
    content:
      "A mild winter allowed vendors to start three weeks ahead of schedule, with the market adding two new produce stands and a rotating food-truck slot this year.",
  },
];

const COUNCILLORS = [
  { name: "Mayor J. Williams", phone: "555-123-4567", email: "mayor@cityname.gov" },
  { name: "Councillor A. Lee", phone: "555-234-5678", email: "alee@cityname.gov" },
  { name: "Councillor M. Garcia", phone: "555-345-6789", email: "mgarcia@cityname.gov" },
  { name: "Councillor R. Smith", phone: "555-456-7890", email: "rsmith@cityname.gov" },
];

const EXPERTS = [
  {
    name: "Dr. Davis",
    title: "Urban Planning",
    quote:
      "The development plan balances economic growth with community needs, though concerns about adequate affordable housing remain.",
  },
  {
    name: "Ms. Johnson",
    title: "Economic Development",
    quote:
      "Local businesses should see increased foot traffic once the downtown improvements are completed in the coming year.",
  },
  {
    name: "Mr. Patel",
    title: "Environmental Consultant",
    quote:
      "The sustainability elements in the plan are a positive step, though more ambitious green space allocations would benefit the community.",
  },
  {
    name: "Ms. Alvarez",
    title: "Public Health",
    quote:
      "Extended cooling center hours are a good stopgap, but the city needs a long-term heat resilience strategy.",
  },
];

const PAGE_SIZE = 4;

function PlaceholderImage({ label, height = 180 }) {
  return (
    <div
      style={{
        height,
        background: `linear-gradient(135deg, ${COLORS.accent}, ${COLORS.primary})`,
        display: "flex",
        flexDirection: "column",
        alignItems: "center",
        justifyContent: "center",
        color: "white",
        gap: 6,
      }}
    >
      <ImageIcon size={22} strokeWidth={1.5} />
      <span style={{ fontSize: 11, opacity: 0.85, padding: "0 12px", textAlign: "center" }}>
        {label}
      </span>
    </div>
  );
}

function CategoryPill({ label, active, onClick }) {
  return (
    <button
      onClick={onClick}
      style={{
        border: `1px solid ${active ? COLORS.primary : COLORS.border}`,
        background: active ? COLORS.primary : "white",
        color: active ? "white" : COLORS.primary,
        padding: "5px 12px",
        fontSize: 13,
        cursor: "pointer",
        borderRadius: 2,
        whiteSpace: "nowrap",
      }}
    >
      {label}
    </button>
  );
}

export default function YoursTruly() {
  const [searchTerm, setSearchTerm] = useState("");
  const [category, setCategory] = useState("All");
  const [page, setPage] = useState(1);
  const [featuredId, setFeaturedId] = useState(1);
  const [expertIndex, setExpertIndex] = useState(0);

  const categories = useMemo(
    () => ["All", ...Array.from(new Set(ARTICLES.map((a) => a.category)))],
    []
  );

  const featured = ARTICLES.find((a) => a.id === featuredId) || ARTICLES[0];

  const filtered = useMemo(() => {
    return ARTICLES.filter((a) => a.id !== featured.id)
      .filter((a) => (category === "All" ? true : a.category === category))
      .filter((a) => {
        const term = searchTerm.trim().toLowerCase();
        if (!term) return true;
        return (
          a.title.toLowerCase().includes(term) ||
          a.summary.toLowerCase().includes(term) ||
          a.category.toLowerCase().includes(term)
        );
      });
  }, [category, searchTerm, featured.id]);

  const totalPages = Math.max(1, Math.ceil(filtered.length / PAGE_SIZE));
  const safePage = Math.min(page, totalPages);
  const pageItems = filtered.slice((safePage - 1) * PAGE_SIZE, safePage * PAGE_SIZE);

  function updateSearch(v) {
    setSearchTerm(v);
    setPage(1);
  }
  function updateCategory(c) {
    setCategory(c);
    setPage(1);
  }
  function makeFeatured(id) {
    setFeaturedId(id);
    setPage(1);
  }

  return (
    <div
      style={{
        fontFamily: "Arial, sans-serif",
        background: COLORS.light,
        color: COLORS.dark,
        lineHeight: 1.6,
        minHeight: "100%",
      }}
    >
      {/* Header */}
      <header style={{ background: COLORS.primary, color: "white", padding: "16px" }}>
        <div
          style={{
            maxWidth: 1100,
            margin: "0 auto",
            display: "flex",
            justifyContent: "space-between",
            alignItems: "center",
            flexWrap: "wrap",
            gap: 8,
          }}
        >
          <div style={{ fontSize: "1.5rem", letterSpacing: 1 }}>Yours Truly</div>
          <ul style={{ display: "flex", listStyle: "none", gap: 24, margin: 0, padding: 0 }}>
            {["Home", "News", "Council", "Community", "Contact"].map((item) => (
              <li key={item}>
                <a href="#" style={{ color: "white", textDecoration: "none", fontSize: 14 }}>
                  {item}
                </a>
              </li>
            ))}
          </ul>
        </div>
      </header>

      {/* Search */}
      <div style={{ maxWidth: 1100, margin: "16px auto", padding: "0 16px" }}>
        <div style={{ display: "flex" }}>
          <input
            value={searchTerm}
            onChange={(e) => updateSearch(e.target.value)}
            placeholder="Search articles..."
            style={{
              flex: 1,
              padding: "8px 10px",
              border: `1px solid ${COLORS.border}`,
              fontSize: 14,
            }}
          />
          <button
            style={{
              padding: "8px 16px",
              background: COLORS.secondary,
              color: "white",
              border: "none",
              cursor: "pointer",
              display: "flex",
              alignItems: "center",
              gap: 6,
            }}
            onClick={() => updateSearch(searchTerm)}
          >
            <Search size={14} /> Search
          </button>
        </div>

        <div style={{ display: "flex", gap: 8, marginTop: 12, overflowX: "auto", paddingBottom: 4 }}>
          {categories.map((c) => (
            <CategoryPill key={c} label={c} active={category === c} onClick={() => updateCategory(c)} />
          ))}
        </div>
      </div>

      <main
        style={{
          maxWidth: 1100,
          margin: "24px auto",
          padding: "0 16px",
          display: "grid",
          gridTemplateColumns: "2fr 1fr",
          gap: 32,
        }}
        className="ytmain"
      >
        <div>
          <h2 style={sectionTitleStyle}>Today in Communities</h2>
          <div style={{ background: "white", border: `1px solid ${COLORS.border}`, marginBottom: 32 }}>
            <PlaceholderImage label={featured.category} height={260} />
            <div style={{ padding: 16 }}>
              <span
                style={{
                  background: COLORS.accent,
                  color: "white",
                  padding: "3px 8px",
                  fontSize: 12,
                  marginRight: 12,
                }}
              >
                {featured.category}
              </span>
              <h2 style={{ fontSize: "1.4rem", fontWeight: "normal", margin: "10px 0" }}>
                {featured.title}
              </h2>
              <div style={{ color: COLORS.muted, fontSize: 13, marginBottom: 12 }}>
                {featured.date} | By {featured.author}
              </div>
              <p style={{ color: COLORS.body, marginBottom: 12 }}>{featured.content}</p>
            </div>
          </div>

          <h2 style={sectionTitleStyle}>Recent Stories</h2>
          {pageItems.length === 0 ? (
            <p style={{ color: COLORS.muted, marginBottom: 24 }}>No stories match your search.</p>
          ) : (
            <div
              style={{
                display: "grid",
                gridTemplateColumns: "repeat(auto-fill, minmax(230px, 1fr))",
                gap: 20,
                marginBottom: 24,
              }}
            >
              {pageItems.map((a) => (
                <div key={a.id} style={{ background: "white", border: `1px solid ${COLORS.border}` }}>
                  <PlaceholderImage label={a.category} height={130} />
                  <div style={{ padding: 12 }}>
                    <h3 style={{ fontSize: 15, fontWeight: "normal", marginBottom: 6 }}>{a.title}</h3>
                    <div
                      style={{
                        display: "flex",
                        justifyContent: "space-between",
                        color: COLORS.muted,
                        fontSize: 12,
                        marginBottom: 6,
                      }}
                    >
                      <span>{a.category}</span>
                      <span>{a.date}</span>
                    </div>
                    <p style={{ fontSize: 13, color: COLORS.body, marginBottom: 8 }}>{a.summary}</p>
                    <button
                      onClick={() => makeFeatured(a.id)}
                      style={{
                        border: "none",
                        background: "none",
                        color: COLORS.primary,
                        cursor: "pointer",
                        fontSize: 13,
                        padding: 0,
                      }}
                    >
                      Continue reading →
                    </button>
                  </div>
                </div>
              ))}
            </div>
          )}

          {totalPages > 1 && (
            <div style={{ display: "flex", justifyContent: "center", gap: 6 }}>
              <PageBtn disabled={safePage === 1} onClick={() => setPage(safePage - 1)}>
                <ChevronLeft size={14} />
              </PageBtn>
              {Array.from({ length: totalPages }, (_, i) => i + 1).map((n) => (
                <PageBtn key={n} active={n === safePage} onClick={() => setPage(n)}>
                  {n}
                </PageBtn>
              ))}
              <PageBtn disabled={safePage === totalPages} onClick={() => setPage(safePage + 1)}>
                <ChevronRight size={14} />
              </PageBtn>
            </div>
          )}
        </div>

        <div style={{ display: "flex", flexDirection: "column", gap: 32 }}>
          <div style={{ background: "white", border: `1px solid ${COLORS.border}`, padding: 16 }}>
            <h2 style={sectionTitleStyle}>City Council Contact Information</h2>
            {COUNCILLORS.map((c, i) => (
              <div
                key={c.name}
                style={{
                  display: "flex",
                  alignItems: "center",
                  gap: 12,
                  paddingBottom: 12,
                  marginBottom: 12,
                  borderBottom: i < COUNCILLORS.length - 1 ? `1px solid ${COLORS.border}` : "none",
                }}
              >
                <div
                  style={{
                    width: 44,
                    height: 44,
                    borderRadius: "50%",
                    background: COLORS.accent,
                    color: "white",
                    display: "flex",
                    alignItems: "center",
                    justifyContent: "center",
                    fontSize: 14,
                    flexShrink: 0,
                  }}
                >
                  {c.name
                    .split(" ")
                    .slice(-1)[0]
                    .charAt(0)}
                </div>
                <div style={{ fontSize: 13 }}>
                  <div style={{ marginBottom: 4 }}>{c.name}</div>
                  <a
                    href={`tel:${c.phone}`}
                    style={{ color: COLORS.muted, textDecoration: "none", display: "flex", alignItems: "center", gap: 4 }}
                  >
                    <Phone size={11} /> {c.phone}
                  </a>
                  <a
                    href={`mailto:${c.email}`}
                    style={{ color: COLORS.muted, textDecoration: "none", display: "flex", alignItems: "center", gap: 4 }}
                  >
                    <Mail size={11} /> {c.email}
                  </a>
                </div>
              </div>
            ))}
          </div>

          <div style={{ background: "white", border: `1px solid ${COLORS.border}`, padding: 16 }}>
            <h2 style={sectionTitleStyle}>Expert Analysis</h2>
            <div style={{ marginBottom: 12 }}>
              <div style={{ fontSize: 14, marginBottom: 2 }}>{EXPERTS[expertIndex].name}</div>
              <div style={{ fontSize: 12, color: COLORS.muted, marginBottom: 8 }}>
                {EXPERTS[expertIndex].title}
              </div>
              <p style={{ fontStyle: "italic", fontSize: 13.5, color: COLORS.body }}>
                "{EXPERTS[expertIndex].quote}"
              </p>
            </div>
            <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center" }}>
              <button
                onClick={() => setExpertIndex((expertIndex - 1 + EXPERTS.length) % EXPERTS.length)}
                style={iconBtnStyle}
              >
                <ChevronLeft size={16} />
              </button>
              <div style={{ display: "flex", gap: 6 }}>
                {EXPERTS.map((_, i) => (
                  <div
                    key={i}
                    onClick={() => setExpertIndex(i)}
                    style={{
                      width: 6,
                      height: 6,
                      borderRadius: "50%",
                      background: i === expertIndex ? COLORS.primary : COLORS.border,
                      cursor: "pointer",
                    }}
                  />
                ))}
              </div>
              <button
                onClick={() => setExpertIndex((expertIndex + 1) % EXPERTS.length)}
                style={iconBtnStyle}
              >
                <ChevronRight size={16} />
              </button>
            </div>
          </div>
        </div>
      </main>

      <footer style={{ background: COLORS.secondary, color: "white", padding: "32px 16px" }}>
        <div
          style={{
            maxWidth: 1100,
            margin: "0 auto",
            display: "grid",
            gridTemplateColumns: "repeat(auto-fit, minmax(230px, 1fr))",
            gap: 32,
          }}
        >
          <div>
            <h3 style={{ fontWeight: "normal", marginBottom: 12 }}>About</h3>
            <p style={{ fontSize: 13.5, color: "#bdbdbd" }}>
              Yours Truly provides accurate, timely information about local government, community
              events, expert analysis, by the communities themselves, along with access to your
              councillors.
            </p>
          </div>
          <div>
            <h3 style={{ fontWeight: "normal", marginBottom: 12 }}>Navigation</h3>
            <ul style={{ listStyle: "none", padding: 0, margin: 0 }}>
              {["Home", "News Archive", "Council Information", "Community Calendar", "Contact"].map(
                (l) => (
                  <li key={l} style={{ marginBottom: 8 }}>
                    <a href="#" style={{ color: "#bdbdbd", textDecoration: "none", fontSize: 13.5 }}>
                      {l}
                    </a>
                  </li>
                )
              )}
            </ul>
          </div>
          <div>
            <h3 style={{ fontWeight: "normal", marginBottom: 12 }}>Contact</h3>
            <p style={{ fontSize: 13.5, color: "#bdbdbd" }}>
              116 Amsterdam Avenue
              <br />
              NY, 10027
              <br />
              info@yourstruly.com
              <br />
              (555) 987-6543
            </p>
          </div>
        </div>
        <div
          style={{
            textAlign: "center",
            paddingTop: 20,
            marginTop: 20,
            borderTop: "1px solid #455a64",
            color: "#9e9e9e",
            fontSize: 12,
          }}
        >
          © 2025 Yours Truly. All rights reserved.
        </div>
      </footer>

      <style>{`
        @media (max-width: 768px) {
          .ytmain { grid-template-columns: 1fr !important; }
        }
      `}</style>
    </div>
  );
}

const sectionTitleStyle = {
  fontSize: "1.15rem",
  fontWeight: "normal",
  marginBottom: 16,
  borderBottom: `1px solid ${COLORS.border}`,
  paddingBottom: 8,
};

const iconBtnStyle = {
  border: `1px solid ${COLORS.border}`,
  background: "white",
  cursor: "pointer",
  padding: 4,
  display: "flex",
  color: COLORS.primary,
};

function PageBtn({ children, active, disabled, onClick }) {
  return (
    <button
      disabled={disabled}
      onClick={onClick}
      style={{
        padding: "6px 12px",
        border: `1px solid ${COLORS.border}`,
        background: active ? COLORS.primary : "white",
        color: active ? "white" : disabled ? "#bbb" : COLORS.primary,
        cursor: disabled ? "default" : "pointer",
      }}
    >
      {children}
    </button>
  );
}
