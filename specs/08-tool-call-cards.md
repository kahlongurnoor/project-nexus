# 08 — Tool Call Cards

> Status indicators for agent tool execution. Appear in the chat thread below analytics or AI responses. Three states: success, processing, error.

---

## Section Label

- **Display:** flex row, align-items center, gap 8px
- **Left margin:** 48px (aligns with message body)
- **Margin bottom:** 14px
- **Icon:** Terminal, 14-15px, color gray-700 (light) / #71717A (dark)
- **Text:** "Tool Calls" — 12-13px, weight 600, color gray-900 (light) / #F4F4F5 (dark)

## Card (shared structure)

- **Display:** flex row, align-items center, gap 12px
- **Padding:** 14px 16px
- **Border radius:** 8px (light) / 12px (dark)
- **Border width:** 2px (light) / 1.5px (dark)
- **Border style:** solid
- **Margin bottom:** 10px between cards
- **Shadow:** 0 1px 3px rgba(0,0,0, 0.1), 0 1px 2px -1px rgba(0,0,0, 0.1)
- **Hover (dark mode):** translateX(2px) shift right

### Tool Icon (left)

- **Size:** 34×34px (36×36px dark)
- **Border radius:** 8px
- **Background:** white (light) / #1F1F27 (dark)
- **Border:** 1px solid gray-300 (light) / rgba(255,255,255, 0.16) (dark)
- **Inner icon:** 14-15px, color gray-700 (light) / #71717A (dark)
- **Icon per tool:** Database icon for search_database, Code brackets for execute_code, Globe for api_request

### Tool Info (center)

- **Flex:** 1
- **Name:** 12-13px, weight 700, font-family Consolas/JetBrains Mono (monospace), color gray-900 (light) / #F4F4F5 (dark)
- **Sub-label (processing only):** 10-11px, weight 500, color gray-400 (light) / #52525B (dark), margin-top 2px

### Status Icon (right)

- **Size:** 14-16px

## Status Variants

### Success

- **Background:** rgba(82,196,26, 0.05) in light / rgba(52,211,153, 0.12) in dark
- **Border color:** rgba(82,196,26, 0.3) in light / rgba(52,211,153, 0.25) in dark
- **Status icon:** Checkmark, color #52c41a (light) / #34D399 (dark)
- **Sub-label:** none (just the tool name)

### Processing

- **Background:** rgba(230,244,255, 0.3) in light / rgba(182,146,246, 0.10) in dark
- **Border color:** rgba(22,119,255, 0.3) in light / rgba(182,146,246, 0.25) in dark
- **Status icon:** Loader/spinner, color blue-600 (light) / brand-400 (#B692F6) (dark), animated rotate 360deg over 1s linear infinite
- **Sub-label:** "Processing..." in gray-400

### Error

- **Background:** rgba(255,77,79, 0.05) in light / rgba(248,113,113, 0.10) in dark
- **Border color:** rgba(255,77,79, 0.3) in light / rgba(248,113,113, 0.25) in dark
- **Status icon:** X mark, color #ff4d4f (light) / #F87171 (dark)
- **Sub-label:** none

## Example Tool Names

- `search_database`
- `execute_code`
- `api_request`
- `fetch_data`
- `generate_report`
