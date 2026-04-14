# 20 — Page Templates

> Full-page assembly instructions. Each template is a specific combination of the components above, assembled within the layout shell.

---

## Template 1: AI Analytics Chat Agent

This is the core template. The primary interface for Nexus agents.

### Assembly

1. Start with the **Layout Shell** (spec 02)
2. Place the **Sidebar** (spec 03) on the left
3. In the main area, stack vertically:
   - **Top Navigation** (spec 04) — title "AI Analytics Assistant"
   - **Breadcrumb** (spec 13) — "← Back to Component Showcase" (optional)
   - **Chat Area** (scrollable) containing:
     - **AI Message** (spec 05) — welcome greeting
     - **User Message** (spec 05) — user query
     - **AI Message** (spec 05) — analytical response
     - **Analytics Section** (spec 07) — "Generated Analytics" label + 2 chart cards
     - **Tool Calls Section** (spec 08) — 3 tool call cards (success, processing, error)
   - **Chat Input** (spec 06) — pinned to bottom

### Variants

- **Light mode:** use all light tokens from spec 01 and spec 19
- **Dark mode:** swap all values using spec 19 mapping
- **With breadcrumb:** adds 42px bar between topnav and chat area
- **Without breadcrumb:** chat area starts immediately below topnav
- **Extended (Social Media + R&D):** after the analytics section, add social media metric cards (spec 09 pattern) and product milestone timeline cards

---

## Template 2: Component Showcase

A documentation/demo page that displays all available components in numbered sections.

### Assembly

1. **Layout Shell** — same sidebar + topnav structure
2. Topnav includes a "← Back to Home" link and a "Component Showcase" title, plus a "Dark Mode" toggle button on the right
3. Content area is a single scrollable column with numbered sections:
   - **1. Chat Cards** — 2×2 grid of agent category cards (icon + title + subtitle). Variants: white bg, blue bg, dark bg, purple bg
   - **2. Chat Conversation** — sample user/AI exchange (spec 05)
   - **3. Left Sidebar** — isolated sidebar preview (spec 03)
   - **4. Top Navigation Bar** — isolated topnav preview (spec 04)
   - **5. Chat Input** — isolated input preview (spec 06)
   - **6. Graphs and Charts** — 2×2 grid of chart cards (spec 07) plus additional bar and pie chart examples
   - **7. Action Cards with Images** — 3-column grid of image cards (spec 17)
   - **8. Tool Call UI** — 3 tool call cards (spec 08)
   - **9. Toast Notifications** — 2×3 grid of toast variants (spec 15)

---

## Template 3: Landing / Marketing Page

A hero + feature grid page for marketing the AI Chat UI library.

### Assembly (no sidebar)

1. **Hero section:** gradient background (blue-50 to white), centered content
   - Badge pill: "✦ AI Chat UI Component Library"
   - Heading: "Build Beautiful AI Chat Interfaces" — display-lg size
   - Subtitle: description text — text-lg, color gray-500
   - Two buttons: primary dark ("View Components") + secondary outlined ("Live Demo")
2. **Feature grid:** 4-column grid of icon cards
   - Each card: icon in colored square (40px) + title (14px semibold) + description (12px gray)
   - Categories: Chat Components, Navigation, Data Visualization, Tool Integrations
3. **Theme preview:** bordered card with 5 color swatches showing the semantic palette
4. **CTA footer:** "Ready to Build?" heading + two buttons

---

## Template 4: Product Information / INCI Agent

A structured data display for product ingredient information.

### Assembly

1. **Layout Shell** — same sidebar + topnav structure
2. Content area contains one or more **INCI Cards** (spec 18)
3. Cards are full-width within the content area, with 24px padding around them
4. Multiple cards (e.g. English and French variants) stack vertically with 16px gap

---

## Template 5: Marketing Chat (Ideas)

A WIP template for a marketing-focused AI chat agent. Uses the same layout shell and component library as Template 1 but with marketing-specific content and potentially different agent personalities/prompts.

### Assembly

- Same as Template 1 but with marketing-oriented sample data
- Chat cards may show marketing-specific categories (Campaign Planner, Content Writer, etc.)
- Charts would show marketing metrics (impressions, CTR, conversion rates)
