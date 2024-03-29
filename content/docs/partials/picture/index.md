---
title: "picture"
description: ""
summary: ""
date: 2023-11-09T16:50:56+01:00
lastmod: 2023-11-09T16:50:56+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "picture-29c573839459b74e792c94ac0f74568c"
weight: 520
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.html` pages by using the `picture` partial. See the [picture partial reference page](/docs/reference/partials/picture/) for all available arguments.

## Examples

### Required arguments only

```go
{{- partial "picture" (dict "page" . "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg") }}
```

### All arguments

```go
{{- $opts := dict
  "page" .
  "src" "images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg"
  "width" 768
  "sizes" "auto"
  "formats" (slice "webp" "jpeg")
  "process" "fill 1600x900"
  "lqip" "16x webp q20"
  "decoding" "async"
  "fetchpriority" "auto"
  "loading" "eager"
  "alt" "A close-up of a butterfly on a rope"
  "title" "A close-up of a butterfly on a rope"
  "class" "foo"
}}
{{- partial "picture" $opts }}
```
