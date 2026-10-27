---
title: "Publish"
weight: 40
description: "Publish public/ to GitHub Pages or to your own server over rsync."
---

The Publish button runs a Hugo build, then publishes `public/`. No credentials are stored. Your SSH key, agent or credential helper signs in.

## GitHub Pages

Choose a remote and a branch (default `gh-pages`). Settings are saved per project in the user config directory. Static Studio commits `public/` in a temporary repository and force-pushes it with the system `git`.

## rsync over SSH

Pick the rsync target and set:

- the destination, as `user@host:path` or a full local path
- the port
- an optional identity file
- an optional delete option, shown with a warning
- an optional dry run

The system `rsync` runs from `public/` with an argument list only, no shell, and without following symlinks. SSH uses `BatchMode`, your agent, your SSH config and `known_hosts`. Host key checking is never turned off, so connect once with `ssh` in a terminal first. Unknown host keys, refused logins, missing programs and unreachable hosts give readable messages.
