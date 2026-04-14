# 22 — Modals (Extended)

> Additional modal types from the Figma Modals page not covered in spec 14.

---

## Date Picker Modal

A calendar-based date selection modal.

### Container

- **Width:** max-width 320px
- **Background:** white, radius 12px, shadow shadow-lg
- **Padding:** 16px

### Month/Year Header

- **Display:** flex row, justify-content space-between, align-items center
- **Month/Year text:** 14px, weight 600, gray-900 (e.g. "January 2025")
- **Nav arrows:** left/right chevrons, 16px, color gray-400, hover gray-700

### Day Grid

- **Display:** grid, 7 columns
- **Day-of-week labels:** 12px, weight 500, gray-500, text-align center (S, M, T, W, T, F, S)
- **Day cells:** 36×36px, text-align center, font 14px
  - **Default:** color gray-700, bg transparent
  - **Today:** border 1px brand-600, radius 50%
  - **Selected:** bg brand-600, color white, radius 50%
  - **Range (between):** bg brand-50, color brand-700
  - **Disabled/out-of-month:** color gray-300
  - **Hover:** bg gray-100, radius 50%

### Footer

- **Border top:** 1px gray-200, margin-top 12px, padding-top 12px
- **Display:** flex row, gap 8px
- **Date input:** text input showing selected date (e.g. "Jan 15, 2025"), 12px, gray-700
- **Apply button:** primary small button, "Select" or "Apply"

---

## Data Table Modal

A scrollable table inside a modal, used for event type distributions, metrics breakdowns.

### Container

- **Width:** max-width 600px
- **Background:** white, radius 12px

### Header

- **Padding:** 16px 20px
- **Title:** 16px, weight 600, gray-900 (e.g. "Event Type Distribution Table")
- **Close:** X icon button, top-right

### Table

- **Width:** 100%
- **Border-collapse:** collapse

#### Table Header Row

- **Background:** gray-50
- **Padding:** 10px 16px per cell
- **Font:** 12px, weight 600, gray-500, text-transform uppercase, letter-spacing 0.05em
- **Columns:** Type (left), Count (center), Percentage (right)
- **Border bottom:** 1px gray-200

#### Table Body Rows

- **Padding:** 10px 16px per cell
- **Font:** 13px, weight 400, gray-700
- **Border bottom:** 1px gray-100
- **Hover:** bg gray-50

#### Percentage Cell

- **Font:** 13px, monospace or tabular-nums
- **Alignment:** right

### Footer

- **Padding:** 12px 20px
- **Border top:** 1px gray-200
- **Button:** primary, "Save Results" or "Close"

---

## Form Modal (Create Red Team Test)

A structured form inside a modal for creating tests, tasks, or records.

### Container

- **Width:** max-width 480px
- **Background:** white, radius 12px

### Header

- **Padding:** 16px 20px
- **Title:** "Create Red Team Test" — 16px, weight 600, gray-900
- **Close:** X icon, top-right

### Form Body

- **Padding:** 20px
- **Display:** flex column, gap 16px

#### Form Sections (stacked)

Each section has a colored left accent bar + content:

- **Section container:** flex row, gap 12px
- **Left accent bar:** 3px wide, radius 2px, full height
  - Color varies: success-500 (green), warning-500 (orange), error-500 (red), blue-500 (info)
- **Section content:** flex column, gap 4px
  - **Label:** 13px, weight 600, color matching the accent bar
  - **Description:** 13px, weight 400, gray-500, line-height 1.5

#### Input Fields

- Standard text inputs (see spec 12)
- Labels: 14px, weight 500, gray-700
- Helper text below inputs

#### Category/Priority Selectors

- **Layout:** 2-column grid (Category | Priority)
- **Each:** dropdown select (see spec 12 dropdown)

### Footer

- **Padding:** 16px 20px
- **Border top:** 1px gray-200
- **Display:** flex row, justify-content flex-end, gap 12px
- **Buttons:** "Cancel" (secondary gray) + "Create Test" (destructive/primary)

---

## Feedback Details Modal

A key-value detail view for inspecting individual feedback records.

### Container

- **Width:** max-width 400px
- **Background:** white, radius 12px

### Header

- **Padding:** 16px 20px
- **Title:** "Feedback Details" — 16px, weight 600, gray-900

### Body — Key-Value Rows

- **Padding:** 16px 20px
- **Each row:** flex row, justify-content space-between, padding 8px 0, border-bottom 1px gray-100

#### Key

- **Font:** 13px, weight 400, gray-500

#### Value

- **Font:** 13px, weight 500, gray-900
- **Special formatting:**
  - Status values: use badge/pill (spec 11) — e.g. "Approved" in green pill, "Rejected" in red pill
  - Links: color brand-600, underline on hover
  - "Converted: P.I. ↗" — link style with external arrow icon

### Footer

- **Padding:** 12px 20px
- **Border top:** 1px gray-200
- **Buttons:** "Cancel" (secondary gray) + "Save Changes" (primary)

---

## Filter/Sort Modal (Show by Individual Metrics)

A two-column selection modal for choosing data dimensions.

### Container

- **Width:** max-width 480px

### Body

- **Display:** 2-column grid, gap 24px
- **Each column:** vertical list of options

#### Option Row

- **Padding:** 8px 0
- **Display:** flex row, gap 8px, align-items center
- **Radio/checkbox:** standard form control (see spec 12)
- **Label:** 14px, gray-700

#### Column Labels

- Left column: "Dimension" / "Priority" / etc.
- Right column: "Metric" / "Grouping" / etc.
- Label font: 12px, weight 600, gray-500, text-transform uppercase
