# Hugo FixIt Blog Template (Go)

This is a quick start template for Hugo theme [FixIt](https://github.com/hugo-fixit/FixIt). It uses [Hugo Modules](https://gohugo.io/hugo-modules/) feature to load the theme.

It comes with a basic theme structure and configuration. GitHub action has been set up to deploy the theme to a public GitHub page automatically. Also, there's a cron job to update the theme automatically everyday.

1. Click *Use this template*, and create your repository on GitHub.
2. Once the repository is created, just clone and enjoy it!

## Directory structure

```bash
▸ .github/       # GitHub configuration
▸ .shell/        # shell commands for hugo project, entrance: hugo_main.sh
▸ archetypes/    # page archetypes (like scaffolds of archetypes)
▸ assets/        # css, js, third-party libraries etc.
▸ config/        # configuration files
▸ content/       # markdown files for hugo project
▸ data/          # blog data (allow: yaml, json, toml), e.g. friends.yml
▸ public/        # build directory
▸ static/        # static files, e.g. favicon.ico
▸ themes/        # theme submodules
▸ go.mod
▸ go.sum
```

## Quick Start

Just install latest version of [Hugo(>= 0.89.0)](https://gohugo.io/installation/) for your OS (Windows, Linux, macOS).

```bash
# Clone with your own repository url
git clone --recursive git@github.com:hugo-fixit/hugo-fixit-blog-go.git
```

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
