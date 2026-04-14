# 03 — Sidebar

> The left navigation panel present on every screen. Always dark navy regardless of light/dark mode.

---

## Container

- **Width:** 224px
- **Background:** #001529
- **Border right:** 1px solid rgba(255,255,255, 0.1)
- **Display:** flex column
- **Font family:** Inter
- **Overflow:** hidden (the chat list child scrolls)

## Sections (top to bottom)

### 1. Header — "New Chat" Button

- **Padding:** 14px all sides
- **Button width:** 100% of sidebar minus padding (196px)
- **Button height:** 36px
- **Button background:** #1677FF (blue-600) for Ant theme variant, or brand-600 (#7F56D9) for brand variant
- **Button border-radius:** 8px (radius-md)
- **Button text:** "New Chat" — font size 12px, weight 600, color white
- **Button icon:** Plus icon (14×14px), white, positioned left of text with 7px gap
- **Button shadow:** shadow-sm
- **Hover state:** background lightens one shade, shadow increases slightly

### 2. Chat List (scrollable)

- **Padding:** 0 horizontal, 8px left/right for items
- **Overflow-y:** auto (scrollable when list exceeds space)
- **Flex:** 1 (takes all available vertical space between header and footer)

#### Section Label

- **Padding:** 8px horizontal, 10px top, 7px bottom
- **Text:** "Recent Chats" or "Recent"
- **Font:** 10px, weight 500, color rgba(255,255,255, 0.51)

#### Chat Item

- **Padding:** 10px horizontal, 10px vertical
- **Border radius:** 8px (radius-md)
- **Display:** flex row, gap 10px
- **Cursor:** pointer
- **Hover background:** rgba(255,255,255, 0.06)

##### Chat Item Icon

- **Size:** 14×14px
- **Type:** MessageSquare outline icon
- **Color:** rgba(255,255,255, 0.51)
- **Margin top:** 2px (align with first line of text)

##### Chat Item Text

- **Title:** font size 12px, weight 500, color rgba(255,255,255, 0.85)
- **Overflow:** hidden, text-overflow ellipsis, white-space nowrap
- **Time:** font size 10px, weight 400, color rgba(255,255,255, 0.51), margin-top 2px

### 3. Footer

- **Border top:** 1px solid rgba(255,255,255, 0.1)
- **Padding:** 12px top, 10px horizontal
- **Display:** flex column, gap 4px

#### Footer Button

- **Display:** flex row, gap 10px, align-items center
- **Padding:** 8px vertical, 12px horizontal
- **Border radius:** 8px (radius-md)
- **Background:** transparent
- **Hover background:** rgba(255,255,255, 0.06)
- **Icon:** 14×14px, color rgba(255,255,255, 0.85)
- **Text:** 12px, weight 500, color rgba(255,255,255, 0.85)

#### Footer Buttons (in order)

1. **Light Mode / Dark Mode** — Sun or Moon icon + label
2. **Settings** — Settings gear icon + "Settings" label
