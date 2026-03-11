# Checkbox

Boolean or indeterminate selection control for forms.

## Import

```tsx
import { Checkbox } from "m3-design-system";
```

## Props

Extends Radix UI Checkbox props:

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| checked | `boolean \| "indeterminate"` | — | Checked state |
| onCheckedChange | `(checked: boolean \| "indeterminate") => void` | — | Change handler |
| disabled | `boolean` | `false` | Disabled state |

## Usage

```tsx
<div className="flex items-center gap-2">
  <Checkbox id="terms" checked={agreed} onCheckedChange={setAgreed} />
  <label htmlFor="terms">I agree to the terms</label>
</div>
```

## Rules

- Always pair with a visible `<label>`.
- Use `indeterminate` state for "select all" when only some children are selected.
- Use Checkbox for multi-select in forms. Use Switch for immediate-effect toggles.
