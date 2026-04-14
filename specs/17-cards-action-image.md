# 17 — Cards: Action with Image

> Image-header cards with action buttons below, used in the Component Showcase for project/resource cards.

---

## Card Container

- **Width:** varies (typically ~180px in a 3-column grid)
- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-200
- **Border radius:** 12px
- **Shadow:** shadow-xs
- **Overflow:** hidden

## Image Area

- **Height:** 70-80px (top portion of card)
- **Width:** 100%
- **Border radius:** 12px top-left and top-right, 0 bottom
- **Background:** placeholder color or actual image
  - Example fills: blue-100 (#D1E9FF), gray-800 (#1D2939), warning-100 (#FEF0C7)
- **Object fit:** cover (for real images)

## Text Area

- **Padding:** 12px 16px

### Title

- **Font:** 12px, weight 600, color gray-900
- **Text align:** center or left (depending on context)

## Action Row

- **Padding:** 0 16px 12px
- **Display:** flex row, gap 12px

### Action Link

- **Font:** 10px, weight 500
- **Color:** blue-600 (#1570EF) for primary actions, gray-500 for secondary
- **Display:** inline-flex, gap 4px, align-items center
- **Icon:** 10-12px, same color as text
- **Hover:** underline
- **Examples:** "👁 View", "✏ Edit", "⬇ Download", "⬆ Share"

## Grid Usage

- **Display:** grid, 3 columns
- **Gap:** 16px
- **Cards per row:** 3

---

