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
weight: 830
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

Hyas Images supports the [Markdown syntax for displaying images](https://www.markdownguide.org/basic-syntax/#images-1) that includes alt-text for screen readers and assistive technology.

{{< callout context="note" icon="info-circle" >}}
Hyas Images uses a [Markdown render hook](https://gohugo.io/templates/render-hooks/) to render a responsive [`<img>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img).
{{< /callout >}}

## Page resource

```md
![Perched blue and orange bird](vincent-van-zalinge-vUNQaTtZeOo-unsplash.jpg)
```

![Perched blue and orange bird](vincent-van-zalinge-vUNQaTtZeOo-unsplash.jpg)

## Global resource

```md
![A bug is sitting on a green stem](images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg)
```

![A bug is sitting on a green stem](images/vincent-van-zalinge-IicWDdQUfsQ-unsplash.jpg)

## Remote resource

```md
![A close-up of a butterfly on a rope](https://images.unsplash.com/photo-1690198517569-45458a850563?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80)
```

![A close-up of a butterfly on a rope](https://images.unsplash.com/photo-1690198517569-45458a850563?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80)
