# FAB (Floating Action Button)

The primary action button for a screen, typically floating in the bottom-right corner.

## Import

```tsx
import { FAB } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"surface" \| "primary" \| "secondary" \| "tertiary"` | `"primary"` | Color scheme |
| size | `"sm" \| "md" \| "lg" \| "extended"` | `"md"` | FAB size |
| icon | `ReactNode` | — | Icon element |

## Usage

```tsx
<FAB icon={<PlusIcon />} />
<FAB size="extended" icon={<EditIcon />}>Compose</FAB>
<FAB variant="tertiary" size="sm" icon={<FilterIcon />} />
```

## Size Selection

- **sm** (40px) — Secondary actions, compact layouts.
- **md** (56px) — Standard primary action.
- **lg** (96px) — Emphasized primary action.
- **extended** — FAB with text label. Use when the icon alone is not clear.

## Rules

- Use only one FAB per screen.
- Position with `fixed bottom-4 right-4` or similar.
- Always provide an `icon`. Extended FABs should also have a text label.
- Use `primary` variant by default. Use `surface` for less emphasis.
