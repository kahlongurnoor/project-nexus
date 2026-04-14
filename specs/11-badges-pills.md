# 11 — Badges & Pills

> Small status indicators and category labels used throughout the system.

---

## Structure

- **Display:** inline-flex, align-items center, gap 6px
- **Padding:** 2px vertical, 10px horizontal
- **Border radius:** 9999px (full pill)
- **Font:** 12px (text-xs), weight 500

## Variants

### Success / Active

- **Background:** success-50 (#ECFDF3)
- **Text color:** success-700 (#027A48)
- **Optional dot:** 6px circle, background success-500 (#12B76A)

### Error / Inactive

- **Background:** error-50 (#FEF3F2)
- **Text color:** error-700 (#B42318)
- **Optional dot:** 6px circle, background error-500 (#F04438)

### Warning / Pending

- **Background:** warning-50 (#FFFAEB)
- **Text color:** warning-700 (#B54708)
- **Optional dot:** 6px circle, background warning-500 (#F79009)

### Brand / Version

- **Background:** brand-50 (#F9F5FF)
- **Text color:** brand-700 (#6941C6)
- **No dot**

### Info / Blue

- **Background:** blue-50 (#EFF8FF)
- **Text color:** blue-700 (#175CD3)
- **No dot**

### Gray / Neutral

- **Background:** gray-100 (#F2F4F7)
- **Text color:** gray-700 (#344054)
- **No dot**

## Quick Filter Pills (selectable)

Used in filter rows where one pill is active:

### Active Pill

- **Background:** brand-50 (#F9F5FF)
- **Text color:** brand-700 (#6941C6)
- **Font weight:** 500

### Inactive Pill

- **Background:** white
- **Border:** 1px solid gray-200 (#E4E7EC)
- **Text color:** gray-600 (#475467)
- **Hover:** gray-50 background
