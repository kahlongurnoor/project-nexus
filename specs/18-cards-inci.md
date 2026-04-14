# 18 — Cards: INCI / Product Info

> Ingredient and safety statement cards for the Product Information / INCI Agent template. Used in Unilever's regulatory workflows.

---

## Card Container

- **Background:** white
- **Border:** 1px solid gray-200
- **Border radius:** 12px
- **Padding:** 24px (sp-6)

## Target Location Header

- **Display:** flex row, align-items center, gap 8px
- **Margin bottom:** 16px
- **Icon:** Globe, 20×20px, color gray-400
- **Label:** "Target Location/Language:" — 14px, weight 400, color gray-500
- **Value:** "INCI:Canada/ English_CA" — 14px, weight 700, color gray-900

## Ingredient List Section

### Section Title

- **Font:** 16px, weight 600, color gray-900
- **Icon prefix:** list icon (≡), inline before text
- **Margin bottom:** 8px

### Ingredient Text Block

- **Background:** gray-50 (#F9FAFB)
- **Border:** 1px solid gray-200
- **Border radius:** 8px
- **Padding:** 16px
- **Font:** 14px, weight 400, color gray-700
- **Line height:** 1.6
- **Content:** full ingredient list, comma-separated

## Ingredient Statements Section

### Section Title

- **Font:** 16px, weight 600, color gray-900
- **Icon prefix:** clipboard icon (📋), inline before text
- **Margin bottom:** 8px

### Table

- **Width:** 100%
- **Border:** 1px solid gray-200
- **Border radius:** 8px
- **Overflow:** hidden (for rounded corners)

#### Table Header Row

- **Background:** gray-100 (#F2F4F7)
- **Padding:** 8px 16px per cell
- **Font:** 12px, weight 600, color gray-700
- **Columns:** "Purpose" (left), "Statement" (right, wider)

#### Table Body Row

- **Background:** white
- **Border top:** 1px solid gray-200
- **Padding:** 12px 16px per cell
- **Font:** 14px, weight 400, color gray-700

#### Safety Warning Formatting

- **Purpose cell:** text in error-600 (#D92D20), weight 500, with ⚠ triangle icon
- **Statement cell:** "CAUTION:" in error-700 (#B42318), weight 700. Remaining text in gray-700, weight 400.
