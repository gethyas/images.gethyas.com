---
title: "figure"
description: ""
summary: ""
date: 2023-11-09T16:50:41+01:00
lastmod: 2023-11-09T16:50:41+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "figure-366fd0d288cb480a67a61ac01f61785c"
weight: 530
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.html` pages by using the `figure` partial. See the [figure partial reference page](/docs/reference/partials/figure/) for all available arguments.

## Examples

### Required arguments only

```go
{{- partial "figure" (dict "page" . "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg") }}
```

### All arguments

```go
{{- $opts := dict
  "page" .
  "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg"
  "width" 768
  "sizes" "auto"
  "formats" (slice "webp" "jpeg")
  "process" "fill 1680x720"
  "decoding" "async"
  "fetchpriority" "auto"
  "loading" "eager"
  "alt" "A close-up of a butterfly on a rope"
  "title" "A close-up of a butterfly on a rope"
  "caption" "A close-up of a butterfly on a rope"
  "class" "foo"
}}
{{- partial "figure" $opts }}
```
