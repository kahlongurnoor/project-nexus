# 16 — Cards: Proposed Plan

> Agent plan card with numbered action items and approve/reject CTAs. Used in the Nexus agent chat workflow when an AI agent proposes a multi-step plan for user approval.

---

## Card Container

- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-200
- **Border radius:** 12px
- **Shadow:** shadow-xs
- **Overflow:** hidden (footer border flush with card edge)

## Header

- **Padding:** 20px 24px
- **Display:** flex row, justify-content space-between, align-items center
- **Title:** "Proposed Plan" — 16px, weight 600, color gray-900
- **Version badge:** brand pill (see spec 11) — e.g. "Version 1"

## Body

- **Padding:** 0 24px 16px
- **Content:** ordered list (numbered 1, 2, 3...)
- **List font:** 14px, weight 400, color gray-700
- **List line-height:** 1.8 (generous spacing between items)
- **List left padding:** 20px (for number indentation)

## Footer

- **Padding:** 16px 24px
- **Border top:** 1px solid gray-200
- **Display:** flex row, justify-content flex-end, gap 12px
- **Left button:** secondary gray, label "Edit Plan", optional pencil icon
- **Right button:** primary, label "Approve Plan", optional checkmark icon

---

