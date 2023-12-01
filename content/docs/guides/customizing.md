---
title: "Customizing Images"
description: ""
summary: ""
date: 2023-11-30T14:45:21+01:00
lastmod: 2023-11-30T14:45:21+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "customizing-images-f36de4637c9b0d897aa3bcdc314d1d18"
weight: 825
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

You can customize Images by updating parameters and processing options.

## Update parameters

Update the following [parameters](/docs/reference/configuration/#parameters) in `./config/_default/params.toml`:

```toml
# Images (@hyas/images)
[hyas_images]
  [hyas_images.landscape]
    normalize = "1360x765" # "1600x900" (default)
    lqip = "16x9" # "16x9" (default)
    widths = [480, 640, 800, 1024]
  [hyas_images.portrait]
    normalize = "765x1360" # "900x1600" (default)
    lqip = "9x16" # "9x16" (default)
    widths = [480, 640, 800, 1024]
```

## Update processing options

Update [processing options](https://gohugo.io/content-management/image-processing/#processing-options) in `./config/_default/hugo.toml`:

```toml
[imaging]
  anchor = "Center"
  bgColor = "#ffffff"
  hint = "photo"
  quality = 85
  resampleFilter = "Lanczos"
```
