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
  "alt" "A close-up of a butterfly on a rope"
  "class" "foo"
  "formats" (slice "webp" "jpeg")
  "loading" "eager"
  "overlay" "images/logo-unsplash.png"
  "overlayAnchor" "bottomright"
  "overlayPadding" 0.0375
  "overlayWidth" 0.050
  "page" .
  "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg"
  "title" "A close-up of a butterfly on a rope"
  "width" 768
  "caption" "A close-up of a butterfly on a rope"
}}
{{- partial "figure" $opts }}
```
