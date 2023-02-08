---
title: "Hello World"
date: 2022-09-29T17:06:11+08:00
tags:
- hello
- FixIt
categories:
- hello
code:
  maxShownLines: 11
# See details front matter: https://fixit.lruihao.cn/theme-documentation-content/#front-matter
---

Welcome to Hugo FixIt! This is your very first post.

<!--more-->

Head to the documentation page linked below for a complete guidence to get started with the [FixIt](https://github.com/hugo-fixit/FixIt) theme.

{{< link href="https://fixit.lruihao.cn/theme-documentation-basics/" content="FixIt" title="documentation of FixIt Theme" card=true >}}

## Quick Start

There are two ways to start this blog.

### NPM

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

### Hugo

```bash
# Development environment
hugo server --disableFastRender --navigateToChanged --bind 0.0.0.0
# Production environment
hugo server --disableFastRender --navigateToChanged --environment production --bind 0.0.0.0
# Update theme manually
hugo mod get -u github.com/hugo-fixit/FixIt
hugo mod tidy
```

In addition, you can run `hugo_main.sh` to choice frequently-used Hugo commands:

```bash
cd .shell && sh hugo_main.sh
```

```text
--------------Hugo Admin--------------
Please enter the serial number to work
--------------------------------------
1. post
2. server
3. server:production
4. build
5. submodule-sync
6. push
--------------------------------------
Press Ctrl+C to stop
```

## Questions, ideas, bugs, pull requests

All feedback is welcome! Head over to the [issues](https://github.com/hugo-fixit/FixIt/issues) or [discussions](https://github.com/hugo-fixit/FixIt/discussions) tracker.

---

> This project was generated with [hugo-fixit-blog-go](https://github.com/hugo-fixit/hugo-fixit-blog-go). Documentation about the original structure can be found [here](https://github.com/hugo-fixit/hugo-fixit-blog-go#directory-structure).
