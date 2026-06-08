---
name: ui-design-system
description: Reusable UI design-system workflow for Codex-built software. Use when designing or implementing polished product UI, choosing a visual style, creating frontend pages/components, turning an agreed style such as Apple-like, Modern SaaS, Enterprise Admin, Chinese Classical, Editorial, Luxury, Brutalist, Data/Finance, Health, or Industrial Console into concrete tokens, components, layouts, states, and screenshot acceptance criteria.
---

# UI Design System

Use this skill to turn an agreed visual style into buildable frontend decisions. The goal is to prevent generic UI output by making Codex select a style, load the right rules, implement with reusable tokens, and verify the result visually.

## Workflow

1. Confirm the product context: target user, platform, primary task, information density, and chosen style.
2. If the style is unclear, propose 2-3 suitable styles from `references/style-taxonomy.md` and ask the user to pick one.
3. Load only the relevant reference files:
   - Use `references/style-taxonomy.md` for style selection and style-specific rules.
   - Use `references/component-spec.md` before implementing components, forms, tables, dialogs, navigation, or stateful UI.
   - Use `references/codex-prompts.md` when the user wants reusable prompts for future Codex sessions.
4. Implement the UI with explicit tokens for color, typography, spacing, radius, shadow, border, and motion.
5. Include expected states: hover, active, focus-visible, disabled, loading, empty, and error where relevant.
6. Verify desktop and mobile screenshots. Fix text overflow, layout overlap, blank canvases, weak contrast, and generic template aesthetics.

## Style Discipline

Choose one clear aesthetic direction per screen. Do not mix unrelated styles unless the product intentionally requires a hybrid system.

Prefer:
- Concrete product UI over marketing hero pages.
- Real workflow surfaces over decorative mockups.
- Stable component dimensions over layout shifts.
- Style-specific typography and spacing over default component-library output.

Avoid:
- Generic purple/blue gradient SaaS pages.
- Nested cards and decorative cards for whole page sections.
- Unexplained bokeh/orb backgrounds.
- Oversized hero typography inside dense tools.
- Components without focus, empty, loading, and error states.

## Component Strategy

For React/Tailwind projects, prefer a source-owned pattern inspired by shadcn/ui: compose accessible primitives, expose tokens through CSS variables, and keep components editable in the project.

For complex interactions, prefer proven primitives such as Radix UI or Headless UI rather than hand-rolling behavior. Style the primitive with the selected visual system.

For enterprise/data-heavy UI, optimize scanability: dense tables, clear filters, consistent status colors, tabular numbers, and predictable navigation.

For expressive styles such as Chinese Classical, Editorial, Luxury, or Neo Brutalism, keep functionality complete while letting typography, spacing, borders, and color carry the character.

## Bundled Assets

Use `assets/tokens/ui-tokens.css` as a small CSS token baseline for static HTML prototypes or as a naming reference for app tokens.

Use `assets/html-examples/` for static examples:
- `index.html`: demo gallery
- `modern-saas.html`: AI/developer tool dashboard
- `apple-productivity.html`: personal productivity workspace
- `chinese-classical.html`: classical Chinese content product
- `admin-console.html`: enterprise admin console

Copy these examples only as starting points. Adapt layout, content, and tokens to the actual product instead of reusing them unchanged.

## Acceptance Checklist

Before finishing, ensure:

- The first viewport shows the actual product experience.
- The chosen style is recognizable without relying on labels.
- Main task, primary action, and navigation are obvious.
- Text fits at desktop and mobile widths.
- Interactive states are visible and accessible.
- Empty/loading/error states exist for dynamic surfaces.
- The UI does not look like an unmodified component-library default.
