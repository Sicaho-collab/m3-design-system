# RadioGroup

Single selection from a group of options.

## Import

```tsx
import { RadioGroup, RadioGroupItem } from "m3-design-system";
```

## Usage

```tsx
<RadioGroup value={selected} onValueChange={setSelected}>
  <div className="flex items-center gap-2">
    <RadioGroupItem value="option1" id="option1" />
    <label htmlFor="option1">Option 1</label>
  </div>
  <div className="flex items-center gap-2">
    <RadioGroupItem value="option2" id="option2" />
    <label htmlFor="option2">Option 2</label>
  </div>
</RadioGroup>
```

## Rules

- Always pair each `RadioGroupItem` with a visible `<label>`.
- Use RadioGroup when the user must pick exactly one option from 2-5 choices.
- For more than 5 options, consider a Select/Dropdown instead.
