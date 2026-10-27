---
title: "Editing"
weight: 20
description: "Browse the content tree, edit Markdown and frontmatter, and add images."
---

## Content tree

The sidebar shows every Hugo content directory as a tree, with pages listed by title. You can search titles, tags and bodies (Ctrl/Cmd+K), sort by name, title or date, and filter by draft status and tag. Create a page from an archetype with the plus button, and rename or delete pages from the right-click menu.

## Markdown editor

The editor is CodeMirror 6 with GFM Markdown. It autosaves after a 1.5 second pause and on page switch, and shows a Saved, Unsaved, Saving or Conflict state. If the file changed on disk, the save is reported as a conflict instead of overwriting your external change.

Live preview renders headings, bold, italic, links, quotes and lists inline, and shows the markup only on lines the cursor touches. A switch in the editor header returns to plain source. A floating toolbar offers headings, bold, italic, code, link, lists and quote.

## Frontmatter

A form above the editor edits title, date, draft and tags. Unknown keys are kept. Comments and TOML key order are not.

## Images

Drop an image onto the editor to upload it to `<assetDir>/images/` and insert `![](/images/name.png)`. PNG, JPEG, GIF and WebP up to 10 MB are accepted, and existing files are never overwritten.

## Command palette

Ctrl/Cmd+Shift+P opens the command palette, Ctrl/Cmd+P opens quick-open for pages, and Ctrl/Cmd+/ lists every shortcut.
