# 02 — Layout Shell

> The top-level container that wraps every page in the AI agent interface. All templates share this structure.

---

## Structure

The app is a **horizontal flex container** that fills the full viewport height. It has exactly two children: the sidebar and the main content area.

```
┌─────────────────────────────────────────────────┐
│ APP (flex row, 100vh)                            │
│ ┌──────────┬───────────────────────────────────┐ │
│ │ SIDEBAR  │  MAIN                             │ │
│ │ 224px    │  flex: 1                          │ │
│ │ fixed    │  ┌─────────────────────────────┐  │ │
│ │ width    │  │ TOP NAV (56px, fixed)       │  │ │
│ │          │  ├─────────────────────────────┤  │ │
│ │          │  │ BREADCRUMB (42px, optional) │  │ │
│ │          │  ├─────────────────────────────┤  │ │
│ │          │  │ CONTENT AREA (flex: 1,      │  │ │
│ │          │  │ overflow-y: auto)           │  │ │
│ │          │  ├─────────────────────────────┤  │ │
│ │          │  │ CHAT INPUT (fixed bottom)   │  │ │
│ │          │  └─────────────────────────────┘  │ │
│ └──────────┴───────────────────────────────────┘ │
└─────────────────────────────────────────────────┘
```

## App Container

- **Display:** flex, direction row
- **Height:** 100vh (fill viewport)
- **Overflow:** hidden (children manage their own scroll)
- **Background:** white (light) / #09090B (dark)

## Sidebar

- **Width:** 224px, fixed (does not flex)
- **Height:** 100% of app container
- **Background:** #001529 (dark navy, same in light and dark mode)
- **Border right:** 1px solid rgba(255,255,255, 0.1)
- **Display:** flex column
- **Children:** header → chat list (flex:1, scrollable) → footer
- See `03-sidebar.md` for full spec

## Main Content Area

- **Width:** flex: 1 (fills remaining space)
- **Height:** 100% of app container
- **Display:** flex column
- **Background:** white (light) / #111116 (dark)
- **Children:** top nav → breadcrumb (optional) → content area (flex:1, scrollable) → chat input bar (fixed)

## Responsive Notes

- At viewport widths below 768px, the sidebar should collapse to an icon-only state (40px wide) or be hidden behind a hamburger toggle
- The main content area always fills the remaining width
- The chat input bar is always pinned to the bottom of the main area, never scrolls with content
