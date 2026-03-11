# Tabs

Content organization into switchable panels.

## Import

```tsx
import { Tabs, TabsList, TabsTrigger, TabsContent } from "m3-design-system";
```

## Usage

```tsx
<Tabs defaultValue="overview">
  <TabsList>
    <TabsTrigger value="overview">Overview</TabsTrigger>
    <TabsTrigger value="details">Details</TabsTrigger>
    <TabsTrigger value="reviews">Reviews</TabsTrigger>
  </TabsList>
  <TabsContent value="overview">Overview content</TabsContent>
  <TabsContent value="details">Details content</TabsContent>
  <TabsContent value="reviews">Reviews content</TabsContent>
</Tabs>
```

## Structure

- `Tabs` — Root. Set `defaultValue` for uncontrolled or `value`/`onValueChange` for controlled.
- `TabsList` — Container for tab triggers. Renders a horizontal bar with bottom border.
- `TabsTrigger` — Individual tab button. Active tab shows a primary-colored bottom border.
- `TabsContent` — Panel content. Only the active panel is visible.

## Rules

- Use 2-5 tabs. More than 5 is hard to navigate.
- Tab labels should be short (1-2 words).
- Do not use tabs for sequential steps — use a stepper pattern instead.
