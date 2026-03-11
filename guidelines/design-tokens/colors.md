# Color Tokens

All colors use the `m3-` prefix and follow Material 3 color roles. Do not use raw hex values.

## Token Naming Pattern

```
{property}-m3-{role}
```

Where `property` is a Tailwind utility (`bg`, `text`, `border`) and `role` is the M3 color role.

## Color Roles

### Primary

Use for key UI elements: buttons, active states, links.

| Token | Usage |
|-------|-------|
| `bg-m3-primary` | Primary action backgrounds (filled buttons) |
| `text-m3-on-primary` | Text/icons on primary backgrounds |
| `bg-m3-primary-container` | Secondary emphasis surfaces (FABs, chips) |
| `text-m3-on-primary-container` | Text on primary containers |

### Secondary

Use for less prominent UI elements.

| Token | Usage |
|-------|-------|
| `bg-m3-secondary-container` | Tonal button backgrounds, filter chips |
| `text-m3-on-secondary-container` | Text on secondary containers |

### Tertiary

Use for accents and complementary elements.

| Token | Usage |
|-------|-------|
| `bg-m3-tertiary-container` | Tertiary FABs |
| `text-m3-on-tertiary-container` | Text on tertiary containers |

### Error

Use exclusively for error states and destructive actions.

| Token | Usage |
|-------|-------|
| `text-m3-error` | Error text, error icons |
| `bg-m3-error` | Error badges |
| `text-m3-on-error` | Text on error backgrounds |
| `bg-m3-error-container` | Error message backgrounds |

### Surface

Use for page backgrounds and content containers.

| Token | Usage |
|-------|-------|
| `bg-m3-surface` | Page background |
| `bg-m3-surface-container-low` | Elevated card backgrounds |
| `bg-m3-surface-container` | General container backgrounds |
| `bg-m3-surface-container-high` | Dialog backgrounds |
| `bg-m3-surface-container-highest` | Input field backgrounds, track fills |
| `text-m3-on-surface` | Primary text color |
| `text-m3-on-surface-variant` | Secondary text, labels, supporting text |
| `border-m3-outline` | Component outlines (outlined buttons, inputs) |
| `border-m3-outline-variant` | Decorative dividers |

### Inverse

Use for high-contrast overlays like snackbars and tooltips.

| Token | Usage |
|-------|-------|
| `bg-m3-inverse-surface` | Snackbar/tooltip background |
| `text-m3-inverse-on-surface` | Text on inverse surfaces |
| `text-m3-inverse-primary` | Accent text on inverse surfaces |

### Scrim

| Token | Usage |
|-------|-------|
| `bg-m3-scrim/32` | Dialog overlay (use with opacity) |

## Hover/Interaction States

Use opacity modifiers on foreground colors for state layers:

```
hover:bg-m3-primary/8       → 8% primary tint on hover
active:bg-m3-primary/12     → 12% primary tint on press
hover:bg-m3-on-surface/8    → 8% surface tint on hover (neutral elements)
```

## Decision Tree

1. Is it a primary action? → `bg-m3-primary` + `text-m3-on-primary`
2. Is it body text? → `text-m3-on-surface`
3. Is it secondary/supporting text? → `text-m3-on-surface-variant`
4. Is it a container/card? → `bg-m3-surface-container-low` (elevated) or `bg-m3-surface-container-highest` (filled)
5. Is it an error? → `text-m3-error` or `bg-m3-error`
6. Is it a tooltip/snackbar? → `bg-m3-inverse-surface` + `text-m3-inverse-on-surface`

## Elevation Shadows

| Token | Level | Usage |
|-------|-------|-------|
| `shadow-m3-1` | Level 1 | Elevated buttons, cards at rest |
| `shadow-m3-2` | Level 2 | Cards on hover |
| `shadow-m3-3` | Level 3 | FABs, dialogs |
| `shadow-m3-4` | Level 4 | FABs on hover |
| `shadow-m3-5` | Level 5 | Maximum elevation |
