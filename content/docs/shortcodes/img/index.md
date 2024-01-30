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
{{</* img process="fill 2100x900" lqip="21x webp q20" loading="eager" fetchpriority="high" src="vincent-van-zalinge-zwFyZI70zlU-unsplash.jpg" alt="A white bird flying over a lush green field" */>}}
```

{{< img process="fill 2100x900" lqip="21x webp q20" loading="eager" fetchpriority="high" src="vincent-van-zalinge-zwFyZI70zlU-unsplash.jpg" alt="A white bird flying over a lush green field" >}}

#### Rendered HTML

```html
<img
  srcset="
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_a8ecff7789b05bbbf84231dda8c81785.webp 480w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_e25b96b1be511e66b3700a10f1a19229.webp 576w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_42102e684f35abe70212aca85dbe4026.webp 768w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_5c2e9ffc10c607d411edbb7aaac9cb79.webp 1025w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_7c866e9d0bf04bfa5fabf1515fc56100.webp 1200w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_8c0caecdd38e190fe26fffeefbdd8bc8.webp 1440w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_8ca397ce816fcd7b5e41c666963cccdf.webp 2100w
  "
  data-srcset="
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_a8ecff7789b05bbbf84231dda8c81785.webp 480w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_e25b96b1be511e66b3700a10f1a19229.webp 576w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_42102e684f35abe70212aca85dbe4026.webp 768w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_5c2e9ffc10c607d411edbb7aaac9cb79.webp 1025w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_7c866e9d0bf04bfa5fabf1515fc56100.webp 1200w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_8c0caecdd38e190fe26fffeefbdd8bc8.webp 1440w,
    /docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_8ca397ce816fcd7b5e41c666963cccdf.webp 2100w
  "
  data-sizes="auto"
  src="/docs/shortcodes/img/vincent-van-zalinge-zwFyZI70zlU-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_240654_4db57474e1546e5b578993f44916d3e6.jpg"
  width="2100"
  height="900"
  decoding="async"
  fetchpriority="high"
  loading="eager"
  alt="A white bird flying over a lush green field"
  class="lazyautosizes ls-is-cached lazyloaded"
  sizes="648px"
>
```

### Global resource

```md
{{</* img process="fill 1600x900" src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" */>}}
```

{{< img process="fill 1600x900" src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" >}}

### Remote resource

```md
{{</* img process="fill 1600x900" src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" */>}}
```

{{< img process="fill 1600x900" src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" >}}
