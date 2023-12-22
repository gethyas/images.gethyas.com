---
title: "Spotlight"
description: ""
summary: ""
date: 2023-12-14T16:33:26+01:00
lastmod: 2023-12-14T16:33:26+01:00
draft: true
menu:
  docs:
    parent: ""
    identifier: "spotlight-d060e3424b90a807a11b0720cea80725"
weight: 640
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

[Spotlight](https://github.com/nextapps-de/spotlight) is web's most easy to integrate lightbox gallery library. Super-lightweight, outstanding performance, no dependencies.

{{< callout context="caution" icon="alert-triangle" >}}
You will need `@hyas/images` 2.1.x or newer. [Check your version](/docs/start-here/getting-started/#check-if-images-is-installed).
{{< /callout >}}

## To Do

### Now

- [x] Proof of Concept
- [ ] Global and local setting to swith Spotlight on/off.
- [ ] Add limited/most used options only (there are sensible defaults).
- [ ] Add Gallery-Group shortcode and partial with options.
- [ ] Support shortcodes and partials fully
- [ ] Support Markdown image with sensible defaults + global setting only
{.list-unstyled}

### Later
- [ ] Light mode theme.
- [ ] Expand options
{.list-unstyled}

## Examples

```md
{{</* img
  src="vincent-van-zalinge-9NapHjhwxEg-unsplash.jpg"
  alt="A bird that is flying in the air"
  download=true
*/>}}
```

<a class="spotlight" data-download="true" href="vincent-van-zalinge-9NapHjhwxEg-unsplash.jpg">

{{< img src="vincent-van-zalinge-9NapHjhwxEg-unsplash.jpg" alt="A bird that is flying in the air" >}}

</a>
