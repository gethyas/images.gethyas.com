---
title: "Resource Locations"
description: ""
summary: ""
date: 2023-11-09T14:37:09+01:00
lastmod: 2023-11-09T14:37:09+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "resources-26b35ed085958e95e9b0e0b59ec3f575"
weight: 310
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
slug: resources
---

You can store your images as a page resource, global resource, or remote resource.

## Page resource

A page resource is a file within a [page bundle](https://gohugo.io/content-management/page-bundles/). A page bundle is a directory with an `index.md` or `_index.md` file at its root.

```bash
content/
└── posts/
    └── post-1/         # page bundle
        ├── index.md
        └── bird.jpg    # page resource
```

If you want to show a page resource image — use the path:

```bash
bird.jpg
```

## Global resource

A global resource is a file within the `assets` directory, or within any directory [mounted](https://gohugo.io/hugo-modules/configuration/#module-configuration-mounts) to the `assets` directory.

```bash
assets/
└── images/
    └── bird.jpg    # global resource
```

If you want to show a global resource image — use the path:

```bash
images/bird.jpg
```

## Remote resource

A remote resource is a file on a remote server, accessible via HTTP(S). If you want to show a remote resource image — use the URL:

```bash
https://images.unsplash.com/photo-1690198517569-45458a850563?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80
```
