# 13 — Tabs & Navigation

> Tab controls for switching between content views.

---

## Underline Tabs

### Container

- **Display:** flex row
- **Border bottom:** 1px solid gray-200

### Tab Item

- **Padding:** 12px 16px
- **Font:** 14px (text-sm)
- **Cursor:** pointer

### Active Tab

- **Font weight:** 600
- **Color:** brand-600 (#6941C6)
- **Border bottom:** 2px solid brand-600 (#6941C6), positioned flush with container border

### Inactive Tab

- **Font weight:** 400
- **Color:** gray-500
- **Hover color:** gray-700

## Pill Tabs

### Container

- **Display:** flex row, gap 4px
- **Padding:** 4px
- **Background:** gray-100 (#F2F4F7)
- **Border radius:** 8px

### Active Pill

- **Padding:** 6px 14px
- **Background:** white
- **Border radius:** 6px
- **Font:** 14px, weight 500, color gray-900
- **Shadow:** shadow-xs

### Inactive Pill

- **Padding:** 6px 14px
- **Background:** transparent
- **Font:** 14px, weight 400, color gray-500

## Breadcrumb

- **Height:** 42px
- **Background:** rgba(255,255,255, 0.5) in light / var(--bg-deep) in dark
- **Border bottom:** 1px solid gray-200 (light) / rgba(255,255,255, 0.06) (dark)
- **Padding:** 0 24px, vertically centered
- **Icon:** ArrowLeft, 14px, same color as text
- **Text:** 12px, weight 400, color blue-600 (#1570EF) in Ant theme / brand-400 (#B692F6) in dark brand theme
- **Gap:** 6px between icon and text
- **Hover:** text underline

---

