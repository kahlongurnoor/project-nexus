# 14 — Modals & Dialogs

> Overlay panels for confirmations, details, and forms.

---

## Backdrop

- **Position:** fixed, inset 0
- **Background:** rgba(16,24,40, 0.6) in light / rgba(0,0,0, 0.7) in dark
- **Display:** flex, align-items center, justify-content center
- **Z-index:** 50

## Modal Container

- **Background:** white (light) / #18181E (dark)
- **Border radius:** 12px (radius-lg)
- **Shadow:** shadow-xl
- **Width:** 100%, max-width varies by type (sm: 400px, md: 512px, lg: 640px)
- **Margin:** 0 16px (safety margin from viewport edges)

## Header

- **Padding:** 20px 24px
- **Border bottom:** 1px solid gray-200 (light) / rgba(255,255,255, 0.06) (dark)
- **Display:** flex row, justify-content space-between, align-items center
- **Title:** 16-18px, weight 600, color gray-900 (light) / #F4F4F5 (dark)
- **Close button:** 20×20px icon button, X icon, color gray-400, hover gray-600

## Body

- **Padding:** 20px 24px

## Footer

- **Padding:** 16px 24px
- **Border top:** 1px solid gray-200 (light) / rgba(255,255,255, 0.06) (dark)
- **Display:** flex row, justify-content flex-end, gap 12px
- **Buttons:** secondary gray (left), primary (right)

## Confirmation Dialog (centered icon variant)

- **Max width:** 400px
- **Padding:** 24px
- **Text align:** center
- **Icon circle:** 48×48px, border-radius 50%
  - Success: bg success-100 (#D1FADF), icon color success-600 (#039855)
  - Destructive: bg error-100 (#FEE4E2), icon color error-600 (#D92D20)
- **Title:** 18px, weight 600, color gray-900, margin-top 16px
- **Description:** 14px, weight 400, color gray-500, margin-top 8px
- **Button(s):** margin-top 24px, full width (single) or flex row gap 12px (dual)

---

