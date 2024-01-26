---
title: "picture"
description: ""
summary: ""
date: 2023-11-09T16:48:27+01:00
lastmod: 2023-11-09T16:48:27+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "picture-542c9977843c7ac523b9e594c870f694"
weight: 420
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.md` pages by using the `picture` shortcode. See the [picture shortcode reference page](/docs/reference/shortcodes/picture/) for all available arguments.

## Examples

### Page resource

```md
{{</* picture class="rounded-3" decoding="auto" loading="eager" src="2024-01-22_16-55-13.jpg" alt="A bird with a little fish in its mouth" */>}}
```

{{< picture class="rounded-3" decoding="auto" loading="eager" src="2024-01-22_16-55-13.jpg" alt="A bird with a little fish in its mouth" >}}

### Global resource

```md
{{</* picture width="320" sizes="75vw" process="fill 1680x720" formats="webp, jpeg" src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" */>}}
```

{{< picture width="320" sizes="75vw" process="fill 1680x720" formats="webp, jpeg" src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" >}}

#### Rendered HTML

```html
<picture>
  <source
    type="image/webp"
    srcset="
      /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_8fb210b55a1c43fbe58035af75b837bf.webp 320w,
      /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_1195a0f60c161cfdbabfb3dc77802841.webp 640w,
      /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_509820779358c6fc814c2a74cc2b1d6d.webp 960w,
      /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_482e8ac2c6a51e65cabb739bbe32756f.webp 1280w,
      /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_ced355676c707141715af245d099fcc8.webp 1680w
    "
    sizes="75vw"
  >
  <source
    type="image/jpeg"
      srcset="
        /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_969769cd7c343d3f9bd0f20af670896d.jpg 320w,
        /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_ee4fd60a9ffe86d69ed9e37fb355049d.jpg 640w,
        /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_dca82a660d2dafd49dc880d76b5e6b97.jpg 960w,
        /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_63c97e8cfad907ea11e435a9ff999416.jpg 1280w,
        /images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_432153bfcfcbe1d5096b4b2684dad06c.jpg 1680w
      "
      sizes="75vw"
  >
  <img
    src="/images/vincent-van-zalinge-XIp7Wna0ua0-unsplash_hu3d03a01dcc18bc5be0e67db3d8d209a6_241522_969769cd7c343d3f9bd0f20af670896d.jpg"
    width="1680"
    height="720"
    decoding="async"
    fetchpriority="auto"
    loading="lazy"
    alt="A small bird perched on top of a tree branch"
  >
</picture>
```

### Remote resource

```md
{{</* picture src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" */>}}
```

{{< picture src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" >}}
