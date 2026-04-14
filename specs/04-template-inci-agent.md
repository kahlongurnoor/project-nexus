# Template: Product Information / INCI Agent

> A structured data display for product ingredient information. Uses the same sidebar + topnav shell as the AI Chat Agent. Read `00-design-tokens.md` first.

---

## Page Layout

Same layout shell: sidebar (224px) + main. The main content area shows one or more INCI cards stacked vertically with 16px gap. No chat input bar at the bottom (this is a read-only data display, not a chat interface).

---

## INCI Card

- **Container:** bg white, border 1px gray-200, radius 12px, padding 24px.

### Target Location Header
- Flex row, gap 8px, align center, margin-bottom 16px.
- **Globe icon:** 20px, gray-400.
- **Label:** "Target Location/Language:" — 14px weight 400 gray-500.
- **Value:** "INCI:Canada/ English_CA" — 14px weight 700 gray-900.

### Ingredient List Section
- **Title:** "≡ Ingredient List:" — 16px weight 600 gray-900. List icon inline. Margin-bottom 8px.
- **Text block:** bg gray-50, border 1px gray-200, radius 8px, padding 16px. Font 14px weight 400 gray-700, line-height 1.6. Full ingredient list, comma-separated.

### Ingredient Statements Section
- **Title:** "📋 Ingredient statements:" — 16px weight 600 gray-900. Margin-bottom 8px. Margin-top 24px.

#### Table
- Width 100%, border 1px gray-200, radius 8px, overflow hidden.
- **Header row:** bg gray-100, padding 8px 16px. Columns: "Purpose" (12px weight 600 gray-700) + "Statement" (same, wider).
- **Body row:** bg white, border-top 1px gray-200, padding 12px 16px.
  - Purpose cell: "⚠ SAFETY INSTRUCTIONS" — 14px weight 500 error-600.
  - Statement cell: "CAUTION:" in error-700 weight 700, then regular text in gray-700 weight 400.

### Variant Support
- Multiple cards for different locales (English_CA, French_CA) — same structure, different content. Stack with 16px gap.
