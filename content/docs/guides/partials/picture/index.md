---
title: "<picture>"
description: ""
summary: ""
date: 2023-11-09T16:50:56+01:00
lastmod: 2023-11-09T16:50:56+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "picture-29c573839459b74e792c94ac0f74568c"
weight: 854
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## Examples

### Required arguments only

```html
{{- partial "picture.html" (dict "page" . "src" "images/zion.jpg") }}
```

### All arguments

```html
{{- $opts := dict
  "alt" "Bryce Canyon National Park"
  "class" "foo"
  "formats" (slice "webp" "jpeg")
  "loading" "eager"
  "overlay" "images/logo.png"
  "overlayAnchor" "bottomright"
  "overlayPadding" 0.02
  "overlayWidth" 0.25
  "page" .
  "src" "images/bryce-canyon-national-park.jpg"
  "title" "A beautiful day in Bryce Canyon National Park"
  "title" "A beautiful day in Bryce Canyon National Park"
  "width" 768
}}
{{- partial "picture.html" $opts }}
```
