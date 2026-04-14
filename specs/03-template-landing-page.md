# Template: Landing / Marketing Page

> A hero + feature grid + theme preview page for marketing the AI Chat UI library. No sidebar — full-width single-column layout. Read `00-design-tokens.md` first.

---

## Page Layout

Full viewport width, single scrollable column. No sidebar, no topnav. Vertically stacked sections.

---

## Section 1: Hero

### Background
- Gradient: blue-50 (#EFF8FF) at top → white (#FFFFFF) at bottom, covering ~220px height.

### Content (centered)
- **Badge pill:** "✦ AI Chat UI Component Library" — border 1px gray-200, bg white, radius full, padding 6px 16px, 12px weight 500 gray-700. Centered. Sparkle icon inline.
- **Heading:** "Build Beautiful AI Chat Interfaces" — display-lg (48px weight 800 gray-900, tracking tight). Centered. Margin-top 20px.
- **Subtitle:** 14px weight 400 gray-500, centered, max-width 480px, line-height 1.6. Margin-top 12px.
- **Buttons row:** flex row gap 12px, centered, margin-top 24px.
  - "View Components" — bg gray-900, text white, padding 10px 20px, radius 8px, 14px weight 600. Gear icon left.
  - "Live Demo" — bg white, border 1px gray-300, text gray-700, padding 10px 20px, radius 8px, 14px weight 600. Grid icon left.

---

## Section 2: What's Included

- Margin-top 80px. Centered.
- **Title:** "What's Included" — 20px weight 700 gray-900, centered.
- **Subtitle:** 14px gray-500, centered, margin-top 8px.

### Feature Grid
- 4-column grid, gap 16px, margin-top 32px, max-width 900px centered.

#### Feature Card
- Bg white, border 1px gray-200, radius 12px, padding 20px.
- **Icon box:** 40px square, radius 8px, flex center.
- **Title:** 14px weight 600 gray-900, margin-top 12px.
- **Description:** 12px gray-500, margin-top 4px, line-height 1.5.

| Card | Icon Bg | Icon Color | Title |
|---|---|---|---|
| Chat Components | blue-50 | blue-600 | Chat Components |
| Navigation | brand-50 | brand-600 | Navigation |
| Data Visualization | error-50 | error-600 | Data Visualization |
| Tool Integrations | gray-100 | gray-600 | Tool Integrations |

---

## Section 3: Theme Preview

- Bg gray-50, border 1px gray-200, radius 12px, padding 32px, max-width 800px centered, margin-top 48px.
- **Title:** "Shadcn-Style Theme System" — 16px weight 700 gray-900, centered.

### Color Swatches Row
- Flex row, gap 16px, centered, margin-top 20px.
- Each swatch: 120px wide, 44px tall, radius 12px, centered text 13px weight 600 white.
- Hex code below: 11px gray-400, centered, margin-top 4px.

#### Theme Variants

**Shadcn:** Primary #18181b, Secondary #F4F4F5 (text dark), Destructive #ef4444, Success #18b981, Warning #f59e0b

**Ant Design:** Primary #1677FF, Success #52c41a, Warning #faad14, Error #ff4d4f, Info #e6f4ff (text dark)

**Custom Unilever:** Primary #005EEF, Secondary #7179BC, Accent #5925DC, Success #00B651, Warning #F79009

### Note Bar
- Margin-top 16px. Bg gray-50, border-left 3px blue-600, padding 12px 16px. Text 13px gray-600. Code reference in monospace bg gray-100 padding 2px 6px radius 4px.

---

## Section 4: CTA Footer

- Margin-top 80px, padding-bottom 60px, centered.
- **Title:** "Ready to Build?" — 20px weight 700 gray-900.
- **Subtitle:** 14px gray-500, margin-top 8px.
- **Buttons:** flex row gap 12px, margin-top 24px. "Browse Components" (primary) + "View Full Template" (secondary gray).

---

## Footer Bar

- Padding 20px 40px, border-top 1px gray-200, flex between.
- Left: "AI Chat UI Component Library" — 12px gray-400.
- Right: "Built with React + Tailwind CSS" — 12px gray-400.
