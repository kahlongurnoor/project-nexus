# 01 — Design Tokens

> All foundational variables used across every component. When building any UI element, reference these tokens — never hardcode values.

---

## Colors

### Brand (Purple) — Primary Interactive

Used for: buttons, links, inputs on focus, active states, selected items, avatars

| Token | Hex | Usage |
|---|---|---|
| brand-25 | #FCFAFF | Lightest hover background |
| brand-50 | #F9F5FF | Selected row, subtle highlight, badge bg |
| brand-100 | #F4EBFF | Light badge bg, pill bg |
| brand-200 | #E9D7FE | Light border, focus ring tint |
| brand-300 | #D6BBFB | Active border state |
| brand-400 | #B692F6 | Placeholder text on dark, disabled icon, chart accent (dark mode) |
| brand-500 | #9E77ED | Mid-emphasis button, chart line (dark mode) |
| brand-600 | #7F56D9 | **Primary button hover**, links hover |
| brand-700 | #6941C6 | **Primary button fill**, links, focus rings |
| brand-800 | #53389E | Dark emphasis text |
| brand-900 | #42307D | Headings on light bg, deepest brand |

### Gray — Neutral Foundation

Used for: text, backgrounds, borders, dividers, form fields, cards

| Token | Hex | Usage |
|---|---|---|
| gray-25 | #FCFCFD | Page bg (lightest) |
| gray-50 | #F9FAFB | Card bg, table row alt, AI message bg |
| gray-100 | #F2F4F7 | Input bg, sidebar bg (light), hover states |
| gray-200 | #E4E7EC | Default borders, dividers, card borders |
| gray-300 | #D0D5DD | Input borders, stronger dividers |
| gray-400 | #98A2B3 | Placeholder text, disabled text, ghost icons |
| gray-500 | #667085 | Supporting text, labels, captions |
| gray-600 | #475467 | Body text (secondary) |
| gray-700 | #344054 | Body text (primary) |
| gray-800 | #1D2939 | Headings, bold text |
| gray-900 | #101828 | Display text, highest contrast |

### Error / Red

Used for: destructive actions, validation errors, critical alerts, error tool calls

| Token | Hex | Usage |
|---|---|---|
| error-50 | #FEF3F2 | Error message bg, error badge bg |
| error-100 | #FEE4E2 | Error highlight |
| error-200 | #FECDCA | Error border light |
| error-300 | #FDA29B | Error input border |
| error-400 | #F97066 | Error icon |
| error-500 | #F04438 | Destructive button fill |
| error-600 | #D92D20 | Destructive button hover |
| error-700 | #B42318 | Error text |
| error-800 | #912018 | Dark error emphasis |
| error-900 | #7A271A | Darkest error |

### Warning / Yellow-Orange

Used for: caution states, pending indicators, non-critical alerts, processing tool calls

| Token | Hex | Usage |
|---|---|---|
| warning-50 | #FFFAEB | Warning alert bg |
| warning-100 | #FEF0C7 | Warning badge bg |
| warning-200 | #FEDF89 | Warning highlight |
| warning-300 | #FEC84B | Warning border |
| warning-400 | #FDB022 | Warning icon |
| warning-500 | #F79009 | Warning indicator |
| warning-600 | #DC6803 | Warning text |
| warning-700 | #B54708 | Dark warning text |
| warning-800 | #93370D | Darker warning |
| warning-900 | #7A2E0E | Darkest warning |

### Success / Green

Used for: confirmation, completion, positive outcomes, success tool calls, active status

| Token | Hex | Usage |
|---|---|---|
| success-50 | #ECFDF3 | Success bg |
| success-100 | #D1FADF | Success badge bg |
| success-200 | #A6F4C5 | Highlight |
| success-300 | #6CE9A6 | Success border |
| success-400 | #32D583 | Success icon |
| success-500 | #12B76A | Active pill, indicator |
| success-600 | #039855 | Success text |
| success-700 | #027A48 | Dark success text |
| success-800 | #05603A | Heading on success bg |
| success-900 | #054F31 | Darkest success |

### Blue (Secondary — Charts/Info)

Used for: chart lines (light mode), info badges, annotation labels, link breadcrumbs

| Token | Hex | Usage |
|---|---|---|
| blue-50 | #EFF8FF | Info badge bg |
| blue-100 | #D1E9FF | Chart area fill (light) |
| blue-300 | #84CAFF | Icon tint |
| blue-500 | #2E90FA | Chart line (light mode), link |
| blue-600 | #1570EF | Primary info element, "New Chat" button (Ant theme) |
| blue-700 | #175CD3 | Annotation label |

### Blue Gray (Secondary — Dark Surfaces)

Used for: dark mode backgrounds, spacer indicators, muted labels

| Token | Hex | Usage |
|---|---|---|
| bluegray-100 | #EAECF5 | Borders |
| bluegray-200 | #D5D9EB | Spacer/divider indicators |
| bluegray-500 | #4E5BA6 | Text labels |
| bluegray-700 | #363F72 | Dark text |
| bluegray-900 | #101323 | Display text, dark bg |

### Purple (Secondary Accent)

Used for: category tags, data visualization accent, accent interactive

| Token | Hex |
|---|---|
| purple-500 | #7A5AF8 |
| purple-600 | #6938EF |
| purple-700 | #5925DC |

---

## Typography

### Font Families

| Role | Family | Fallback |
|---|---|---|
| UI / Body | Inter | system-ui, sans-serif |
| Brand / Display | Unilever Desire | serif |
| Code / Monospace | Consolas | JetBrains Mono, Monaco, monospace |

### Type Scale

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| display-2xl | 72px | 700 | 90px | -2% | Hero headings |
| display-xl | 60px | 700 | 72px | -2% | Section headings |
| display-lg | 48px | 700 | 60px | -2% | Page titles |
| display-md | 36px | 600 | 44px | -2% | Subsection titles |
| display-sm | 30px | 600 | 38px | 0 | Card/widget titles |
| display-xs | 24px | 600 | 32px | 0 | Panel headings, section labels |
| text-xl | 20px | 400 or 600 | 30px | 0 | Large body text |
| text-lg | 18px | 400 or 600 | 28px | 0 | Descriptions, supporting text |
| text-md | 16px | 400 or 600 | 24px | 0 | Default body text |
| text-sm | 14px | 400 or 600 | 20px | 0 | Table cells, form labels, buttons |
| text-xs | 12px | 400 or 600 | 18px | 0 | Captions, timestamps, footnotes |

### Font Weights

| Weight | Value | Usage |
|---|---|---|
| Regular | 400 | Body text, descriptions, placeholders |
| Medium | 500 | Labels, sidebar items, menu items |
| Semibold | 600 | Headings, button labels, bold labels |
| Bold | 700 | Display headings, stat values |

---

## Spacing

Base unit: 16px = 1rem. All spacing is a multiple of 4px.

| Token | Rem | Pixels | Common Usage |
|---|---|---|---|
| sp-1 | 0.25rem | 4px | Inline icon gap, tight padding |
| sp-2 | 0.5rem | 8px | Compact element gap, icon-to-text in sidebar |
| sp-3 | 0.75rem | 12px | Button padding-x, badge padding, sidebar item padding |
| sp-4 | 1rem | 16px | Default internal padding, card gap, form field gap |
| sp-5 | 1.25rem | 20px | Medium padding, topnav horizontal padding |
| sp-6 | 1.5rem | 24px | Default card padding, chat message padding, section gap |
| sp-8 | 2rem | 32px | Large internal spacing |
| sp-10 | 2.5rem | 40px | Widget/section separation |
| sp-12 | 3rem | 48px | Panel section breaks |
| sp-16 | 4rem | 64px | Major section dividers |

---

## Border Radius

| Token | Value | Usage |
|---|---|---|
| radius-sm | 6px | Small elements, tags, inline badges |
| radius-md | 8px | Buttons, inputs, cards, sidebar items, avatars (square) |
| radius-lg | 12px | Large cards, modals, chart containers |
| radius-xl | 16px | Hero cards, prominent panels |
| radius-full | 9999px | Circular avatars, pills, round badges |

---

## Shadows

| Token | Value | Usage |
|---|---|---|
| shadow-xs | 0px 1px 2px rgba(16,24,40, 0.05) | Subtle elevation, secondary buttons |
| shadow-sm | 0px 1px 3px rgba(16,24,40, 0.1), 0px 1px 2px rgba(16,24,40, 0.06) | Cards, dropdowns, topnav |
| shadow-md | 0px 4px 8px -2px rgba(16,24,40, 0.1), 0px 2px 4px -2px rgba(16,24,40, 0.06) | Elevated cards, popovers |
| shadow-lg | 0px 12px 16px -4px rgba(16,24,40, 0.08), 0px 4px 6px -2px rgba(16,24,40, 0.03) | Modals, large overlays |
| shadow-xl | 0px 20px 24px -4px rgba(16,24,40, 0.08), 0px 8px 8px -4px rgba(16,24,40, 0.03) | Full-screen modals |

---

## Borders

| Context | Width | Color (Light) | Color (Dark) |
|---|---|---|---|
| Default | 1px solid | gray-200 (#E4E7EC) | rgba(255,255,255, 0.1) |
| Input default | 1px solid | gray-300 (#D0D5DD) | rgba(255,255,255, 0.16) |
| Input focused | 1px solid | brand-300 (#D6BBFB) | brand-600 (#7F56D9) |
| Input error | 1px solid | error-300 (#FDA29B) | error-400 (#F97066) |
| Divider | 1px solid | gray-200 (#E4E7EC) | rgba(255,255,255, 0.06) |
| Card border | 1px solid | gray-200 (#E4E7EC) | rgba(255,255,255, 0.1) |
| Tool call border | 2px solid | varies by status | varies by status |

---

## Focus Rings

When an interactive element receives keyboard focus:

- **Ring width:** 4px
- **Ring color (brand):** brand-100 (#F4EBFF) at 100% opacity
- **Ring color (error):** error-100 (#FEE4E2) at 100% opacity
- **Ring offset:** 0px (flush with element border)
- **Border change:** border color changes to brand-300 (#D6BBFB) or error-300 (#FDA29B)
