---
title: "gif"
description: ""
summary: ""
date: 2024-01-25T13:18:03+01:00
lastmod: 2024-01-25T13:18:03+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "gif-267ffe5d3427129a2d2d3e4af8d63df3"
weight: 640
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add `.gif` images to your `.md` pages by using the [Markdown](https://daringfireball.net/projects/markdown/syntax#img) syntax for images.

## Examples

### Page resource

```md
![Good Morning cat](good-morning.gif)
```

![Good Morning cat](good-morning.gif)

#### Rendered HTML

```html
<img
  src="/docs/built-ins/gif/good-morning.gif"
  width="480"
  height="480"
  decoding="async"
  fetchpriority="auto"
  loading="lazy"
  alt="Good Morning cat"
  id="h-rh-i-0"
>
```

### Global resource

```md
![Unschuldig](gifs/unschuldig.gif)
```

![Unschuldig](gifs/unschuldig.gif)

### Remote resource

```md
![Swimming duck](https://media3.giphy.com/media/T3VjdigJhgYapB9Upz/giphy.gif)
```

![Swimming duck](https://media3.giphy.com/media/T3VjdigJhgYapB9Upz/giphy.gif)
