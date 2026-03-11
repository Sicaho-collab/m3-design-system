# Progress

Loading and completion indicator in linear or circular form.

## Import

```tsx
import { Progress } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| value | `number` | `0` | Progress percentage (0-100) |
| variant | `"linear" \| "circular"` | `"linear"` | Display style |
| indeterminate | `boolean` | `false` | Unknown duration loading state |

## Usage

```tsx
{/* Determinate linear */}
<Progress value={75} />

{/* Indeterminate linear */}
<Progress indeterminate />

{/* Circular */}
<Progress variant="circular" value={50} />
<Progress variant="circular" indeterminate />
```

## Rules

- Use `linear` for page-level or section-level loading.
- Use `circular` for inline/component-level loading (e.g., inside a button).
- Use `indeterminate` when the duration is unknown.
- Set `value` as a number from 0-100 for determinate progress.
