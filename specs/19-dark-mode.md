# 19 — Dark Mode Rules

> How every token maps from light to dark theme. When building dark mode, swap every value listed below — do not mix light and dark tokens.

---

## Surface Colors

| Role | Light | Dark |
|---|---|---|
| App background | white (#FFFFFF) | #09090B |
| Sidebar background | #001529 (same) | #001529 (same) |
| Top nav background | white | #0C0C10 |
| Content background | white | #111116 |
| AI message background | gray-50 (#F9FAFB) | #18181E |
| User message background | white | #111116 |
| Card / elevated surface | white | #18181E |
| Raised surface (tool icons, dropdowns) | white | #1F1F27 |
| Hover state | gray-100 (#F2F4F7) | #27272F |
| Active/pressed state | gray-200 (#E4E7EC) | #2E2E38 |
| Input background | white | #18181E |

## Text Colors

| Role | Light | Dark |
|---|---|---|
| Primary text | gray-900 (#101828) | #F4F4F5 |
| Secondary text | gray-700 (#344054) | #A1A1AA |
| Tertiary text / labels | gray-500 (#667085) | #71717A |
| Ghost text / placeholders | gray-400 (#98A2B3) | #52525B |
| Timestamps | gray-400 (#98A2B3) | #52525B |

## Border Colors

| Role | Light | Dark |
|---|---|---|
| Default border | gray-200 (#E4E7EC) | rgba(255,255,255, 0.1) |
| Strong border / inputs | gray-300 (#D0D5DD) | rgba(255,255,255, 0.16) |
| Subtle border / dividers | gray-200 (#E4E7EC) | rgba(255,255,255, 0.06) |
| Focus border | brand-300 (#D6BBFB) | brand-600 (#7F56D9) |

## Interactive Colors

| Role | Light | Dark |
|---|---|---|
| Primary button / CTA | brand-600 (#6941C6) | brand-600 (#7F56D9) |
| Primary hover | brand-700 (#7F56D9) | brand-500 (#9E77ED) |
| Chart line | blue-600 (#1570EF) | brand-500 (#9E77ED) |
| Chart area fill | rgba(22,119,255, 0.08) | rgba(158,119,237, 0.08) |
| Link text | blue-600 (#1570EF) | brand-400 (#B692F6) |
| Section label accent | blue-600 (#1570EF) | brand-400 (#B692F6) |

## Icon Colors

| Role | Light | Dark |
|---|---|---|
| Default icons | gray-500 (#667085) | #71717A |
| Ghost icons | gray-400 (#98A2B3) | #52525B |
| Interactive icons (hover) | gray-600 (#475467) | #A1A1AA |

## Shadows

In dark mode, shadows become more pronounced since the background is dark:

| Light | Dark |
|---|---|
| shadow-xs | 0 1px 2px rgba(0,0,0, 0.2) |
| shadow-sm | 0 2px 8px rgba(0,0,0, 0.5), 0 0 1px rgba(0,0,0, 0.4) |
| shadow-glow (brand) | 0 0 20px rgba(127,86,217, 0.1) — added on hover for cards |

## Scrollbar

| Part | Light | Dark |
|---|---|---|
| Track | transparent | transparent |
| Thumb | gray-300 (#D0D5DD) | #2E2E38 |
| Thumb hover | gray-400 (#98A2B3) | #52525B |
| Width | 6px | 6px |

---

