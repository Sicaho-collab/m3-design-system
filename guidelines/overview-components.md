# Components Overview

All components are exported from `m3-design-system`. Import them directly:

```tsx
import { Button, Card, TextField } from "m3-design-system";
```

## Available Components

| Component | Purpose | Variants | Guidelines |
|-----------|---------|----------|------------|
| Button | Primary actions and interactions | filled, outlined, text, elevated, tonal | components/button.md |
| Card | Content containers | elevated, filled, outlined | components/card.md |
| TextField | Text input with floating labels | filled, outlined | components/text-field.md |
| Chip | Compact elements for filters, input, actions | assist, filter, input, suggestion | components/chip.md |
| Dialog | Modal overlays for focused tasks | — | components/dialog.md |
| FAB | Floating action button for primary screen action | surface, primary, secondary, tertiary | components/fab.md |
| Badge | Notification indicators | small, large | components/badge.md |
| Tabs | Content organization into tab panels | — | components/tabs.md |
| Checkbox | Boolean selection | — | components/checkbox.md |
| RadioGroup | Single selection from a set | — | components/radio-group.md |
| Switch | Toggle on/off states | — | components/switch.md |
| Slider | Value selection from a range | — | components/slider.md |
| Progress | Loading/completion indicators | linear, circular | components/progress.md |
| Snackbar | Brief messages at screen bottom | — | components/snackbar.md |
| Tooltip | Informational text on hover | — | components/tooltip.md |

## Component Selection Guide

- **User needs to trigger an action** → Use `Button`. Choose `filled` for primary, `outlined` for secondary, `text` for low-emphasis.
- **User needs to enter text** → Use `TextField`. Choose `filled` for most forms, `outlined` for dense layouts.
- **Content needs a container** → Use `Card`. Choose `elevated` for primary content, `outlined` for secondary, `filled` for supporting.
- **Binary on/off toggle** → Use `Switch` for immediate effect settings, `Checkbox` for form submissions.
- **Select one from a group** → Use `RadioGroup`.
- **Filter or tag content** → Use `Chip` with `filter` variant for toggleable filters, `input` variant for removable entries.
- **Primary screen-level action** → Use `FAB`.
- **Show notification count** → Use `Badge`.
- **Brief feedback message** → Use `Snackbar`.
- **Organize content sections** → Use `Tabs`.
- **Show progress** → Use `Progress` with `linear` for page-level, `circular` for inline.
- **Supplementary info on hover** → Use `Tooltip`.
- **Focused task or confirmation** → Use `Dialog`.

## Common Patterns

All components accept `className` for extending styles and forward `ref` to the underlying DOM element.

Use the `cn()` utility for class merging:

```tsx
import { Button, cn } from "m3-design-system";

<Button className={cn("w-full", isActive && "opacity-50")} />
```
