# Project Habibi — UI Specification Templates

> Machine-readable specs for building AI agent interfaces on Nexus. An agent reads **2 files max** to build any screen: the tokens file + the relevant template file.

## How to Use

1. **Always start with** `00-design-tokens.md` — every color, font, spacing, and dark mode mapping
2. **Then read the template** for the screen you're building:
   - `01-template-ai-chat-agent.md` — the core Nexus chat interface
   - `02-template-component-showcase.md` — the docs/demo page
   - `03-template-landing-page.md` — the marketing/hero page
   - `04-template-inci-agent.md` — the product info display
3. **If you need a reusable component** not covered in the template file, check `05-shared-components.md` — buttons, badges, form inputs, tabs, modals

## Files

| File | What It Covers |
|---|---|
| [00-design-tokens.md](specs/00-design-tokens.md) | All colors, typography, spacing, radius, shadows, borders, dark mode map |
| [01-template-ai-chat-agent.md](specs/01-template-ai-chat-agent.md) | Sidebar, topnav, chat messages, analytics cards, tool calls, chat input, stat cards, proposed plan, agents table, toasts |
| [02-template-component-showcase.md](specs/02-template-component-showcase.md) | 9-section demo page: chat cards, conversation, charts, action cards, tool calls, toasts |
| [03-template-landing-page.md](specs/03-template-landing-page.md) | Hero, feature grid, theme preview, CTA footer — no sidebar |
| [04-template-inci-agent.md](specs/04-template-inci-agent.md) | Ingredient list cards, safety statement tables |
| [05-shared-components.md](specs/05-shared-components.md) | Buttons (6 variants), badges, form inputs, checkbox, radio, tabs, modals, date picker, scrollbar |

## Source

| Detail | Value |
|---|---|
| Figma | [Design System 2.0](https://www.figma.com/design/qafioCr7GiesyZtf90byDh/Design-System-2.0?node-id=339-11336) |
| Fonts | Inter (UI), Unilever Desire (brand), Consolas (code) |
| Base Unit | 16px = 1rem |
