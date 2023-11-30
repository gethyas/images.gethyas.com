---
title: "Configuration"
description: ""
summary: ""
date: 2023-11-29T10:47:42+01:00
lastmod: 2023-11-29T10:47:42+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "configuration-cc48b7360e5d947bc63c77e137bb5d69"
weight: 900
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

This reference guide describes the [Images parameters](/docs/guides/customizing-images/#update-parameters).

## Parameters

### Landscape

#### normalize

(`string`) The normalized image's width and height, in pixels. Default is `1600x900`.

#### lqip

(`string`) The LQIP image's width and height, in pixels. Default is `16x9`.

#### widths

(`string slice`) A slice of image widths, ordered by precendence, used when creating images for the `srcset` attribute of each `source` element.

### Portrait

#### normalize

(`string`) The normalized image's width and height, in pixels. Default is `900x1600`.

#### lqip

(`string`) The LQIP image's width and height, in pixels. Default is `9x16`.

#### widths

(`string slice`) A slice of image widths, ordered by precendence, used when creating images for the `srcset` attribute of each `source` element.
