# Hugo FixIt Blog Template (Go)

👉 English | [简体中文](README.md)

This is a quick start template for Hugo theme [FixIt](https://github.com/hugo-fixit/FixIt). It uses [Hugo Modules](https://gohugo.io/hugo-modules/) feature to load the theme. If you favor Git more, you can [check this template](https://github.com/hugo-fixit/hugo-fixit-starter1).

It comes with a basic theme structure and configuration. GitHub action has been set up to deploy the blog to a public GitHub page automatically. Also, there's a cron job to update the theme automatically everyday.

## Directory structure

```bash
▸ .github/       # GitHub configuration
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

For a complete quick start, see this [page](https://fixit.lruihao.cn/documentation/getting-started/).

### Prerequisites

- [Go](https://go.dev/dl/)
- [Hugo](https://gohugo.io/installation/) (extended version)

### Use Template

#### CLI

```bash
npx fixit-cli create my-blog
```

#### Manual

1. Click [**Use this template**](https://github.com/hugo-fixit/hugo-fixit-starter/generate), and create your repository on GitHub.

    <img width="913" alt="image" src="https://github.com/hugo-fixit/hugo-fixit-starter1/assets/33419593/d5fbd940-3ffd-4750-b1e6-4e87b50b0696">

2. Once the repository is created, just clone and enjoy it!

    ```bash
    # Clone with your own repository url
    git clone --recursive https://github.com/<your_name>/<your_blog_repo>.git
    ```

> [!TIP]
> The repository name determines your GitHub Pages URL, for example:
>
> | Repository Name | GitHub Pages |
> | :--- | :--- |
> | `<your_name>.github.io` | `https://<your_name>.github.io/` |
> | `blog` | `https://<your_name>.github.io/blog/` |

### Launching the Site

```bash
# Development environment
hugo server
# Production environment
hugo server -e production
```

### Build the Site

When your site is ready to deploy, run the following command:

```bash
hugo
```

### Deploy to GitHub Pages

> [!NOTE]
> You may have noticed that the first automatic deployment of GitHub Actions after the template initialization failed. This is because you have not configured Workflow permissions and GitHub Pages.

1. Head to Setting => Actions => General => Workflow permissions => Check "Read and write permissions".
2. GitHub Pages settings: Setting => Pages => Source: GitHub Actions.
3. Modify `config/_default/hugo.toml` file `baseURL` to your site URL.
4. Commit the changes from the previous step to the `main` branch, and GitHub Actions will automatically build and deploy the site to GitHub Pages.

### Update Theme

Afterwards you can upgrade the theme with the following command:

```bash
# Update theme manually
hugo mod get -u github.com/hugo-fixit/FixIt@latest
hugo mod tidy
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

## Troubleshooting

<details>
  <summary>remote: Permission to git denied to github-actions[bot].</summary>
  Head to Setting => Actions => General => Workflow permissions => Check "Read and write permissions".
</details>

<!-- This project was generated with [hugo-fixit-starter](https://github.com/hugo-fixit/hugo-fixit-starter). -->
