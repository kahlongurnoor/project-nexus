# 04 — Top Navigation Bar

> The horizontal header bar at the top of the main content area. Contains the agent title, search, and user controls.

---

## Container

- **Height:** 56px (fixed, does not scroll)
- **Background:** white (light) / #0C0C10 (dark)
- **Border bottom:** 1px solid gray-200 (light) / rgba(255,255,255, 0.1) (dark)
- **Shadow:** shadow-xs
- **Padding:** 0 20px horizontal
- **Display:** flex row, align-items center, justify-content space-between

## Left Section

- **Display:** flex row, align-items center, gap 16px

### Agent Title

- **Font:** 16px, weight 700, color gray-900 (light) / #F4F4F5 (dark)
- **Text:** e.g. "AI Analytics Assistant"
- **Letter spacing:** -0.01em

### Search Box

- **Width:** 224px
- **Height:** 34px
- **Background:** white (light) / #18181E (dark)
- **Border:** 1px solid gray-300 (light) / rgba(255,255,255, 0.1) (dark)
- **Border radius:** 8px (radius-md)
- **Padding:** 7px 14px
- **Display:** flex row, align-items center, gap 8px
- **Focus state:** border-color changes to brand-600

#### Search Icon

- **Size:** 14×14px
- **Color:** gray-400 (light) / #52525B (dark)
- **Position:** left side of search box

#### Search Input

- **Font:** 12px, weight 400, color gray-700 (light) / #F4F4F5 (dark)
- **Placeholder:** "Search conversations..." in gray-400 (light) / #52525B (dark)
- **Background:** transparent
- **Border:** none
- **Outline:** none

## Right Section

- **Display:** flex row, align-items center, gap 4px

### Help Button (icon-only)

- **Size:** 36×36px
- **Border radius:** 8px
- **Background:** transparent
- **Hover background:** gray-100 (light) / #27272F (dark)
- **Icon:** HelpCircle, 18×18px, color gray-500 (light) / #71717A (dark)

### Notification Button (icon-only)

- **Size:** 36×36px
- **Border radius:** 8px
- **Background:** transparent
- **Hover background:** gray-100 (light) / #27272F (dark)
- **Icon:** Bell, 18×18px, color gray-500 (light) / #71717A (dark)
- **Notification dot:** 7px circle, background error-500 (#F04438), positioned top-right at 7px from top, 8px from right. In dark mode, add 2px border matching the topnav background to create visual separation.

### Divider

- **Width:** 1px
- **Height:** 20px
- **Background:** gray-200 (light) / rgba(255,255,255, 0.1) (dark)
- **Margin:** 0 8px horizontal

### User Profile Button

- **Display:** flex row, gap 10px, align-items center
- **Padding:** 6px 10px
- **Border radius:** 8px
- **Background:** transparent
- **Hover background:** gray-50 (light) / #27272F (dark)

#### User Avatar

- **Size:** 28×28px
- **Border radius:** 50% (circle)
- **Background:** blue-600 (#1570EF) for Ant theme, or linear-gradient(135deg, brand-600, brand-400) for brand theme
- **Icon inside:** User icon, 14×14px, color white

#### User Name

- **Font:** 12px, weight 500, color gray-900 (light) / #F4F4F5 (dark)
- **Text:** e.g. "John Doe"

#### Chevron Down

- **Size:** 14×14px
- **Color:** gray-400 (light) / #52525B (dark)
