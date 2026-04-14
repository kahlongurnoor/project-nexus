# 05 — Chat Messages

> The conversation thread displayed in the main content area. Alternating AI and user messages with distinct visual treatments.

---

## Message Container

- **Display:** flex row, gap 14px
- **Padding:** 24px horizontal, 24px top, 6px bottom
- **Width:** 100%

### Background Alternation

- **AI messages:** gray-50 (#F9FAFB) in light / #18181E in dark
- **User messages:** white (#FFFFFF) in light / #111116 in dark

## Avatar

- **Size:** 34×34px (32px in some variants)
- **Border radius:** 8px (radius-md) — square with rounded corners, not circular
- **Flex shrink:** 0 (never collapse)

### AI Avatar

- **Background:** white (light) / #1F1F27 (dark)
- **Border:** 2px solid gray-300 (light) / 1.5px solid rgba(255,255,255, 0.16) (dark)
- **Icon:** Bot icon, 18×18px, color gray-700 (light) / #71717A (dark)

### User Avatar

- **Background:** blue-600 (#1570EF) for Ant theme, or brand-600 (#7F56D9) for brand theme
- **Border:** none
- **Icon:** User icon, 18×18px, color white
- **Shadow (dark mode):** 0 0 10px rgba(127,86,217, 0.2)

## Message Body

- **Flex:** 1 (fill remaining width)
- **Min width:** 0 (allow text to wrap)

### Header Row

- **Display:** flex row, align-items center, gap 8px
- **Margin bottom:** 6px

#### Name

- **Font:** 12px, weight 600, color gray-900 (light) / #F4F4F5 (dark)
- **Text:** "AI Assistant" or "You"

#### Timestamp

- **Font:** 10px (text-xs), weight 400, color gray-400 (light) / #52525B (dark)
- **Text:** e.g. "10:00 AM"

### Message Text

- **Font:** 14px (text-sm), weight 400
- **Line height:** 1.75 (24.5px)
- **Color:** gray-900 (light) / #A1A1AA (dark)
- **Word wrap:** normal (allow long text to wrap naturally)

### Action Buttons Row (AI messages only)

- **Display:** flex row, gap 2px
- **Margin top:** 10px
- **Padding bottom:** 10px

#### Action Button

- **Size:** 28×28px (30×30px in dark)
- **Border radius:** 8px (radius-md)
- **Background:** transparent
- **Hover background:** gray-200 (light) / #27272F (dark)
- **Icon size:** 14×14px
- **Icon color:** gray-400 (light) / #52525B (dark)
- **Hover icon color:** gray-600 (light) / #A1A1AA (dark)

#### Actions (left to right)

1. **Copy** — two-rectangles icon
2. **Thumbs Up** — thumbs-up icon
3. **Thumbs Down** — thumbs-down icon
