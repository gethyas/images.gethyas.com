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
weight: 910
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

This reference guide describes the [Images parameters](/docs/basics/customizing-images/#update-parameters).

## Parameters

### decoding

A string representing the [decoding](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/decoding) hint. Possible values are:

`sync`

: Decode the image synchronously for atomic presentation with other content.

`async`

: Decode the image asynchronously and allow other content to be rendered before this completes.

`auto`

: No preference for the decoding mode; the browser decides what is best for the user. This is the default value, but different browsers have different defaults:

  - Chromium defaults to `sync`.
  - Firefox defaults to `async`.
  - Safari defaults to `sync` except in a small number of circumstances.

### fetchpriority

A string representing the [priority](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/fetchPriority) hint. Possible values are:

`high`
: Fetch the image at a high priority relative to other images.

`low`
: Fetch the image at a low priority relative to other images.

`auto`
: Default mode, which indicates no preference for the fetch priority. The browser decides what is best for the user.

### loading

A string providing a hint to the user agent as to how to best schedule the [loading](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/loading) of the image to optimize page performance. The possible values are:

`eager`
: The default behavior, `eager` tells the browser to load the image as soon as the `<img>` element is processed.

`lazy`
: Tells the user agent to hold off on loading the image until the browser estimates that it will be needed imminently. For instance, if the user is scrolling through the document, a value of `lazy` will cause the image to only be loaded shortly before it will appear in the window's [visual viewport](https://developer.mozilla.org/en-US/docs/Glossary/Visual_Viewport).

### widths

A slice of image widths ordered by pixel size, used when creating images for the `srcset` attribute of each `source` element — for example `[480, 576, 768, 1025, 1200, 1440]` Recommended resources:

- [HTMLImageElement: srcset property](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/srcset)
- [Responsive Images - Serve Scaled Images](https://www.keycdn.com/blog/responsive-images)
- [Applying srcset: choosing the right sizes for responsive images at different breakpoints](https://medium.com/hceverything/applying-srcset-choosing-the-right-sizes-for-responsive-images-at-different-breakpoints-a0433450a4a3)

### sizes

A string containing a comma-separated list of source size descriptors followed by an optional fallback size — for example `75vw`. Recommended resources:

- [HTMLImageElement: sizes property](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/sizes)
- [sizes=auto is a great idea](https://chriscoyier.net/2023/06/23/sizesauto-is-a-great-idea/)
- [Responsive Images - Serve Scaled Images](https://www.keycdn.com/blog/responsive-images)
- [Applying srcset: choosing the right sizes for responsive images at different breakpoints](https://medium.com/hceverything/applying-srcset-choosing-the-right-sizes-for-responsive-images-at-different-breakpoints-a0433450a4a3)

### process

A string containing a Hugo [process](https://gohugo.io/content-management/image-processing/#process) method — for example `fill 1680x720`.
