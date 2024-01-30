---
title: "Blog Post Cover Image"
description: ""
summary: ""
date: 2023-11-10T20:43:26+01:00
lastmod: 2023-11-10T20:43:26+01:00
draft: true
menu:
  docs:
    parent: ""
    identifier: "blog-0f2ab30692aa8c549c91e792d11ee6e9"
weight: 610
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can show a blog post cover image in your blog pages.

## Cover image

Show a blog post cover image in your [blog list](/blog/) and [blog post](/blog/example-post/) pages by adding a [page resource](/docs/basics/resources/#page-resource) image with a filename containing `feature`, `cover`, or `thumbnail`.

```bash
cover-vincent-van-zalinge-XJO99LpVHnU-unsplash.jpg
```

## Settings

Change default settings in `config/_default/params.toml`:

```toml { title="params.toml" }
# Doks (@hyas/doks-core)
[doks]

  # Blog
  relatedPosts = false # false (default) or true
  imageList = true # true (default) or false
  imageSingle = true # true (default) or false
```
