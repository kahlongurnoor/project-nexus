# 15 — Toast Notifications

> Transient alert banners, typically appearing in the bottom-right or top-right of the viewport.

---

## Container

- **Min width:** 300px
- **Padding:** 12px 16px
- **Border radius:** 8px (radius-md)
- **Font:** 14px, weight 600, color white
- **Shadow:** shadow-md

## Variants

| Type | Background | Text Color |
|---|---|---|
| Success | success-500 (#12B76A) | white |
| Error | error-500 (#F04438) | white |
| Warning | warning-500 (#F79009) | white |
| Info | blue-500 (#2E90FA) | white |
| Custom | brand-700 (#6941C6) | white |
| Loading | gray-200 (#E4E7EC) | gray-700 (#344054) |

## Layout

- **Display:** flex row, align-items center, gap 8px
- **Icon (optional):** 16px, color white (or gray-700 for loading)
- **Text:** flex 1
- **Dismiss X (optional):** 14px, color white, hover opacity 0.8

## Behavior

- **Entry animation:** slide in from right, fade in (200ms ease-out)
- **Duration:** 4 seconds default, then auto-dismiss
- **Exit animation:** fade out, slide right (150ms ease-in)
- **Stacking:** multiple toasts stack vertically with 8px gap
