---
title: "Image Overlay"
description: ""
summary: ""
date: 2023-11-09T16:43:06+01:00
lastmod: 2023-11-09T16:43:06+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "overlay-7507cdecdd9e414faad33a8e0027d8ba"
weight: 630
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images with an overlay using a shortcode or partial.

## Examples

### Watermark

Add a watermark to any image. To change the watermark location, set the `overlayAnchor` and adjust `overlayPadding` as needed. The `overlayPadding` and `overlayWidth` are a percentage of the base image width.

```md
{{</* picture 
  alt="Granada, Spain"
  overlay="images/logo-unsplash.png"
  overlayAnchor="BottomLeft"
  overlayPadding=0.0375
  overlayWidth=0.050
  src="https://images.unsplash.com/photo-1673105048185-a22384eb59a1?q=80&w=1742&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
*/>}}
```

{{< picture
  alt="Granada, Spain"
  overlay="images/logo-unsplash.png"
  overlayAnchor="BottomLeft"
  overlayPadding=0.0375
  overlayWidth=0.050
  src="https://images.unsplash.com/photo-1673105048185-a22384eb59a1?q=80&w=1742&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
>}}

### Frame within a frame

Place one image inside another. You can adjust the relative size of the overlay image with `overlayWidth`, a percentage of the base image width.

```md
{{</* picture 
  alt="A large bird flying over Granada, Spain"
  overlay="images/vincent-van-zalinge-6lRE6ScsC_o-unsplash-removebg.png"
  overlayAnchor="Center"
  overlayPadding=0.025
  overlayWidth=0.99
  src="https://images.unsplash.com/photo-1673105048185-a22384eb59a1?q=80&w=1742&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
*/>}}
```

{{< picture
  alt="A large bird flying over Granada, Spain"
  overlay="images/vincent-van-zalinge-6lRE6ScsC_o-unsplash-removebg.png"
  overlayAnchor="Center"
  overlayPadding=0.025
  overlayWidth=0.99
  src="https://images.unsplash.com/photo-1673105048185-a22384eb59a1?q=80&w=1742&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
>}}
