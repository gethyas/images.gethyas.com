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
weight: 120
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

The quickest way to get started with Images is using a Thulite theme with [Images already installed](/docs/start-here/getting-started/#check-if-images-is-installed). If you want to add Images to an existing Thulite project, this guide will explain how.

## Set up Images

To follow this guide, you'll need an existing Thulite project.

### Add the Images integration

Images is a [Thulite integration](https://docs.thulite.io/guides/integrations/). Add it to your site by running the following command in your project's root directory:

{{< tabs "install-images" >}}
{{< tab "npm" >}}

```bash
npm install @thulite/images@latest
```

{{< /tab >}}
{{< tab "pnpm" >}}

```bash
pnpm install @thulite/images@latest
```

{{< /tab >}}
{{< tab "Yarn" >}}

```bash
yarn add @thulite/images@latest
```

{{< /tab >}}
{{< /tabs >}}

This will install the required dependencies.

### Configure the integration

#### Update mounts

Add mounts to `./config/_default/module.toml`:

```toml {title=module.toml}
## assets
[[mounts]]
  source = "node_modules/@thulite/images/assets"
  target = "assets"

[[mounts]]
  source = "assets"
  target = "assets"

## layouts
[[mounts]]
  source = "node_modules/@thulite/images/layouts"
  target = "layouts"

[[mounts]]
  source = "layouts"
  target = "layouts"
```

#### Add parameters

Add the following [parameters](/docs/reference/configuration/#parameters) to `./config/_default/params.toml`:

```toml {title=params.toml}
# Images (@thulite/images)
[thulite_images]
  [thulite_images.defaults]
    decoding = "async" # sync, async, or auto (default)
    fetchpriority = "auto" # high, low, or auto (default)
    loading = "lazy" # eager or lazy (default)
    widths = [480, 576, 768, 1025, 1200, 1440] # [640, 768, 1024, 1366, 1600, 1920] for example
    sizes = "auto" # 100vw (default), 75vw, or auto for example
    process = "" # "fill 1600x900" or "fill 2100x900" for example
    lqip = "16x webp q20" # "16x webp q20" or "21x webp q20" for example
```

#### Set processing options

Set [processing options](https://gohugo.io/content-management/image-processing/#processing-options) in `./config/_default/hugo.toml`:

```toml {title=hugo.toml}
[imaging]
  anchor = "Center"
  bgColor = "#ffffff"
  hint = "photo"
  quality = 85
  resampleFilter = "Lanczos"
```

#### Add CSS

Add CSS class selectors to `./assets/scss/components/_images.scss`:

```scss {title=_images.scss}
img {
  height: auto;
  max-width: 100%;
}

img, picture {
  font-size: 0;
}

img[data-sizes="auto"] {
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

#### Update PostCSS settings

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

### Add images

Images is now set up and it's time to add some images!

- Add images to your `.md` pages by using Markdown or by using the `img`, `picture`, or `figure` shortcode.
- Add images to your `html` pages by using the the `img`, `picture`, or `figure` partial.

## Next steps

- **Resources**: Learn where to store your images in the ["Resource Locations"](/docs/basics/resources/) guide.
- **Shortcodes**: Get started with the ["img"](/docs/shortcodes/img/), ["picture"](/docs/shortcodes/picture/), and ["figure"](/docs/shortcodes/figure/) shortcode guides.
- **Partials**: Get started with the ["img"](/docs/partials/img/), ["picture"](/docs/partials/picture/), and ["figure"](/docs/partials/figure/) partial guides.
