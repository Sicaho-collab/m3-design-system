# Tooltip

Informational text shown on hover or focus.

## Import

```tsx
import { Tooltip, TooltipTrigger, TooltipContent, TooltipProvider } from "m3-design-system";
```

## Usage

Wrap your app (or a section) with `TooltipProvider`:

```tsx
<TooltipProvider>
  <Tooltip>
    <TooltipTrigger asChild>
      <Button size="icon"><InfoIcon /></Button>
    </TooltipTrigger>
    <TooltipContent>More information</TooltipContent>
  </Tooltip>
</TooltipProvider>
```

## Rules

- Always wrap tooltip usage in a `TooltipProvider` (once at app root is sufficient).
- Use for supplementary info only. Do not put critical information in tooltips.
- Keep tooltip text short (under 40 characters).
- Do not put interactive elements inside tooltips.
- Use `asChild` on `TooltipTrigger` to pass trigger behavior to your own element.
