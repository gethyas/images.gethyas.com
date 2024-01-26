---
title: "img"
description: ""
summary: ""
date: 2023-11-09T16:44:55+01:00
lastmod: 2023-11-09T16:44:55+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "img-9e488db6ee7b133adb11ec93bf3b6eb0"
weight: 410
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.md` pages by using the `img` shortcode. See the [img shortcode reference page](/docs/reference/shortcodes/img/) for all available arguments.

## Examples

### Page resource

```md
{{</* img src="vincent-van-zalinge-zwFyZI70zlU-unsplash.jpg" alt="A white bird flying over a lush green field" */>}}
```

{{< img src="vincent-van-zalinge-zwFyZI70zlU-unsplash.jpg" alt="A white bird flying over a lush green field" >}}

#### Rendered HTML

```html
<img
  srcset="
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_480x0_resize_q85_h2_lanczos.webp 480w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_576x0_resize_q85_h2_lanczos.webp 576w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_768x0_resize_q85_h2_lanczos.webp 768w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_1025x0_resize_q85_h2_lanczos.webp 1025w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_1200x0_resize_q85_h2_lanczos.webp 1200w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_1440x0_resize_q85_h2_lanczos.webp 1440w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_1920x0_resize_q85_h2_lanczos.webp 1920w
  "
  sizes="75vw"
  src="/docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_480x0_resize_q85_lanczos.jpg"
  width="1920"
  height="1280"
  decoding="async"
  fetchpriority="auto"
  loading="lazy"
  alt="A white bird flying over a lush green field"
>
```

### Global resource

```md
{{</* img src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" */>}}
```

{{< img src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" >}}

### Remote resource

```md
{{</* img src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" */>}}
```

{{< img src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" >}}
