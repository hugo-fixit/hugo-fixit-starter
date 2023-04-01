---
title: Hello World
date: 2022-09-29T17:06:11+08:00
tags:
- hello
- FixIt
categories:
- hello
code:
  maxShownLines: 11
# See details front matter: https://fixit.lruihao.cn/documentation/content-management/introduction/#front-matter
---

Welcome to Hugo FixIt! This is your very first post.

<!--more-->

Head to the documentation page linked below for a complete guidence to get started with the [FixIt](https://github.com/hugo-fixit/FixIt) theme.

{{< link href="https://fixit.lruihao.cn/documentation/" content="All Documentation - FixIt" title="documentation of FixIt Theme" card=true >}}

## Quick Start

### Prerequisites

Just install latest version of [Hugo(>= 0.109.0)](https://gohugo.io/installation/) for your OS (Windows, Linux, macOS).

### Clone Template

Clone with your own repository url

```bash
git clone --recursive git@github.com:hugo-fixit/hugo-fixit-blog-go.git
```

Afterwards you can upgrade the theme with the following command:

```bash
# Update theme manually
hugo mod get -u github.com/hugo-fixit/FixIt
hugo mod tidy
```

### Launching the Site

```bash
# Development environment
hugo server --disableFastRender --navigateToChanged --bind 0.0.0.0
# Production environment
hugo server --disableFastRender --navigateToChanged --environment production --bind 0.0.0.0
```

<details>
  <summary>Start via NPM script</summary>

  ```bash
  # build the blog
  npm run build
  # run a local debugging server with watch
  npm run server
  # run a local debugging server in production environment
  npm run server:production
  # update theme submodules
  npm run update:theme
  ```

</details>

### Build the Site

When your site is ready to deploy, run the following command:

```bash
hugo
```

For a complete quick start, see this [page](https://fixit.lruihao.cn/documentation/getting-started/).

## Questions, ideas, bugs, pull requests

All feedback is welcome! Head over to the [issues](https://github.com/hugo-fixit/FixIt/issues) or [discussions](https://github.com/hugo-fixit/FixIt/discussions) tracker.
