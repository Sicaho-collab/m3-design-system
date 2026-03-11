# Card

Content container for grouping related information.

## Import

```tsx
import { Card, CardHeader, CardTitle, CardDescription, CardContent, CardFooter } from "m3-design-system";
```

## Props (Card)

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| variant | `"elevated" \| "filled" \| "outlined"` | `"elevated"` | Visual style |

## Variant Selection

- **elevated** — Primary content. Has shadow. Use for main content cards.
- **filled** — Supporting content. Uses `surface-container-highest` background. Use for secondary content.
- **outlined** — Content with clear boundary. Use when cards sit on colored surfaces.

## Structure

```tsx
<Card variant="elevated">
  <CardHeader>
    <CardTitle>Title</CardTitle>
    <CardDescription>Supporting text</CardDescription>
  </CardHeader>
  <CardContent>
    <p>Card content here</p>
  </CardContent>
  <CardFooter>
    <Button variant="text">Action</Button>
  </CardFooter>
</Card>
```

## Rules

- Always include `CardHeader` with at least a `CardTitle`.
- Place actions in `CardFooter`, not `CardContent`.
- Do not nest cards inside cards.
