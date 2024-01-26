---
title: "figure"
description: ""
summary: ""
date: 2023-11-09T16:48:34+01:00
lastmod: 2023-11-09T16:48:34+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "figure-70458aac7861b66a081360f8fdc6c12d"
weight: 430
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.md` pages by using the `figure` shortcode. See the [figure shortcode reference page](/docs/reference/shortcodes/figure/) for all available arguments.

## Examples

### Page resource

```md
{{</* figure
  src="vincent-van-zalinge-e5VzJJDODbQ-unsplash.jpg"
  alt="A yellow and black bird sitting on top of a body of water"
  caption="A yellow and black bird sitting on top of a body of water. Photo by Vincent van Zalinge"
*/>}}
```

{{< figure src="vincent-van-zalinge-e5VzJJDODbQ-unsplash.jpg" alt="A yellow and black bird sitting on top of a body of water" caption="A yellow and black bird sitting on top of a body of water. Photo by Vincent van Zalinge" >}}

#### Rendered HTML

```html
<figure>
  <img
    srcset="
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_480x0_resize_q85_h2_lanczos.webp 480w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_576x0_resize_q85_h2_lanczos.webp 576w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_768x0_resize_q85_h2_lanczos.webp 768w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_1025x0_resize_q85_h2_lanczos.webp 1025w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_1200x0_resize_q85_h2_lanczos.webp 1200w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_1440x0_resize_q85_h2_lanczos.webp 1440w,
      /docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_1920x0_resize_q85_h2_lanczos.webp 1920w
    "
    sizes="75vw"
    src="/docs/shortcodes/figure/vincent-van-zalinge-e5VzJJDODbQ-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_162847_480x0_resize_q85_lanczos.jpg"
    width="1920"
    height="1280"
    decoding="async"
    fetchpriority="auto"
    loading="lazy"
    alt="A yellow and black bird sitting on top of a body of water"
  >
  <figcaption>
    A yellow and black bird sitting on top of a body of water. Photo by Vincent van Zalinge
  </figcaption>
</figure>
```

### Global resource

```md
{{</* figure
  src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg"
  alt="A small bird perched on top of a tree branch"
  caption="A small bird perched on top of a tree branch. Photo by Vincent van Zalinge"
*/>}}
```

{{< figure src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" caption="A small bird perched on top of a tree branch. Photo by Vincent van Zalinge" >}}

### Remote resource

```md
{{</* figure
  src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg"
  alt="A small bird perched on top of a pine tree"
  caption="A small bird perched on top of a pine tree. Photo by Vincent van Zalinge"
*/>}}
```

{{< figure src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" caption="A small bird perched on top of a pine tree. Photo by Vincent van Zalinge" >}}
