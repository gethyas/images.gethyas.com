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
weight: 330
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

```toml {title=params.toml}
# Images (@hyas/images)
[hyas_images]
  [hyas_images.defaults]
    decoding = "async" # sync, async, or auto (default)
    fetchpriority = "auto" # high, low, or auto (default) 
    loading = "lazy" # eager or lazy (default)
    widths = [480, 576, 768, 1025, 1200, 1440] # [640, 768, 1024, 1366, 1600, 1920] for example
    sizes = "auto" # 100vw (default), 75vw, or auto for example
    process = "" # "fill 1600x900" or "fill 2100x900" for example
    lqip = "16x webp q20" # "16x webp q20" or "21x webp q20" for example
```

## Update processing options

Update [processing options](https://gohugo.io/content-management/image-processing/#processing-options) in `./config/_default/hugo.toml`:

```toml {title=hugo.toml}
[imaging]
  anchor = "Center"
  bgColor = "#ffffff"
  hint = "photo"
  quality = 85
  resampleFilter = "Lanczos"
```
