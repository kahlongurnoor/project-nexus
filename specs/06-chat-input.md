# 06 — Chat Input

> The bottom input bar pinned to the bottom of the main content area. Always visible, never scrolls.

---

## Container

- **Border top:** 1px solid gray-200 (light) / rgba(255,255,255, 0.1) (dark)
- **Padding:** 16px 20px (light) / 16px 24px (dark)
- **Background:** white (light) / #0C0C10 (dark)
- **Shadow:** 0 -1px 3px rgba(0,0,0, 0.05)
- **Flex shrink:** 0 (never collapse)

## Inner Wrapper

- **Max width:** 780px
- **Margin:** 0 auto (centered)

## Input Row

- **Display:** flex row, align-items flex-end, gap 8px

### Attach Button (left)

- **Size:** 38×38px (40×40px dark)
- **Border radius:** 8px
- **Background:** transparent
- **Hover:** gray-100 (light) / #27272F (dark)
- **Icon:** Paperclip, 18×18px, color gray-400 (light) / #52525B (dark)

### Textarea

- **Flex:** 1
- **Min height:** 48px
- **Max height:** 160px (grows with content, capped)
- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-300 (light) / rgba(255,255,255, 0.1) (dark)
- **Border radius:** 8px (light) / 12px (dark)
- **Padding:** 12px 14px (light) / 13px 16px (dark)
- **Font:** 14px, weight 400, color gray-900 (light) / #F4F4F5 (dark)
- **Placeholder:** "Ask about analytics, insights, or request data visualizations..." in gray-400 (light) / #52525B (dark)
- **Resize:** none (auto-grows via JavaScript)
- **Focus border:** brand-600 (#7F56D9)
- **Focus ring:** 0 0 0 3px rgba(127,86,217, 0.15)

### Mic Button

- **Identical to Attach Button** but with Microphone icon

### Send Button

- **Size:** 38×38px (40×40px dark)
- **Border radius:** 8px
- **Background:** blue-600 (#1570EF) for Ant theme, brand-600 (#7F56D9) for brand theme
- **Shadow:** shadow-sm
- **Icon:** Send/paper-plane, 18×18px, color white
- **Default state:** opacity 0.5 (disabled appearance when textarea is empty)
- **Active state (text entered):** opacity 1, add glow shadow in dark mode
- **Hover (active):** background lightens one shade, slight translateY(-1px) lift

## Footer Row

- **Display:** flex row, justify-content space-between
- **Margin top:** 8px
- **Padding:** 0 4px

### Left Hint

- **Font:** 10px, weight 400, color gray-400 (light) / #52525B (dark)
- **Text:** "Press Enter to send, Shift+Enter for new line"

### Right Counter

- **Font:** 10px, weight 500, color gray-400 (light) / #52525B (dark)
- **Text:** "0 characters" (updates dynamically)

## Behavior

- **Auto-resize:** textarea height grows as user types, up to max-height (160px), then scrolls internally
- **Enter key:** submits the message (clears input, resets height)
- **Shift+Enter:** inserts a newline
- **Send button:** only fully opaque and clickable when textarea has content
