# 10 — Buttons

> All button variants, sizes, and states used across the design system.

---

## Shared Properties

- **Font family:** Inter
- **Font weight:** 600 (semibold)
- **Border radius:** 8px (radius-md)
- **Cursor:** pointer
- **Transition:** background 0.15s, box-shadow 0.15s
- **Disabled:** opacity 0.5, cursor not-allowed, no hover effects

## Variants

### Primary

- **Background:** brand-600 (#6941C6)
- **Text color:** white
- **Border:** none
- **Hover:** brand-700 (#7F56D9)
- **Focus ring:** 4px, brand-100 (#F4EBFF)
- **Shadow:** shadow-sm

### Secondary Color

- **Background:** brand-50 (#F9F5FF)
- **Text color:** brand-700 (#6941C6)
- **Border:** 1px solid brand-200 (#E9D7FE)
- **Hover:** brand-100 (#F4EBFF)

### Secondary Gray

- **Background:** white
- **Text color:** gray-700 (#344054)
- **Border:** 1px solid gray-300 (#D0D5DD)
- **Hover:** gray-50 (#F9FAFB)
- **Shadow:** shadow-xs

### Tertiary Color

- **Background:** transparent
- **Text color:** brand-700 (#6941C6)
- **Border:** none
- **Hover:** brand-50 (#F9F5FF)

### Tertiary Gray

- **Background:** transparent
- **Text color:** gray-500 (#667085)
- **Border:** none
- **Hover:** gray-50 (#F9FAFB), text darkens to gray-700

### Destructive

- **Background:** error-600 (#D92D20)
- **Text color:** white
- **Border:** none
- **Hover:** error-700 (#B42318)
- **Focus ring:** 4px, error-100 (#FEE4E2)

## Sizes

| Size | Padding | Font Size | Approx Height | Gap (icon to text) |
|---|---|---|---|---|
| sm | 8px vertical, 14px horizontal | 14px | 36px | 8px |
| md | 10px vertical, 18px horizontal | 14px | 40px | 8px |
| lg | 12px vertical, 20px horizontal | 16px | 44px | 8px |

## Sub-Variants

- **Text only:** just the label, no icon
- **Leading icon:** icon (16-20px) + 8px gap + label
- **Trailing icon:** label + 8px gap + icon (16-20px)
- **Icon only:** square button (same height as width), icon centered, no text
- **Dot indicator:** 6px colored circle + 8px gap + label (for status buttons)
