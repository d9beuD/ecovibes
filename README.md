# EcoVibes

Votre destination pour des produits durables et écologiques.

## Introduction

This project is an experimental blog hosted on GitHub Pages. It aims to introduce to readers sustainable products and display referral links to them. Once a product is bought, the site owner gets a fee.

If the SEO is optimized, images are attractive, the product doesn't suck and is well presented, readers should buy it. The received fee may pay for the custom domain name and eventually the social advertising.

## How to customize

If you want to try this adventure and clone (or fork) this repository, please think of changing the author name, the blog name and the theme colors.

### Change names

In the `_config.yml` file, you can change all information that can't fit your needs.

### Change colors

In the `./docs/_sass/_variables.scss` file, you can change theme SCSS variables.

```scss
$primary: #90c292;
$secondary: #e0eadf;
$success: #5cb85c;
$info: #a3d7ff;
$warning: #ffb347;
$danger: #f88379;
```

It should be sufficient for you, but feel free to adapt other variables if needed.

### Change Font Awesome kit

I included a pro [Font Awesome](https://fontawesome.com) license which is limited to domains of my own. You need to change it in the `default.html` layout.

## Run dev server

First you need to setup a [Jekyll environment](https://jekyllrb.com).

When you open the project, `cd` into `./docs` execute the following command:

```bash
bundle exec jekyll serve -H localhost -l --draft
```

Setting the host to `localhost` is required for your Font Awesome kit to work because the default `127.0.0.1` is not supported.

## Deploy

This repository contains a GitHub workflow in which you can find  the deployment script. Basically, it clones the repository, install Ruby and the project dependencies, build the website and commit changes to the `gh-pages` branch.

GitHub support the build process and deployment of the website without a workflow file, but it is limited to an old Jekyll version and a limited number of plugins. This workflow file bypass all limitations.

## Contribute

Found a typo? Think you can improve the website? Feel free to fork the project and make a pull request. Please, follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), name your branch verbosely and explain what you did in the pull request body.
