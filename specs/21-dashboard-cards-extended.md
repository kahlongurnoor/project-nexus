# 21 — Dashboard Cards (Extended)

> Additional card types visible on the Figma Cards page that are used in Nexus agent dashboards. These extend the basic stat card pattern with richer content.

---

## Red Team Test Card

An empty-state card with CTA, used to initiate red team testing.

### Empty State

- **Container:** same as base card (white bg, 1px border gray-200, radius 12px, padding 24px)
- **Header row:** title "Red Team Tests" (14px, weight 600, gray-900) + count badge right-aligned ("0 Tests", 12px, gray-500)
- **Center content:** vertically centered in card
  - **Icon:** circle with clock/target icon, 48×48px, bg gray-100, icon color gray-400
  - **Title:** "No tests yet" — 14px, weight 600, gray-900, margin-top 12px
  - **Description:** "Create your first red team test" — 12px, gray-500, margin-top 4px
  - **CTA button:** destructive/error style — bg error-500, text white, "Create Test" label, 12px weight 600, padding 8px 16px, radius 8px, margin-top 12px

### With Tests

- Same header, but list of test rows below
- Each row: test name (14px, gray-700) + status badge + timestamp

## System Variations Table

A two-column data table showing orchestrator/system information.

- **Container:** white bg, border gray-200, radius 12px, no padding (table fills the card)
- **Header row:** bg gray-50, padding 12px 20px, border-bottom 1px gray-200
  - Title: "System Variations" (14px, weight 600, gray-900)
  - Right label: "Important Info" (12px, gray-500)
- **Table rows:** alternating, padding 10px 20px
  - **Left column:** text 14px, gray-700 (e.g. "Orchestrator-for")
  - **Right column:** text 14px, gray-500, monospace font (e.g. "12:18-DEV")
  - **Row divider:** 1px solid gray-100

## Available Agents Table

A list of agents with status pills.

- **Container:** white bg, border gray-200, radius 12px
- **Header row:** padding 16px 24px, border-bottom 1px gray-200
  - Title: "Available Agents" (14px, weight 600, gray-900)
  - Right label: "Past 20 Seconds" (12px, gray-500)
- **Agent rows:** padding 12px 24px, border-bottom 1px gray-100
  - **Left:** agent name (14px, gray-700)
  - **Right:** status badge (see spec 11)
    - Active: success pill with "Active" label
    - Error: error pill with colored background
    - Learning: brand pill

## Feedback Stats Row

A horizontal row of 5 stat cards, each with an icon and metric.

- **Layout:** grid, 5 columns equal width, gap 12px
- **Each card:** white bg, border gray-200, radius 12px, padding 16px 20px

### Card Anatomy

- **Header row:** flex between
  - Label: 12px, gray-500, weight 500 (e.g. "Total Feedback", "Positive", "Negative")
  - Icon: 16×16px, color varies — chat icon for total, thumbs-up for positive (green), thumbs-down for negative (red), star for rating, trend for satisfaction
- **Value:** 24px, weight 600, gray-900, margin-top 4px (e.g. "24", "13", "11", "44", "88%")

## Agent Turn Card

An expandable card showing one turn/step in an agent's execution.

- **Container:** white bg, border gray-200, radius 8px, padding 12px 16px
- **Display:** flex row, align-items center, gap 12px
- **Left icon:** expand/collapse chevron (▶ collapsed, ▼ expanded), 14px, gray-400
- **Turn label:** "Turn 1" — 14px, weight 600, gray-900
- **Function name:** monospace font, 12px, gray-500 (e.g. "FINAL_REPORT_GENERATED")
- **Event count:** "12 events" — 12px, gray-400
- **Right:** expand button — brand pill style, "Expand" label + arrow icon
- **Expanded state:** reveals child event list below with indented rows

## Info Tile Card

A content card with icon, title, body, and optional tag.

- **Container:** white bg, border gray-200, radius 12px, padding 20px
- **Icon:** 24×24px circle, bg brand-50, icon color brand-600, positioned top
- **Title:** 16px, weight 600, gray-900, margin-top 12px
- **Body text:** 14px, weight 400, gray-500, margin-top 4px, line-height 1.5
- **Tag (optional):** pill badge at bottom, margin-top 12px — "Button ✕" with dismiss X

## Timer/Counter Card

A small card with a circular icon and large counter value.

- **Container:** white bg, border gray-200, radius 12px, padding 16px, width ~80px
- **Icon:** 24×24px, centered, clock/timer icon, color brand-600
- **Value:** 24px, weight 600, gray-900, centered, margin-top 8px (e.g. "100")
- **Label:** 12px, gray-500, centered (e.g. "Body text")
