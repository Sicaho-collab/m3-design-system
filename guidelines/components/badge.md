# Badge

Notification indicator for icons and navigation items.

## Import

```tsx
import { Badge } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"small" \| "large"` | `"large"` | Badge size |
| count | `number` | — | Notification count (large variant only) |

## Usage

```tsx
{/* Dot indicator */}
<Badge variant="small" />

{/* Count indicator */}
<Badge count={5} />
<Badge count={1200} />  {/* Renders as "999+" */}
```

## Rules

- Use `small` (dot) when presence matters more than count.
- Use `large` with `count` when the number matters.
- Counts over 999 display as "999+".
- Position badges absolutely relative to their parent icon/element.
