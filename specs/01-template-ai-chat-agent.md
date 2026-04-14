# Template: AI Analytics Chat Agent

> The core Nexus agent interface. Read `00-design-tokens.md` first for all color/font/spacing values. This file contains every component needed to build the full chat screen.

---

## Page Layout

Horizontal flex container, 100vh. Two children: sidebar (fixed 224px) + main (flex:1).

```
┌──────────┬──────────────────────────────────┐
│ SIDEBAR  │  MAIN                            │
│ 224px    │  ┌────────────────────────────┐   │
│ fixed    │  │ TOP NAV (56px)             │   │
│          │  ├────────────────────────────┤   │
│          │  │ BREADCRUMB (42px, optional) │  │
│          │  ├────────────────────────────┤   │
│          │  │ CHAT AREA (flex:1, scrolls) │  │
│          │  ├────────────────────────────┤   │
│          │  │ CHAT INPUT (fixed bottom)  │   │
│          │  └────────────────────────────┘   │
└──────────┴──────────────────────────────────┘
```

---

## Sidebar

- **Width:** 224px, bg #001529, border-right 1px rgba(255,255,255,0.1)
- **Font:** Inter throughout

### New Chat Button
- Padding 14px container. Button: 100% width, 36px tall, bg #1677FF (Ant) or brand-700 (Habibi), radius 8px, shadow-sm. Label: 12px weight 600 white. Plus icon 14px white, gap 7px. Hover: lighten bg, increase shadow.

### Chat History List
- Flex:1, overflow-y auto, padding 0 8px
- **Section label:** "Recent Chats" — 10px weight 500, rgba(255,255,255,0.51), padding 8px 12px
- **Each item:** flex row, gap 10px, padding 10px 12px, radius 8px. Hover: bg rgba(255,255,255,0.06). MessageSquare icon 14px rgba(255,255,255,0.51). Title: 12px weight 500 rgba(255,255,255,0.85), ellipsis overflow. Time: 10px rgba(255,255,255,0.51).

### Footer
- Border-top 1px rgba(255,255,255,0.1), padding 12px 10px, flex column gap 4px
- **Buttons:** flex row, gap 10px, padding 8px 12px, radius 8px, bg transparent, hover rgba(255,255,255,0.06). Icon 14px + label 12px weight 500 rgba(255,255,255,0.85).
- Items: "Dark Mode" (moon icon) + "Settings" (gear icon)

---

## Top Navigation Bar

- Height 56px, bg white, border-bottom 1px gray-200, shadow-xs, padding 0 20px, flex between

### Left: title + search
- **Title:** 16px weight 700 gray-900
- **Search:** 224px wide, 34px tall, bg white, border 1px gray-300, radius 8px, padding 7px 14px. Search icon 14px gray-400 left. Input: 12px gray-700, placeholder gray-400.

### Right: icons + user
- **Help button:** 36px square, radius 8px, transparent, hover gray-100. HelpCircle icon 18px gray-500.
- **Bell button:** same. Bell icon. Red dot: 7px circle bg error-500, top-right 7px/8px.
- **Divider:** 1px × 20px, gray-200, margin 0 8px.
- **User button:** flex row gap 10px, padding 6px 10px, radius 8px, hover gray-50. Avatar: 28px circle bg blue-600, User icon 14px white. Name: 12px weight 500 gray-900. ChevronDown: 14px gray-400.

---

## Breadcrumb Bar (optional)

- Height 42px, bg rgba(255,255,255,0.5), border-bottom 1px gray-200, padding 0 24px
- ArrowLeft icon 14px + "Back to Component Showcase" 12px weight 400 blue-600. Gap 6px. Hover: underline.

---

## Chat Messages

Each message: flex row, gap 14px, padding 24px horizontal 24px top 6px bottom.

### AI Message
- **Background:** gray-50 (light) / #18181E (dark)
- **Avatar:** 34px, radius 8px, border 2px gray-300, bg white. Bot icon 18px gray-700.
- **Name:** 12px weight 600 gray-900. **Time:** 10px gray-400. Gap 8px.
- **Text:** 14px weight 400 gray-900, line-height 1.75.
- **Actions row:** margin-top 10px, flex row gap 2px. Each button 28px square, radius 8px, transparent, hover gray-200. Icons 14px gray-400. Buttons: Copy, ThumbsUp, ThumbsDown.

### User Message
- **Background:** white (light) / #111116 (dark)
- **Avatar:** 34px, radius 8px, bg blue-600 (Ant) or brand-700 (Habibi), no border. User icon 18px white.
- Same header/text spec as AI, no actions row.

---

## Generated Analytics Section

Appears in chat area after AI response.

### Section Label
- Left margin 48px (past avatar). Flex row gap 8px. Sparkles icon 18px blue-600 (light) / brand-400 (dark). Text: 16px weight 500 same color. Margin-bottom 16px.

### Chart Grid
- 2-column grid, gap 14px, left margin 48px.

### Chart Card
- Bg white, border 1px gray-300, radius 8px, padding 20px, shadow-sm.
- **Header:** flex between. Left: label (12px weight 500 gray-400) + value (26px weight 600 gray-900, letter-spacing -0.5px, margin-top 6px). Right: trend badge — pill (radius full), padding 2px 10px, bg rgba(82,196,26,0.1), text 12px weight 500 #52c41a, TrendingUp icon 14px.
- **Chart:** 160px height. Line chart (left card): stroke #1677FF (light) / #9E77ED (dark), 2.5px width, dot circles 4px. Area chart (right card): same stroke + fill rgba(22,119,255,0.08). Grid lines #f0f0f0 (light) / rgba(255,255,255,0.04) (dark). Axis labels 11px gray-400.
- **X-axis:** Mon–Sun. **Y-axis:** 0, 250, 500, 750, 1000.

---

## Tool Call Cards

Below analytics. Left margin 48px.

### Section Label
- Terminal icon 14px gray-700 + "Tool Calls" 12px weight 600 gray-900. Gap 8px, margin-bottom 14px.

### Card Structure (shared)
- Flex row, gap 12px, padding 14px 16px, radius 8px, border 2px, shadow-sm, margin-bottom 10px.
- **Icon box:** 34px square, radius 8px, border 1px gray-300, bg white. Inner icon 14px gray-700.
- **Name:** 12px weight 700, monospace font (Consolas), gray-900.
- **Status icon:** 14px, right-aligned.

### Variants

| Status | Card bg | Card border | Status icon | Sub-label |
|---|---|---|---|---|
| Success | rgba(82,196,26,0.05) | rgba(82,196,26,0.3) | Checkmark #52c41a | none |
| Processing | rgba(230,244,255,0.3) | rgba(22,119,255,0.3) | Spinner blue-600, rotating 1s | "Processing..." 10px gray-400 |
| Error | rgba(255,77,79,0.05) | rgba(255,77,79,0.3) | X mark #ff4d4f | none |

Tool icon per type: Database icon for `search_database`, Code brackets for `execute_code`, Globe for `api_request`.

---

## Chat Input Bar

Pinned to bottom, never scrolls.

- Border-top 1px gray-200, padding 16px 20px, bg white, shadow 0 -1px 3px rgba(0,0,0,0.05).
- Inner wrapper: max-width 780px, margin 0 auto.

### Input Row (flex, gap 8px, align end)
- **Attach button:** 38px square, radius 8px, transparent, hover gray-100. Paperclip icon 18px gray-400.
- **Textarea:** flex:1, min-height 48px, max-height 160px, bg white, border 1px gray-300, radius 8px, padding 12px 14px, 14px font. Placeholder: "Ask about analytics, insights, or request data visualizations..." gray-400. Focus: border brand-300, ring 4px brand-100. Auto-resizes with content.
- **Mic button:** same as attach, Microphone icon.
- **Send button:** 38px square, radius 8px, bg blue-600 (Ant) / brand-700 (Habibi), shadow-sm. Send icon 18px white. Default: opacity 0.5. Active (text entered): opacity 1. Hover when active: bg lightens, translateY(-1px).

### Footer Row
- Flex between, margin-top 8px, padding 0 4px. Left: "Press Enter to send, Shift+Enter for new line" 10px gray-400. Right: "0 characters" 10px weight 500 gray-400 (updates live).

### Behavior
- Textarea auto-grows up to 160px then scrolls internally. Enter submits. Shift+Enter inserts newline. Send button activates when textarea has content.

---

## Stat Cards (for dashboard rows)

- Grid: 3 or 5 columns, gap 24px.
- Each card: bg white, border 1px gray-200, radius 12px, padding 24px, shadow-xs.
- Header: flex between — label 14px weight 500 gray-500 + info icon 16px gray-400.
- Value: 30px weight 600 gray-900, margin-top 8px.

---

## Proposed Plan Card

- Bg white, border 1px gray-200, radius 12px, overflow hidden.
- **Header:** padding 20px 24px, flex between. Title "Proposed Plan" 16px weight 600 gray-900. Version badge: brand pill "Version 1".
- **Body:** padding 0 24px 16px. Ordered list, 14px gray-700, line-height 1.8, left-padding 20px.
- **Footer:** padding 16px 24px, border-top 1px gray-200, flex end gap 12px. "Edit Plan" (secondary gray) + "Approve Plan" (primary).

---

## Available Agents Table

- Bg white, border 1px gray-200, radius 12px.
- **Header:** padding 16px 24px, border-bottom 1px gray-200. Title 14px weight 600 gray-900 + "Past 20 Seconds" 12px gray-500.
- **Rows:** padding 12px 24px, border-bottom 1px gray-100. Name 14px gray-700 left. Status badge right (success/error pill per spec).

---

## Toast Notifications

- Min-width 300px, padding 12px 16px, radius 8px, 14px weight 600 white, shadow-md.
- Types: Success (#12B76A), Error (#F04438), Warning (#F79009), Info (#2E90FA), Custom (#6941C6), Loading (gray-200, text gray-700).
- Animation: slide-in from right 200ms, auto-dismiss after 4s, fade-out 150ms.
