# Dialog

Modal overlay for focused tasks, confirmations, and alerts.

## Import

```tsx
import {
  Dialog, DialogTrigger, DialogContent,
  DialogHeader, DialogTitle, DialogDescription, DialogFooter, DialogClose
} from "m3-design-system";
```

## Usage

```tsx
<Dialog>
  <DialogTrigger asChild>
    <Button>Open Dialog</Button>
  </DialogTrigger>
  <DialogContent>
    <DialogHeader>
      <DialogTitle>Confirm Action</DialogTitle>
      <DialogDescription>This cannot be undone.</DialogDescription>
    </DialogHeader>
    <DialogFooter>
      <DialogClose asChild>
        <Button variant="text">Cancel</Button>
      </DialogClose>
      <Button>Confirm</Button>
    </DialogFooter>
  </DialogContent>
</Dialog>
```

## Structure

- `Dialog` — Root wrapper (manages open/close state).
- `DialogTrigger` — Element that opens the dialog.
- `DialogContent` — The modal panel. Includes overlay and close button automatically.
- `DialogHeader` — Contains title and description.
- `DialogTitle` — Required. The dialog heading.
- `DialogDescription` — Optional supporting text.
- `DialogFooter` — Action buttons. Aligned to the right.
- `DialogClose` — Wraps elements that close the dialog.

## Rules

- Always include a `DialogTitle` for accessibility.
- Place dismiss/cancel actions before confirm actions in `DialogFooter`.
- Do not nest dialogs inside dialogs.
- Use `DialogClose asChild` to make buttons close the dialog.
