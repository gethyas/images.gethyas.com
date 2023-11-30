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
weight: 844
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
{{</* picture src="vincent-van-zalinge-6lRE6ScsC_o-unsplash.jpg" alt="A large bird flying through a blue sky" */>}}
```

{{< picture src="vincent-van-zalinge-6lRE6ScsC_o-unsplash.jpg" alt="A large bird flying through a blue sky" >}}

### Global resource

```md
{{</* picture src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" */>}}
```

{{< picture src="images/vincent-van-zalinge-XIp7Wna0ua0-unsplash.jpg" alt="A small bird perched on top of a tree branch" >}}

### Remote resource

```md
{{</* picture src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" */>}}
```

{{< picture src="https://images.unsplash.com/photo-1699192781399-e2275a9f60b6?q=80&w=1740&auto=format&fit=crop" alt="A small bird perched on top of a pine tree" >}}
