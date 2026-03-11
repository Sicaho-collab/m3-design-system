# TextField

Text input with Material 3 floating label animation.

## Import

```tsx
import { TextField } from "m3-design-system";
```

## Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"filled" \| "outlined"` | `"filled"` | Visual style |
| label | `string` | — | Floating label text |
| supportingText | `string` | — | Helper text below the field |
| error | `boolean` | `false` | Error state |
| errorText | `string` | — | Error message (shown when `error` is true) |
| leadingIcon | `ReactNode` | — | Icon before input |
| trailingIcon | `ReactNode` | — | Icon after input |

Also accepts all standard `<input>` HTML attributes (`type`, `placeholder`, `value`, `onChange`, etc.).

## Usage

```tsx
<TextField label="Email" type="email" />
<TextField label="Search" leadingIcon={<SearchIcon />} />
<TextField
  label="Password"
  type="password"
  error={!!errors.password}
  errorText={errors.password}
/>
```

## Variant Selection

- **filled** — Default for most forms. Recognizable input affordance.
- **outlined** — Use in dense layouts or when multiple inputs are stacked.

## Rules

- Always provide a `label`. Do not use TextField without a label.
- Use `supportingText` for format hints (e.g., "Must be at least 8 characters").
- Use `errorText` with `error={true}` for validation messages. Do not use red text manually.
