# Feature Request: Add/Delete Row Support for Markdown Tables in Rich-Text Editor

## Summary

Allow users to add and delete rows in markdown tables directly within the rich-text editor, similar to how TipTap's table extension supports row manipulation programmatically.

## Current Behavior

The rich-text editor correctly recognizes and renders markdown tables, allowing users to edit cell contents inline. However, there is no UI to:
- Add a new row (above or below the current row)
- Delete an existing row
- Add/delete columns

Users must currently switch to raw markdown editing or use a workaround with `list: true` object fields in frontmatter to achieve editable, expandable data structures.

## Proposed Behavior

When the cursor is inside a table cell, provide UI controls to manipulate table structure:

1. **Context menu (right-click)** or **toolbar buttons** with options:
   - Insert row above
   - Insert row below
   - Delete row
   - Insert column left
   - Insert column right
   - Delete column

2. **Row/column handles** (optional): Visual handles on hover that allow drag-to-reorder or click-to-access row/column operations (similar to TipTap's TableNode component).

## Use Case

I'm building a petition site where multiple people sign by adding their name, title, and a link to evidence. The natural representation is a markdown table:

```markdown
| Name | Title | Evidence |
| --- | --- | --- |
| Jane Doe | AI Researcher | [Twitter](https://twitter.com/janedoe) |
| John Smith | Tech Journalist | [Article](https://example.com/article) |
```

Currently, editors can modify existing entries but cannot add new signatories without leaving the rich-text editor. This forces a workaround using YAML frontmatter with `type: object` and `list: true`, which is less intuitive for simple tabular data.

## Technical Context

TipTap (which powers the rich-text editor) already provides the underlying commands:
- `addRowBefore()`
- `addRowAfter()`
- `deleteRow()`
- `addColumnBefore()`
- `addColumnAfter()`
- `deleteColumn()`

The feature request is to expose these existing capabilities through a user-facing UI.

## References

- TipTap Table Extension: https://tiptap.dev/docs/editor/extensions/nodes/table
- TipTap TableNode UI Component: https://tiptap.dev/docs/ui-components/node-components/table-node

## Priority

Medium - There is a viable workaround using list fields, but native table row manipulation would significantly improve the editing experience for tabular content.
