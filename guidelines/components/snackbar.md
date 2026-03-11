# Snackbar

Brief feedback message displayed at the bottom of the screen.

## Import

```tsx
import { Snackbar } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| message | `string` | — | The message text (required) |
| action | `string` | — | Action button label |
| onAction | `() => void` | — | Action button callback |
| onDismiss | `() => void` | — | Dismiss callback (shows X button) |
| open | `boolean` | `true` | Visibility state |

## Usage

```tsx
<Snackbar
  message="Item deleted"
  action="Undo"
  onAction={handleUndo}
  onDismiss={() => setOpen(false)}
  open={isOpen}
/>
```

## Rules

- Keep messages short (1 line, under 60 characters).
- Use `action` for undo or retry operations.
- Auto-dismiss after 4-8 seconds (manage with `setTimeout` + `open` prop).
- Only show one snackbar at a time.
- Position at the bottom of the viewport with `fixed bottom-4 left-1/2 -translate-x-1/2`.
