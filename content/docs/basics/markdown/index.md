---
title: "Markdown"
description: ""
summary: ""
date: 2023-11-09T12:54:19+01:00
lastmod: 2023-11-09T12:54:19+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "markdown-ed2167cc27ea7fa3a03835e9e0907fba"
weight: 320
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can add images to your `.md` pages by using the [Markdown](https://daringfireball.net/projects/markdown/syntax#img) syntax for images.

## Examples

### Page resource

```md
![A bird with a little fish in its mouth](2024-01-22_16-55-13.jpg "A bird with a little fish in its mouth")
```

![A bird with a little fish in its mouth](2024-01-22_16-55-13.jpg "A bird with a little fish in its mouth")

#### Rendered HTML

```html
<img
  src="/docs/basics/markdown/2024-01-22_16-55-13_hu2f182e3f395c5b315c12df5e4e37e701_15767_410x274_resize_q85_h2_lanczos.webp"
  width="410"
  height="274"
  decoding="async"
  fetchpriority="auto"
  loading="lazy"
  alt="A bird with a little fish in its mouth"
  title="A bird with a little fish in its mouth"
  id="h-rh-i-0"
>
```

### Global resource

```md
![A bug is sitting on a green stem](images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg)
```

![A bug is sitting on a green stem](images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg)

### Remote resource

```md
![A young lion cub walking through a wooded area](https://images.unsplash.com/photo-1703237307519-104c7aebf46c?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwcm9maWxlLXBhZ2V8M3x8fGVufDB8fHx8fA%3D%3D)
```

![A young lion cub walking through a wooded area](https://images.unsplash.com/photo-1703237307519-104c7aebf46c?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwcm9maWxlLXBhZ2V8M3x8fGVufDB8fHx8fA%3D%3D)
