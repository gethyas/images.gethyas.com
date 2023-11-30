---
title: "picture"
description: ""
summary: ""
date: 2023-11-10T19:45:58+01:00
lastmod: 2023-11-10T19:45:58+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "picture-1376df46b3aac933c8bdabf0fa2efe0a"
weight: 914
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

This reference guide describes the [picture shortcode](/docs/guides/shortcodes/picture/) arguments.

## Arguments

The `src` argument is required; others are optional.

### alt
(`string`) The `img` element's `alt` attribute.

### class
(`string`) The img element's `class` attribute.

### formats
(`string`) A comma- or space-delimited list of image formats, ordered by precedence, to use when creating images for the `srcset` attribute of each `source` element.

### loading
(`string`) The `img` element's `loading` attribute. Default is `lazy`.

### overlay
(`string`) The path to the overlay image: a page resource, a global resource, or a remote resource.

### overlayAnchor
(`string`) The anchor point of the overlay image. May be one of `TopLeft`, `Top`, `TopRight`, `Left`, `Center`, `Right`, `BottomLeft`, `Bottom`, or `BottomRight`. The value is case-insensitive. Default is `BottomRight`.

### overlayPadding
(`float`) The padding around the overlay image, as a percentage of the base image width, between 0 and 1 (inclusive). Default is `0.00`.

### overlayWidth
(`float`) The width of the overlay image, as a percentage of the base image width, between 0 and 1. Default is `0.20`.

### src
(`string`) The path to the base image: a page resource, a global resource, or a remote resource.

### title
(`string`) The `img` element's `title` attribute.

### width
(`int`) The display width of the image, in pixels, falling back to 100% of the viewport width.
