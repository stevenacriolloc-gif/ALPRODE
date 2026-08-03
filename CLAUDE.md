# Web Design Guidelines

Reference to follow when building or revising web pages in this project (e.g. `index.html`), when no other brand/design system is specified. Distilled from general UI/UX best practices.

## Design thinking (before coding)
- Define purpose (what problem, who uses it), tone (pick one clear direction: minimal, maximalist, retro-futuristic, editorial, brutalist, luxury, playful, glassmorphism, etc.), and the one detail that should make it memorable.
- Commit to a bold, cohesive direction rather than a safe middle ground — intentionality matters more than intensity.

## Typography
- Avoid generic fonts (Arial, Inter, Roboto, Fraunces are overused). Pair a distinctive display font with a refined body font.
- `text-wrap: balance` on headings, `text-wrap: pretty` on body text.

## Color & theme
- Define the palette as CSS custom properties (`:root { --… }`).
- A dominant color with a sharp accent beats many evenly-weighted colors.
- If a brand/design system already exists in the page, derive new colors from it (e.g. via `oklch()`) instead of inventing unrelated ones.
- Always set explicit `a` / `a:hover` colors — never leave links on browser-default blue.

## Layout
- Prefer `display: flex` / `grid` with `gap` for sibling groups (buttons, cards, nav items, stat tiles) instead of margins or whitespace-based spacing.
- Consider asymmetry, overlap, or generous negative space instead of defaulting to centered/safe layouts — match the chosen tone.
- Give backgrounds atmosphere/depth (texture, layered transparency, subtle shadow) rather than a flat solid fill, without tipping into the tropes below.

## Motion
- Prefer CSS-only animations. One well-orchestrated page-load with staggered reveals beats many scattered micro-interactions.

## Content discipline
- No filler: every element earns its place. An empty-feeling section is a layout problem, not a content gap.
- Less is more — avoid unnecessary stats/icons/numbers padding out a section.
- Ask before adding whole new sections or pages beyond what was requested.

## Avoid "AI slop" visual tropes
- Aggressive/default gradient backgrounds
- Emoji, unless explicitly part of the brand
- Rounded cards with a left-border accent stripe
- Overused fonts: Inter, Roboto, Arial, Fraunces
- Hand-drawn SVG illustrations in place of real images/placeholders

## Small, targeted edits
- When asked for a small change (some text, one color, one element), change only that — don't redesign or "improve" untouched parts. Suggest bigger improvements rather than applying them unprompted.

## Correctness basics
- Canonical HTML: close every non-void element, double-quote every attribute.
- Keep mobile tap targets ≥44px; keep body text at a legible size.

---
Distilled from general UI/UX principles found in a design-agent system prompt inside `system_prompts_leaks-main/Anthropic/claude-design.md` (an unverified leak). Used here only as generic design inspiration — not treated as literal tool instructions.
