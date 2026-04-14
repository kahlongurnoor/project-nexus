# 09 — Stat Cards

> Metric display cards used in dashboard rows, typically 3-5 per row.

---

## Card

- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-200 (light) / rgba(255,255,255, 0.1) (dark)
- **Border radius:** 12px (radius-lg)
- **Padding:** 24px (sp-6)
- **Shadow:** shadow-xs
- **Min width:** 160px

## Layout

- **Display:** flex column

### Header Row

- **Display:** flex row, justify-content space-between, align-items center
- **Margin bottom:** 8px

#### Label

- **Font:** 14px (text-sm), weight 500, color gray-500

#### Info Icon

- **Size:** 16×16px, color gray-400
- **Purpose:** tooltip trigger (optional)

### Value

- **Font:** 30px, weight 600, color gray-900 (light) / #F4F4F5 (dark)
- **Letter spacing:** -0.5px

## Grid Usage

When showing multiple stat cards, use a horizontal grid:

- **Display:** grid
- **Columns:** repeat(3, 1fr) for 3 cards, repeat(5, 1fr) for 5 cards
- **Gap:** 24px (sp-6) between cards

## Example Data

| Label | Value |
|---|---|
| Total Conversations | 48 |
| Total Time | 288 |
| Correlation Rate | 3.9M |
| Total Cost | $4.43 |
| Avg. Latency | 11.58s |
| Error Rate | 0.0% |
