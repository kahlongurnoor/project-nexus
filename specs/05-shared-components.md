# Shared UI Components

> Reusable components that appear across multiple templates. Read `00-design-tokens.md` first for all values.

---

## Buttons

**Shared:** font Inter, weight 600, radius 8px, cursor pointer, transition 0.15s. Disabled: opacity 0.5, cursor not-allowed.

| Variant | Background | Text | Border | Hover |
|---|---|---|---|---|
| Primary | brand-700 | white | none | brand-600 |
| Secondary Color | brand-50 | brand-700 | 1px brand-200 | brand-100 |
| Secondary Gray | white | gray-700 | 1px gray-300 | gray-50 |
| Tertiary Color | transparent | brand-700 | none | brand-50 |
| Tertiary Gray | transparent | gray-500 | none | gray-50, text gray-700 |
| Destructive | error-600 | white | none | error-700 |

**Sizes:** sm (8px/14px vertical/horizontal, 14px font, 36px tall), md (10px/18px, 14px, 40px), lg (12px/20px, 16px, 44px).

**Focus:** 4px ring — brand-100 for brand buttons, error-100 for destructive.

**Sub-types:** text-only, leading icon, trailing icon, icon-only (square), dot indicator (6px circle + gap + label).

---

## Badges & Pills

Inline-flex, gap 6px, padding 2px 10px, radius full, 12px weight 500.

| Variant | Background | Text | Dot Color |
|---|---|---|---|
| Success/Active | success-50 | success-700 | success-500 |
| Error/Inactive | error-50 | error-700 | error-500 |
| Warning/Pending | warning-50 | warning-700 | warning-500 |
| Brand/Version | brand-50 | brand-700 | — |
| Info | blue-50 | blue-700 | — |
| Neutral | gray-100 | gray-700 | — |

**Filter pills (selectable):** Active: brand-50 bg, brand-700 text. Inactive: white bg, 1px gray-200 border, gray-600 text, hover gray-50.

---

## Form Inputs

### Text Input
- Label: 14px weight 500 gray-700, margin-bottom 6px.
- Input: 100% wide, 40px tall, padding 10px 14px, bg white, border 1px gray-300, radius 8px, 14px gray-900. Placeholder: gray-400. Focus: border brand-300, ring 4px brand-100.
- Helper: 14px gray-500, margin-top 6px. Error: 14px error-700.

### Textarea
- Same as input but multi-line, min-height 96px, resize vertical.

### Dropdown
- Trigger: same as text input + ChevronDown 14px gray-400 right.
- Panel: bg white, border 1px gray-200, radius 8px, shadow-lg, padding 4px vertical, max-height 240px scroll.
- Item: padding 8px 12px, 14px gray-700, hover gray-50. Divider: 1px gray-100 margin 4px.

### Checkbox
- 16px square, border 2px gray-300, radius 4px, bg white. Checked: border brand-600, bg brand-50, checkmark "✓" 10px brand-600.
- With label: flex row gap 8px. Title 14px weight 500 gray-700, description 14px gray-500.

### Radio
- 16px circle, border 2px gray-300, bg white. Selected: border 5px brand-600 (thick border = filled center).
- Group: flex row gap 16px or column gap 12px. Label: 14px gray-700.

---

## Tabs

### Underline Tabs
- Container: flex row, border-bottom 1px gray-200.
- Active: padding 12px 16px, 14px weight 600 brand-600, border-bottom 2px brand-600.
- Inactive: same padding, 14px weight 400 gray-500, hover gray-700.

### Pill Tabs
- Container: flex row gap 4px, padding 4px, bg gray-100, radius 8px.
- Active: padding 6px 14px, bg white, radius 6px, 14px weight 500 gray-900, shadow-xs.
- Inactive: same padding, transparent bg, 14px gray-500.

---

## Modals

### Backdrop
- Fixed inset 0, bg rgba(16,24,40,0.6), flex center, z-index 50.

### Container
- Bg white, radius 12px, shadow-xl, max-width varies (400/512/640px), margin 0 16px.

### Structure
- **Header:** padding 20px 24px, border-bottom 1px gray-200. Title 16px weight 600 gray-900 + close X button gray-400.
- **Body:** padding 20px 24px.
- **Footer:** padding 16px 24px, border-top 1px gray-200, flex end gap 12px.

### Confirmation (centered icon)
- Max-width 400px, padding 24px, text-align center.
- Icon circle: 48px, radius 50%. Success: bg success-100, icon success-600. Destructive: bg error-100, icon error-600.
- Title: 18px weight 600 gray-900, margin-top 16px. Description: 14px gray-500, margin-top 8px.
- Buttons: margin-top 24px. Single (full-width) or dual (flex row gap 12px).

### Date Picker
- Max-width 320px, padding 16px. Month header: 14px weight 600 + nav arrows. Day grid: 7 columns, 36px cells. Selected: bg brand-600 text white radius 50%. Today: border 1px brand-600.

### Data Table Modal
- Max-width 600px. Table header: bg gray-50, 12px weight 600 gray-500 uppercase. Body rows: 13px gray-700, hover gray-50. Scrollable body.

### Form Modal
- Max-width 480px. Colored left accent bars (3px wide) per section — success/warning/error/blue. Standard form inputs.

---

## Scrollbar
- Width 6px, track transparent, thumb gray-300 (light) / #2E2E38 (dark), hover gray-400 / #52525B, radius 3px.
