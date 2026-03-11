# Slider

Value selection from a continuous or discrete range.

## Import

```tsx
import { Slider } from "m3-design-system";
```

## Props

Extends Radix UI Slider props:

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| value | `number[]` | — | Current value(s) |
| onValueChange | `(value: number[]) => void` | — | Change handler |
| min | `number` | `0` | Minimum value |
| max | `number` | `100` | Maximum value |
| step | `number` | `1` | Step increment |
| disabled | `boolean` | `false` | Disabled state |

## Usage

```tsx
<Slider value={[volume]} onValueChange={([v]) => setVolume(v)} max={100} step={1} />
```

## Rules

- Always show the current value near the slider (via label or adjacent text).
- Use `step` for discrete values.
- Value is always an array (supports range sliders).
