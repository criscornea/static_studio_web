---
title: "Getting started"
weight: 10
description: "Install Static Studio, start it and open your first Hugo site."
---

Static Studio is one Go binary. It serves a JSON API and an embedded web app on `127.0.0.1:7777`. Nothing leaves your machine except what you publish.

## Requirements

[Hugo](https://gohugo.io/) and `git` must be on your `PATH`. Publishing to your own server also needs the system `rsync` and `ssh`.

## Install

Download a binary from the Releases page, or build from source (Go and Node 22):

```sh
make build
./bin/studio
```

Open http://127.0.0.1:7777, pick your site folder, and edit. Recent projects are listed on the open screen for one-click access.

## Flags

| Flag | Default | Meaning |
| --- | --- | --- |
| `-addr` | `127.0.0.1:7777` | address to listen on |
| `-log-level` | `info` | `debug`, `info`, `warn` or `error` |
| `-log-format` | `text` | `text` or `json` |

## Scope

Hugo is supported. Astro projects are detected but rejected with a clear message. Plugins, theme design, general git integration, multi-user, cloud sync and auth are out of scope.
