# 12 — Form Inputs

> Text inputs, textareas, email subscribe, and dropdown menus.

---

## Text Input

### Label

- **Font:** 14px (text-sm), weight 500, color gray-700
- **Margin bottom:** 6px

### Input Field

- **Width:** 100% of parent
- **Height:** 40px (single line), auto for textarea
- **Padding:** 10px 14px
- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-300 (light) / rgba(255,255,255, 0.1) (dark)
- **Border radius:** 8px (radius-md)
- **Font:** 14px, weight 400, color gray-900 (light) / #F4F4F5 (dark)
- **Placeholder:** color gray-400 (light) / #52525B (dark)
- **Focus border:** brand-300 (#D6BBFB) in light / brand-600 (#7F56D9) in dark
- **Focus ring:** 0 0 0 4px brand-100 (#F4EBFF) in light / 0 0 0 3px rgba(127,86,217, 0.15) in dark
- **Error border:** error-300 (#FDA29B)
- **Error ring:** 0 0 0 4px error-100 (#FEE4E2)

### Helper Text

- **Font:** 14px (text-sm), weight 400, color gray-500
- **Margin top:** 6px

### Error Text

- **Font:** 14px (text-sm), weight 400, color error-700 (#B42318)
- **Margin top:** 6px

## Email Subscribe

- **Layout:** flex row, gap 8px
- **Input:** flex 1, standard text input styling
- **Button:** primary button, "Subscribe" label, aligned to bottom of input

## Dropdown / Select Menu

### Trigger

- Same as text input, with a ChevronDown icon (14px) on the right side, color gray-400

### Dropdown Panel

- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-200 (light) / rgba(255,255,255, 0.1) (dark)
- **Border radius:** 8px
- **Shadow:** shadow-lg
- **Padding:** 4px vertical
- **Max height:** 240px, overflow-y auto

### Dropdown Item

- **Padding:** 8px 12px
- **Font:** 14px, weight 400, color gray-700
- **Hover:** gray-50 background
- **Keyboard shortcut (optional):** right-aligned, font 12px, color gray-400

### Dropdown Divider

- **Height:** 1px
- **Background:** gray-100
- **Margin:** 4px vertical

---

