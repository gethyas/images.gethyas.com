---
title: "Getting Started"
description: ""
summary: ""
date: 2023-11-08T11:42:20+01:00
lastmod: 2023-11-08T11:42:20+01:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "getting-started-fa68d7c8600c3a18e71e96b5bcbde732"
weight: 110
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

Images is the official images integration for the [Thulite](https://thulite.io/) framework. This guide will help you get started with Images already installed. See the [manual setup instructions](/docs/start-here/manual-setup/) to add Images to an existing Thulite project.

## Quick start

To follow this guide, you'll need an existing Thulite project with Images installed.

### Check if Images is installed

Check if Images is installed by running the following command in your project's root directory:

{{< tabs "install-images" >}}
{{< tab "npm" >}}

```bash
npm list @hyas/images
```

{{< /tab >}}
{{< tab "pnpm" >}}

```bash
pnpm list @hyas/images --depth 1
```

{{< /tab >}}
{{< tab "Yarn" >}}

```bash
yarn list @hyas/images --depth=1
```

{{< /tab >}}
{{< /tabs >}}

This will print the version of the package installed. If nothing is printed, you'll first need to add Images — proceed with the [manual setup instructions](/docs/start-here/manual-setup/).

### Add images

Images is installed and it's time to add some images!

- Add images to your `.md` pages by using Markdown or by using the `img`, `picture`, or `figure` shortcode.
- Add images to your `html` pages by using the the `img`, `picture`, or `figure` partial.

### Next steps

- **Resources**: Learn where to store your images in the ["Resource Locations"](/docs/basics/resources/) guide.
- **Shortcodes**: Get started with the ["img"](/docs/shortcodes/img/), ["picture"](/docs/shortcodes/picture/), and ["figure"](/docs/shortcodes/figure/) shortcode guides.
- **Partials**: Get started with the ["img"](/docs/partials/img/), ["picture"](/docs/partials/picture/), and ["figure"](/docs/partials/figure/) partial guides.

## Updating Images

Images is a Thulite integration, and is updated like any `@hyas/*` integration (or theme):

{{< tabs "update-images" >}}
{{< tab "npm" >}}

```bash
npm install @hyas/images@latest
```

{{< /tab >}}
{{< tab "pnpm" >}}

```bash
pnpm upgrade @hyas/images --latest
```

{{< /tab >}}
{{< tab "Yarn" >}}

```bash
yarn upgrade @hyas/images --latest
```

{{< /tab >}}
{{< /tabs >}}

See the [Images changelog](https://github.com/gethyas/images/blob/main/CHANGELOG.md) for a full list of the changes made in each release.

## Troubleshooting Images

Use the [project configuration](/docs/reference/configuration/), shortcodes (["img"](/docs/reference/shortcodes/img/), ["picture"](/docs/reference/shortcodes/picture/), and ["figure"](/docs/reference/shortcodes/figure/)), and partials (["img"](/docs/reference/partials/img/), ["picture"](/docs/reference/partials/picture/), and ["figure"](/docs/reference/partials/figure/)) reference pages to ensure that images is configured and functioning properly. See the guides in the sidebar for help storing images and customizing your Images setup.

If your answer cannot be found in these docs, please visit the [full Thulite Docs](https://docs.thulite.io/) for complete Thulite documentation. Your question may be answered by understanding how Thulite works in general, underneath this Images integration.

You can also check for any known [Images issues on GitHub](https://github.com/gethyas/images/issues), and get help in [Thulite Discussions](https://github.com/gethyas/hyas/discussions) from our active, friendly community!

## Credits

All photos on this site are by [Vincent van Zalinge](https://unsplash.com/@vincentvanzalinge).

All illustrations on this site are by [Franziska Höllbacher](https://giphy.com/franziskahoellbacher).

This npm package is based on:

- [Image render hook](https://www.veriphor.com/articles/link-and-image-render-hooks/#image-render-hook)
- [Images with overlays](https://www.veriphor.com/articles/images-with-overlays/)
