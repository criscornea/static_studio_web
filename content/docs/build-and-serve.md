---
title: "Build and serve"
weight: 30
description: "Preview with a Hugo server and build with streamed output."
---

## Preview

The Preview button starts a `hugo server` bound to `127.0.0.1` on a free port and shows the page in a side-by-side frame. The server is stopped when you close or switch projects, and when Static Studio exits.

## Build

The Build button runs `hugo` in the project root. One build runs at a time and it can be cancelled. Output streams live to the build log panel, toggled with Ctrl/Cmd+J.

## Build errors

Hugo error lines are parsed into file, line and message. Affected pages are marked in the tree, the build panel lists the problems, and clicking one opens the page at that line.
