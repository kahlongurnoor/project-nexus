# 23 — Form Controls (Extended)

> Additional form controls visible on the Smaller Widgets page not covered in spec 12.

---

## Checkbox

### Unchecked

- **Size:** 16×16px
- **Border:** 2px solid gray-300
- **Border radius:** 4px
- **Background:** white

### Checked

- **Border:** 2px solid brand-600 (#6941C6)
- **Background:** brand-50 (#F9F5FF)
- **Checkmark:** "✓" character or SVG, color brand-600, centered
- **Font size of checkmark:** 10px

### With Label

- **Layout:** flex row, gap 8px, align-items flex-start
- **Checkbox:** margin-top 2px (aligns with first line of text)
- **Label title:** 14px, weight 500, gray-700
- **Label description (optional):** 14px, weight 400, gray-500, margin-top 2px

---

## Radio Button

### Unselected

- **Size:** 16×16px
- **Border:** 2px solid gray-300
- **Border radius:** 50% (circle)
- **Background:** white

### Selected

- **Border:** 5px solid brand-600 (#6941C6)
- **Background:** white
- **Visual:** thick border creates the filled-center effect

### Radio Group

- **Layout:** flex row, gap 16px (horizontal) or flex column, gap 12px (vertical)
- **Each option:** flex row, gap 8px, align-items center
- **Label:** 14px, weight 400, gray-700

---

## Scrollbar

Custom scrollbar styling for scrollable containers.

- **Width:** 6px
- **Track:** transparent background
- **Thumb:** gray-300 (#D0D5DD) in light / #2E2E38 in dark
- **Thumb hover:** gray-400 (#98A2B3) in light / #52525B in dark
- **Thumb border-radius:** 3px
- **Visibility:** auto-hide after 2 seconds of inactivity (CSS overflow behavior)

Figma shows two variants:
- **Vertical scrollbar:** right edge of scrollable container
- **Horizontal scrollbar:** bottom edge (rare, used for wide tables)

---

## Accordion / FAQ

Collapsible content sections.

### Container

- **Border:** 1px solid gray-200
- **Border radius:** 12px
- **Background:** white
- **Overflow:** hidden (rounded corners on first/last items)

### Accordion Item

- **Padding:** 16px 20px
- **Border bottom:** 1px solid gray-100 (except last item)
- **Cursor:** pointer

#### Header Row

- **Display:** flex row, justify-content space-between, align-items center
- **Title:** 14px, weight 500, gray-900
- **Chevron:** 16px, color gray-400, rotates 180deg when expanded

#### Content (expanded)

- **Padding top:** 8px
- **Font:** 14px, weight 400, gray-500
- **Line height:** 1.6
- **Animation:** height transition 200ms ease

---

## Menu Bar

A traditional application-style menu bar (File, Edit, View, Profile).

### Bar

- **Height:** 40px
- **Background:** white
- **Border bottom:** 1px solid gray-200
- **Display:** flex row, align-items center

### Menu Item

- **Padding:** 8px 16px
- **Font:** 14px, weight 400, gray-700
- **Hover:** bg gray-100
- **Active/open:** bg gray-100, font-weight 500

### Dropdown Panel

- Same as spec 12 dropdown panel styling

---

## Segmented Control

A toggle group where one option is selected at a time (like pill tabs but for form values).

### Container

- **Display:** flex row
- **Border:** 1px solid gray-200
- **Border radius:** 8px
- **Overflow:** hidden (segments flush against container edges)

### Segment

- **Padding:** 8px 16px
- **Font:** 14px, weight 500
- **Border right:** 1px solid gray-200 (except last)

#### Selected Segment

- **Background:** gray-900 (#101828) or brand-600
- **Color:** white

#### Unselected Segment

- **Background:** white
- **Color:** gray-700
- **Hover:** bg gray-50

---

## Width/Value Input

A labeled input for numeric CSS-like values.

### Layout

- **Display:** flex row, align-items center, gap 8px
- **Label:** 14px, weight 500, gray-700 (e.g. "Width")
- **Input:** 80px wide, standard text input style (spec 12)
- **Value format:** text or "Auto value" placeholder in gray-400
