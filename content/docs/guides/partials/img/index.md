---
title: "img"
description: ""
summary: ""
date: 2023-11-09T16:50:46+01:00
lastmod: 2023-11-09T16:50:46+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "img-73fde1b0a94e33b9dbe13c6bb1eb86e8"
weight: 852
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.html` pages by using the `img` partial. See the [img partial reference page](/docs/reference/partials/img/) for all available arguments.

## Examples

### Required arguments only

```go
{{- partial "img" (dict "page" . "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg") }}
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
}}
{{- partial "img" $opts }}
```
