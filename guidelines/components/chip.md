# Chip

Compact element for filters, input, and actions.

## Import

```tsx
import { Chip } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"assist" \| "filter" \| "input" \| "suggestion"` | `"assist"` | Chip type |
| selected | `boolean` | — | Selected state (filter variant) |
| onRemove | `() => void` | — | Remove callback (shows X icon) |
| icon | `ReactNode` | — | Leading icon |

## Variant Selection

- **assist** — Action shortcuts (e.g., "Add to calendar", "Share").
- **filter** — Toggleable filters. Use `selected` prop for active state.
- **input** — Removable entries (e.g., email recipients, tags). Shows X button.
- **suggestion** — Contextual suggestions (e.g., search suggestions).

## Usage

```tsx
<Chip variant="filter" selected={isActive} onClick={toggle}>
  Vegetarian
</Chip>

<Chip variant="input" onRemove={() => removeTag(tag)}>
  {tag}
</Chip>
```

## Rules

- Use `filter` chips in groups for multi-select filtering.
- Use `input` chips when users can add and remove items.
- Do not use chips for primary actions — use Button instead.
