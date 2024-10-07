# Hello World


Welcome to Hugo FixIt! This is your very first post.

&lt;!--more--&gt;

Head to the documentation page linked below for a complete guidence to get started with the [FixIt](https://github.com/hugo-fixit/FixIt) theme.

{{&lt; fixit-docs-bookmark &gt;}}

## Quick Start

For a complete quick start, see this [page](https://fixit.lruihao.cn/documentation/getting-started/).

### Prerequisites

- [Go](https://go.dev/dl/)
- [Hugo](https://gohugo.io/installation/): &gt;= 0.132.0 (extended version)

### Use this Template

1. Click [**Use this template**](https://github.com/hugo-fixit/hugo-fixit-starter/generate), and create your repository on GitHub.

    &lt;img width=&#34;913&#34; alt=&#34;image&#34; src=&#34;https://github.com/hugo-fixit/hugo-fixit-starter1/assets/33419593/d5fbd940-3ffd-4750-b1e6-4e87b50b0696&#34;&gt;

2. Once the repository is created, just clone and enjoy it!

    ```bash
    # Clone with your own repository url
    git clone --recursive https://github.com/&lt;your_name&gt;/&lt;your_blog_repo&gt;.git
    ```

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

### Update Theme

Afterwards you can upgrade the theme with the following command:

```bash
# Update theme manually
hugo mod get -u github.com/hugo-fixit/FixIt@latest
hugo mod tidy
```

&lt;details&gt;
  &lt;summary&gt;Start via NPM script&lt;/summary&gt;

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

&lt;/details&gt;

## Feedback

Whether it&#39;s questions, ideas, bugs or pull requests, all feedback is welcome!

Head over to the [issues](https://github.com/hugo-fixit/FixIt/issues) or [discussions](https://github.com/hugo-fixit/FixIt/discussions) tracker.


---

> Author: [Lruihao](https://github.com/Lruihao)  
> URL: https://hugo-fixit.github.io/hugo-fixit-starter/posts/hello-world/  

