# Template: Component Showcase

> A documentation/demo page showing all available chat components in numbered sections. Uses the same layout shell as the AI Chat Agent. Read `00-design-tokens.md` first.

---

## Page Layout

Same as AI Chat Agent: sidebar (224px) + main area. The main area has a topnav, then a single scrollable content area with numbered sections (no chat input bar at the bottom).

### Topnav Additions
- Left: "← Back to Home" link (12px blue-600) + "⚙ Component Showcase" title (14px weight 600 gray-900)
- Right: "Dark Mode" toggle button — bg gray-900, text white, radius 8px, padding 8px 16px, 12px weight 500

---

## Section 1: Chat Cards

A 2×2 grid of agent category cards. Gap 12px.

### Card Structure
- Flex row, gap 12px, padding 16px, radius 12px.
- **Icon container:** 40px square, radius 8px, flex center.
- **Title:** 14px weight 600.
- **Subtitle:** 12px, lighter color.

### Variants

| Card | Background | Icon Bg | Title Color | Subtitle Color |
|---|---|---|---|---|
| General Assistant | white, border gray-200 | gray-100 | gray-900 | gray-500 |
| Creative Writing | blue-500 | white/20% opacity | white | white/70% |
| Code Helper | gray-900 | white/10% | white | white/60% |
| Personal Tutor | brand-50 | brand-100 | brand-700 | gray-500 |

---

## Section 2: Chat Conversation

A sample 3-message exchange: User → AI → User. Same spec as chat messages in the AI Chat Agent template. Displayed in a bordered container (1px gray-200, radius 12px).

---

## Section 3: Left Sidebar

An isolated preview of the sidebar component. Same spec as AI Chat Agent sidebar, rendered inside a bordered container.

---

## Section 4: Top Navigation Bar

An isolated preview of the topnav. Same spec, inside a bordered container.

---

## Section 5: Chat Input

An isolated preview of the chat input bar. Same spec, inside a bordered container.

---

## Section 6: Graphs and Charts

A 2×2 grid of chart cards. Same chart card spec as AI Chat Agent analytics cards, but with 4 cards:

| Card | Chart Type | Metric | Value | Trend |
|---|---|---|---|---|
| Conversation Volume | Line chart | Volume | 2,543 | ↗ 12.5% |
| Response Time | Area chart | Time | 1.2s | ↘ 8.3% (red) |
| Monthly Usage | Bar chart | Count | 45,678 | ↗ 23.1% |
| Category Distribution | Pie/donut chart | % | — | — |

### Bar Chart Specifics
- Vertical bars, 6 bars (Jan–Jun), bar width proportional, gap 8px between.
- Bar color: gray-900 (light) / blue-500 (dark).
- Same axis label styling as line charts.

### Pie Chart Specifics
- 4 segments. Colors: brand-700, blue-500, success-500, brand-400.
- No labels on chart, legend optional.

---

## Section 7: Action Cards with Images

A 3-column grid, gap 16px.

### Card Structure
- Bg white, border 1px gray-200, radius 12px, overflow hidden.
- **Image area:** top, 70px tall, full width, object-fit cover. Bg placeholder colors: blue-100, gray-800, warning-100.
- **Title:** 12px weight 600 gray-900, padding 12px 16px.
- **Action row:** padding 0 16px 12px, flex row gap 12px. Links: 10px weight 500, icon 10px + label. "👁 View" (blue-600), "✏ Edit" (gray-500), "⬇ Download" (blue-600), "⬆ Share" (gray-500).

Cards: "Project Overview", "Analytics Dashboard", "Team Collaboration"

---

## Section 8: Tool Call UI

3 tool call cards. Same spec as AI Chat Agent tool calls (success, processing, error).

---

## Section 9: Toast Notifications

A 2×3 grid of toast blocks, gap 12px.

| Toast | Background | Text |
|---|---|---|
| Success Toast | #12B76A | white |
| Error Toast | #F04438 | white |
| Warning Toast | #F79009 | white |
| Info Toast | #2E90FA | white |
| Custom Toast | #6941C6 | white |
| Loading Toast | gray-200 | gray-700 |

Each: min-width 140px, padding 12px 16px, radius 8px, 12px weight 600, text centered.

---

## Section Numbering Style

Each section has a label above it: "1. Chat Cards", "2. Chat Conversation", etc.
- Font: 16px weight 600 gray-900.
- Margin-bottom 16px.
- Margin-top 32px (between sections).
