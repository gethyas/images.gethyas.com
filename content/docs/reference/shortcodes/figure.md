---
title: "figure"
description: ""
summary: ""
date: 2023-11-28T14:23:43+01:00
lastmod: 2023-11-28T14:23:43+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "figure-d6d8664a7203fc8681a006a8fccb5117"
weight: 926
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

This reference guide describes the [figure shortcode](/docs/shortcodes/figure/) arguments.

## Arguments

The `src` argument is required; others are optional.

### alt
(`string`) The `figure` element's `alt` attribute.

### class
(`string`) The figure element's `class` attribute.

### formats
(`string`) A comma- or space-delimited list of image formats, ordered by precedence, to use when creating images for the `srcset` attribute of each `source` element.

### loading
(`string`) The `figure` element's `loading` attribute. Default is `lazy`.

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
(`string`) The `figure` element's `title` attribute.

### width
(`int`) The display width of the image, in pixels, falling back to 100% of the viewport width.

### caption
(`string`) The `figure` element's `figcaption` attribute.
