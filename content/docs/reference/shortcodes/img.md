---
title: "img"
description: ""
summary: ""
date: 2023-11-28T14:23:35+01:00
lastmod: 2023-11-28T14:23:35+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "img-b7633eb1109e6cbdeef1e8b9bd84b3a3"
weight: 922
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

This reference guide describes the [img shortcode](/docs/shortcodes/img/) arguments.

## Arguments

The `src` argument is required; others are optional.

### src

A string containing the path to the image — a [page resource](/docs/basics/resources/#page-resource), a [global resource](/docs/basics/resources/#global-resource), or a [remote resource](/docs/basics/resources/#remote-resource).

### width

Integer containing the display width of the image in pixels, falling back to 100% of the viewport width — for example `320`.

### sizes

A string containing a comma-separated list of source size descriptors followed by an optional fallback size — for example `75vw`. Recommended resources:

- [HTMLImageElement: sizes property](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/sizes)
- [sizes=auto is a great idea](https://chriscoyier.net/2023/06/23/sizesauto-is-a-great-idea/)
- [Responsive Images - Serve Scaled Images](https://www.keycdn.com/blog/responsive-images)
- [Applying srcset: choosing the right sizes for responsive images at different breakpoints](https://medium.com/hceverything/applying-srcset-choosing-the-right-sizes-for-responsive-images-at-different-breakpoints-a0433450a4a3)

### formats

A string slice of image formats, ordered by precedence, used when creating images for the `srcset` attribute of each `source` element — for example `webp, jpeg`.

### process

A string containing a Hugo [process](https://gohugo.io/content-management/image-processing/#process) method — for example `fill 1680x720`.

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

### alt

String containing the `img` element's `alt` attribute.

### title

String containing the `img` element's `title` attribute.

### class

String containing the `img` element's `class` attribute.
