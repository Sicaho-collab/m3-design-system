# M3 Design System

This is the M3 Design System (`m3-design-system`), a Material 3 React component library built on Radix UI primitives with Tailwind CSS v4 design tokens.

## Package

```bash
npm install m3-design-system
```

Import the design tokens CSS in your app entry point:

```css
@import "m3-design-system/styles";
```

Import components:

```tsx
import { Button, Card, TextField } from "m3-design-system";
```

## Reading Order

1. **Start here** for an overview of the system.
2. Read `overview-components.md` for a full list of available components and when to use each.
3. Read `design-tokens/colors.md` for color token usage.
4. Read `design-tokens/typography.md` for typography and spacing tokens.
5. When using a specific component, read its file in `components/` (e.g., `components/button.md`).

## General Rules

- Do not use raw hex colors. Always use M3 design tokens (e.g., `bg-m3-primary`, `text-m3-on-surface`).
- Do not hardcode border-radius values. Use M3 shape tokens (e.g., `rounded-m3-md`, `rounded-m3-full`).
- Do not hardcode shadow values. Use M3 elevation tokens (e.g., `shadow-m3-1` through `shadow-m3-5`).
- Use the `cn()` utility from `m3-design-system` to merge Tailwind classes when extending components.
- All components support `className` for custom styling and `ref` forwarding.
- Components use the `variant` prop pattern for visual variants (e.g., `filled`, `outlined`, `elevated`, `tonal`, `text`).
- Components use the `size` prop for sizing (e.g., `sm`, `md`, `lg`).
