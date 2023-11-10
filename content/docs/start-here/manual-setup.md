---
title: "Manual Setup"
description: ""
summary: ""
date: 2023-11-08T12:26:26+01:00
lastmod: 2023-11-08T12:26:26+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "manual-setup-63d8f730cb9b7281a2d6c333721d4781"
weight: 520
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## Mounts

Add mounts to `./config/_default/module.toml`:

```toml
## assets
[[mounts]]
  source = "node_modules/@hyas/images/assets"
  target = "assets"

[[mounts]]
  source = "assets"
  target = "assets"

## layouts
[[mounts]]
  source = "node_modules/@hyas/images/layouts"
  target = "layouts"

[[mounts]]
  source = "layouts"
  target = "layouts"
```

## Parameters

Set parameters in `./config/_default/params.toml`:

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

## Processing options

Set [processing options](https://gohugo.io/content-management/image-processing/#processing-options) in `./config/_default/hugo.toml`:

```toml
[imaging]
  anchor = "Center"
  bgColor = "#ffffff"
  hint = "photo"
  quality = 85
  resampleFilter = "Lanczos"
```

## CSS

Add CSS class selectors to `./assets/scss/components/_images.scss`:

```scss
img[data-sizes="auto"] {
  display: block;
  width: 100%;
}

.figure {
  display: block;
}

.blur-up {
  filter: blur(5px);
  transition: filter 400ms;
}

.blur-up.lazyloaded {
  filter: unset;
}

figcaption {
  font-size: 1rem;
  margin-top: 0.5rem;
  font-style: italic;
}
```

## PostCSS

Add CSS class selectors to `safelist` in `./config/postcss.config.js`:

```js
..
      safelist: [
        'img-fluid',
        'lazyloaded',
        'blur-up',
      ],
..
```
