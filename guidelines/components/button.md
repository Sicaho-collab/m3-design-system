# Button

Primary action component for triggering interactions.

## Import

```tsx
import { Button } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"filled" \| "outlined" \| "text" \| "elevated" \| "tonal"` | `"filled"` | Visual style |
| size | `"sm" \| "md" \| "lg" \| "icon"` | `"md"` | Button size |
| asChild | `boolean` | `false` | Render as child element (for links) |
| disabled | `boolean` | `false` | Disabled state |
| className | `string` | — | Additional classes |

## Variant Selection

- **filled** — Primary actions. High emphasis. Use once per screen section.
- **outlined** — Secondary actions. Medium emphasis. Use alongside filled buttons.
- **text** — Low-emphasis actions. Tertiary actions, cancel buttons.
- **elevated** — Mid-emphasis on flat surfaces. Use when filled is too strong and outlined too subtle.
- **tonal** — Secondary emphasis with color. Use for actions that need more prominence than outlined.

## Usage

```tsx
<Button variant="filled">Save</Button>
<Button variant="outlined">Cancel</Button>
<Button variant="text">Learn more</Button>
<Button size="icon"><PlusIcon /></Button>
```

## As Link

```tsx
<Button asChild variant="text">
  <a href="/settings">Settings</a>
</Button>
```

## Rules

- Do not use more than one `filled` button per section.
- Pair `filled` with `outlined` or `text` for action groups.
- Use `icon` size only when the button contains a single icon with no text.
