# Switch

Toggle control for on/off states with immediate effect.

## Import

```tsx
import { Switch } from "m3-design-system";
```

## Props

Extends Radix UI Switch props:

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| checked | `boolean` | — | On/off state |
| onCheckedChange | `(checked: boolean) => void` | — | Change handler |
| disabled | `boolean` | `false` | Disabled state |

## Usage

```tsx
<div className="flex items-center gap-3">
  <Switch id="notifications" checked={enabled} onCheckedChange={setEnabled} />
  <label htmlFor="notifications">Enable notifications</label>
</div>
```

## Rules

- Use Switch for settings that take effect immediately (e.g., dark mode, notifications).
- Use Checkbox instead when the change requires a form submission to apply.
- Always pair with a visible label.
