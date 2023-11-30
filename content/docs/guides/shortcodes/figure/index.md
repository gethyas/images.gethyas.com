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
weight: 846
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
