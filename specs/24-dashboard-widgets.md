# 24 — Dashboard Widgets

> Complex composite components from the Figma Dashboard Widgets page. These are larger panel-level elements used in Nexus agent dashboards.

---

## Full-Width Search Input

A search bar that spans the full width of the content area, used at the top of dashboard views.

- **Height:** 44px
- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-200
- **Border radius:** 8px
- **Padding:** 10px 16px
- **Icon:** Search, 18px, color gray-400, left side
- **Input:** 14px, weight 400, gray-900, placeholder "Search..." in gray-400
- **Right side (optional):** "Submit" button — primary small

---

## Agent Dashboard Header

A horizontal bar identifying the current agent context with navigation.

- **Height:** 52px
- **Background:** white
- **Border bottom:** 1px solid gray-200
- **Padding:** 0 24px
- **Display:** flex row, align-items center, justify-content space-between

### Left Side

- **Breadcrumb dots:** flex row of colored dots (6px, rounded full) in brand-600, success-500, warning-500 — shows agent hierarchy
- **Agent name:** 14px, weight 600, gray-900

### Right Side

- **Action buttons:** secondary gray buttons ("⚡ Actions", "📊 Metrics")
- **Status indicator:** badge pill (Active/Inactive)

---

## Notification Banner

A full-width colored banner for system-level notifications or alerts.

- **Width:** 100% of content area
- **Padding:** 12px 20px
- **Border radius:** 8px
- **Display:** flex row, align-items center, gap 10px
- **Icon:** 16px, left side
- **Text:** 14px, weight 500
- **Dismiss button:** X icon, 14px, right side

### Color Variants

| Type | Background | Icon/Text Color | Border |
|---|---|---|---|
| Info | brand-50 (#F9F5FF) | brand-700 (#6941C6) | 1px brand-200 |
| Success | success-50 (#ECFDF3) | success-700 (#027A48) | 1px success-200 |
| Warning | warning-50 (#FFFAEB) | warning-700 (#B54708) | 1px warning-200 |
| Error | error-50 (#FEF3F2) | error-700 (#B42318) | 1px error-200 |
| Dark/CRT Agent | navy #001529 | white text | none |

---

## Agent Conversation Card (Expandable)

A card representing one conversation in a list/grid of agent conversations. Shows summary with expand-to-detail.

### Collapsed State

- **Container:** white bg, border gray-200, radius 12px, padding 16px 20px
- **Display:** flex row, justify-content space-between
- **Left side:**
  - User avatar (24px, rounded full, brand bg)
  - User name: 14px, weight 500, gray-900
  - Preview text: 13px, gray-500, truncated 1 line
- **Right side:**
  - Timestamp: 12px, gray-400
  - Status badge: pill (spec 11)

### Expanded State

- Reveals full conversation thread below
- Padding: 16px 20px
- Border-top: 1px gray-100
- Shows message list using spec 05 pattern at reduced scale

---

## LLM Evaluation Results Panel

A wide panel for displaying evaluation/benchmark results from Nexus agent testing.

- **Container:** white bg, border gray-200, radius 12px
- **Header:** "LLM Evaluation Results" — 16px, weight 600, gray-900
- **Tabs below header:** underline tabs (spec 13) — "Overview", "Details", "Comparison"
- **Body:** scrollable data table or chart content
- **Footer:** pagination or "Load More" link

---

## Red Team Testing Panel

A management interface for red team tests against agents.

### Header

- **Title:** "Red Team Testing" — 16px, weight 600, gray-900
- **Right:** "Create Test" button (primary or destructive)

### Test List

- **Layout:** vertical list of test cards
- **Each card:** border gray-200, radius 8px, padding 12px 16px
  - **Test name:** 14px, weight 500, gray-900
  - **Status:** badge pill
  - **Metrics row:** small stat values inline (e.g. "Score: 85%", "Turns: 12")
  - **Timestamp:** 12px, gray-400

### Empty State

- Same as Red Team Test Card empty state (spec 21)

---

## CRT Agent Panel (dark variant)

A dark-themed agent panel visible in the Dashboard Widgets page.

- **Background:** #001529 (navy/dark)
- **Text:** white / rgba(255,255,255, 0.85)
- **Title:** "CRT Agent" — 16px, weight 600, white
- **Content:** follows same layout patterns but with dark mode token swaps (spec 19)
- **Chat interface:** embedded chat component at smaller scale
- **Agent avatar:** brand gradient circle
