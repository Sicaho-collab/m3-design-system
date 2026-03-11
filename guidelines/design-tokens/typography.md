# Typography & Spacing Tokens

## Font Family

The system uses Roboto as the default sans-serif font:

```
font-family: 'Roboto', system-ui, -apple-system, sans-serif
```

This is set automatically via the `--font-sans` token when you import the design tokens CSS.

## Typography Scale

Use standard Tailwind text utilities. The design system does not define custom type scale tokens — use Tailwind's built-in classes:

| Usage | Class |
|-------|-------|
| Display/Hero text | `text-4xl` or `text-5xl` |
| Page headings | `text-2xl font-normal` |
| Section headings | `text-lg font-medium` |
| Body text | `text-base` or `text-sm` |
| Labels/Captions | `text-xs` |
| Supporting text | `text-sm text-m3-on-surface-variant` |

## Border Radius (Shape)

Do not use raw pixel values. Use M3 shape tokens:

| Token | Value | Usage |
|-------|-------|-------|
| `rounded-m3-none` | 0px | No rounding |
| `rounded-m3-xs` | 4px | Small chips, code blocks, input fields |
| `rounded-m3-sm` | 8px | Chips, small containers |
| `rounded-m3-md` | 12px | Cards, medium containers |
| `rounded-m3-lg` | 16px | FABs (medium), large containers |
| `rounded-m3-xl` | 28px | Dialogs, large FABs |
| `rounded-m3-full` | 9999px | Buttons, pills, circular elements |

## Spacing

Use M3 spacing tokens for consistent spacing:

| Token | Value | Usage |
|-------|-------|-------|
| `m3-1` | 4px | Tight gaps, icon padding |
| `m3-2` | 8px | Small gaps between related items |
| `m3-3` | 12px | Medium gaps |
| `m3-4` | 16px | Standard padding (cards, dialogs) |
| `m3-5` | 20px | Section spacing |
| `m3-6` | 24px | Large padding |
| `m3-8` | 32px | Section gaps |
| `m3-10` | 40px | Large section gaps |
| `m3-12` | 48px | Page-level spacing |
| `m3-16` | 64px | Maximum spacing |

Usage with Tailwind:

```tsx
<div className="p-m3-4 gap-m3-2">  // 16px padding, 8px gap
```

## Disabled State

All components use `opacity-38` (38% opacity) for disabled states. Do not change disabled styling — it is built into each component via the `disabled` prop.
