# Project Habibi — UI Specification Templates

> **Purpose:** Machine-readable and human-readable specification documents for building AI agent interfaces on Nexus. These files define every visual and structural decision — fonts, colors, spacing, layout rules, component anatomy, and behavior — so that a coding agent or developer can build any screen without needing access to Figma.

## How to Use These Specs

**For AI coding agents:** Read the relevant spec file before generating code. Each file is self-contained — it tells you exactly what font to use, what hex color to apply, how many pixels of padding, and what the layout structure is. Follow the specs literally.

**For developers:** Use these as your source of truth when the Figma file isn't available. Every value is extracted directly from the Figma Design System 2.0.

**For new agent builders on Nexus:** Start with `01-design-tokens.md` to understand the foundational variables, then read the template spec for the interface you're building.

---

## Spec Files

| # | File | What It Covers |
|---|---|---|
| 01 | [Design Tokens](specs/01-design-tokens.md) | Colors, typography, spacing, shadows, radii — all foundational variables |
| 02 | [Layout Shell](specs/02-layout-shell.md) | The app-level container: sidebar + topnav + content area structure |
| 03 | [Sidebar](specs/03-sidebar.md) | Left navigation panel: new chat button, chat history list, footer actions |
| 04 | [Top Navigation Bar](specs/04-top-navigation.md) | Header bar: title, search, notifications, user profile |
| 05 | [Chat Messages](specs/05-chat-messages.md) | AI and user message bubbles, avatars, timestamps, feedback actions |
| 06 | [Chat Input](specs/06-chat-input.md) | Bottom input bar: textarea, attachment, mic, send button |
| 07 | [Analytics Cards](specs/07-analytics-cards.md) | Inline chart cards: stat value + trend badge + chart area |
| 08 | [Tool Call Cards](specs/08-tool-call-cards.md) | Status indicators for agent tool execution: success, processing, error |
| 09 | [Stat Cards](specs/09-stat-cards.md) | Metric display cards used in dashboard rows |
| 10 | [Buttons](specs/10-buttons.md) | All button variants, sizes, states, and sub-types |
| 11 | [Badges & Pills](specs/11-badges-pills.md) | Status indicators, version tags, filter pills |
| 12 | [Form Inputs](specs/12-form-inputs.md) | Text inputs, textareas, email subscribe, dropdowns |
| 13 | [Tabs & Navigation](specs/13-tabs-navigation.md) | Underline tabs, pill tabs, breadcrumbs |
| 14 | [Modals & Dialogs](specs/14-modals-dialogs.md) | Modal overlays: confirmation, destructive, info, form |
| 15 | [Toast Notifications](specs/15-toast-notifications.md) | Transient alert banners: success, error, warning, info, custom, loading |
| 16 | [Cards — Proposed Plan](specs/16-cards-proposed-plan.md) | Agent plan card with numbered list + approve/reject CTAs |
| 17 | [Cards — Action with Image](specs/17-cards-action-image.md) | Image-header cards with action buttons |
| 18 | [Cards — INCI / Product Info](specs/18-cards-inci.md) | Ingredient and safety statement cards |
| 19 | [Dark Mode Rules](specs/19-dark-mode.md) | How every token maps from light to dark theme |
| 20 | [Page Templates](specs/20-page-templates.md) | Full-page assembly instructions for each agent type |
| 21 | [Dashboard Cards (Extended)](specs/21-dashboard-cards-extended.md) | Red Team card, System Variations table, Available Agents table, Feedback stats, Agent Turn card, Info Tile, Timer card |
| 22 | [Modals (Extended)](specs/22-modals-extended.md) | Date Picker, Data Table modal, Form modal, Feedback Details modal, Filter/Sort modal |
| 23 | [Form Controls (Extended)](specs/23-form-controls-extended.md) | Checkbox, Radio, Scrollbar, Accordion, Menu Bar, Segmented Control, Width Input |
| 24 | [Dashboard Widgets](specs/24-dashboard-widgets.md) | Full-width search, Agent header, Notification banners, Expandable conversation card, LLM eval panel, Red Team panel |

---

## Design System Source

| Detail | Value |
|---|---|
| **Figma File** | [Design System 2.0](https://www.figma.com/design/qafioCr7GiesyZtf90byDh/Design-System-2.0?node-id=339-11336) |
| **Page** | Project Habibi Components |
| **Font (UI)** | Inter (400, 500, 600, 700) |
| **Font (Brand)** | Unilever Desire |
| **Font (Code)** | Consolas / JetBrains Mono |
| **Base Unit** | 16px = 1rem |
| **Framework Target** | React + Tailwind CSS (but specs are framework-agnostic) |
