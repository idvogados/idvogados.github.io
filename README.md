# Idvogados

## Features

- [Live Search](https://github.com/thiagorossener/jekflix-template/wiki/Features#live-search)
- [Estimated Reading Time](https://github.com/thiagorossener/jekflix-template/wiki/Features#estimated-reading-time)
- [Reading Progress Bar](https://github.com/thiagorossener/jekflix-template/wiki/Features#reading-progress-bar) *(optional)*
- ["New Post" tag](https://github.com/thiagorossener/jekflix-template/wiki/Features#new-post-tag)
- [Load images on demand](https://github.com/thiagorossener/jekflix-template/wiki/Features#load-images-on-demand)
- [Push Menu](https://github.com/thiagorossener/jekflix-template/wiki/Features#push-menu)
- [SVG icons](https://github.com/thiagorossener/jekflix-template/wiki/Features#svg-icons)
- [Shell script to create posts](https://github.com/thiagorossener/jekflix-template/wiki/Features#shell-script-to-create-posts)
- [Tags page](https://github.com/thiagorossener/jekflix-template/wiki/Features#tags-page)
- [About page](https://github.com/thiagorossener/jekflix-template/wiki/Features#about-page)
- [Contact page](https://github.com/thiagorossener/jekflix-template/wiki/Features#contact-page)
- [404 error page](https://github.com/thiagorossener/jekflix-template/wiki/Features#404-error-page)
- [Feed RSS](https://github.com/thiagorossener/jekflix-template/wiki/Features#feed-rss)
- [Disqus](https://github.com/thiagorossener/jekflix-template/wiki/Features#disqus) *(optional)*
- [Featured post](https://github.com/thiagorossener/jekflix-template/wiki/Features#featured-post) *(optional)*
- [Home page pagination](https://github.com/thiagorossener/jekflix-template/wiki/Features#home-page-pagination) *(optional)*
- [Posts sidebar](https://github.com/thiagorossener/jekflix-template/wiki/Features#posts-sidebar) *(optional)*
- [Paginated posts](https://github.com/thiagorossener/jekflix-template/wiki/Features#paginated-posts) *(optional)*
- ["Before you go" modal](https://github.com/thiagorossener/jekflix-template/wiki/Features#before-you-go-modal) *(optional)*
- [Post recommendation](https://github.com/thiagorossener/jekflix-template/wiki/Features#post-recommendation)
- [Netlify CMS ready](https://github.com/thiagorossener/jekflix-template/wiki/Features#netlify-cms-ready)
- [Translations](https://github.com/thiagorossener/jekflix-template/wiki/setup#translations) **new!**
- [Math Expressions](https://github.com/thiagorossener/jekflix-template/wiki/Features#math-expressions) *(optional)* **new!**

## SEO

- Google Analytics
- Meta tags
- JSON-LD
- Sitemap.xml
- Social Media ready

### Site configuration

Below are some properties you can change in your project `_config.yml`, check the [documentation](https://github.com/thiagorossener/jekflix-template/wiki/settings) for more details.

```
# Site Settings
name: Idvogados
title: Idvogados
description: Plataforma gratuita conectando trabalhadores e advogados.
email: contato@idvogados.org
disqus_username: idvogados
link-anchor:
  - title: Home
    url: /
  - title: Blog
    url: /blog/
link-button:
  - title: Quero Colaborar
    url: /colabore/
link-footer:
  - title: Termos de Uso
    url: /termos-de-uso/
  - title: Imprint
    action: window.print()
copyrightYear: 2020

# Social Media Settings
# Remove the item if you don't need it
github_username: idvogados
facebook_username: idvogados
twitter_username: idvogados_ofc
instagram_username: idvogados.ofc
linkedin_username: idvogados

# Posts Settings
show_modal_on_exit: true


# Advanced Settings
baseurl: "" # the subpath of your site, e.g. /blog
url: "" # the base hostname & protocol for your site
google_analytics: "G-DTG3FDMY4V"
language: "pt-BR"


# Pagination Settings
paginate_path: "/page/:num/"
pagination:
  enabled: true
  per_page: 6
  permalink: '/page/:num/'
  title_suffix: ' - page :num'
  limit: 0
  sort_field: 'date'
  sort_reverse: true

# Build settings
# paginate: 5
markdown: kramdown
highlighter: rouge
permalink: /:title/
collections:
  authors:
    output: true
categories_folder: category

# SASS
sass:
  style: compressed

  
# Plugins
plugins:
  - jekyll-paginate-v2
  - jekyll-paginate-content

# Exclude my node related stuff
exclude: [
  'package.json',
  'package-lock.json',
  'src',
  'node_modules',
  'initpost.sh',
  'Gemfile',
  'Gemfile.lock',
  'gulpfile.js',
  'README.md'
]
```

## Setup

In the case you're cloning this repo, follow those instructions:

- [Environment](https://github.com/thiagorossener/jekflix-template/wiki/setup#environment)
- [Installing template](https://github.com/thiagorossener/jekflix-template/wiki/setup#installing-template)
- [Running local](https://github.com/thiagorossener/jekflix-template/wiki/setup#running-local)

### Customization

See the [settings documentation](https://github.com/thiagorossener/jekflix-template/wiki/settings) to customize layout, titles, social media and more.

### Theme

You can easily change the theme colors by changing the file `src/yml/theme.yml`, then running `gulp build` in your terminal.

#### GitHub pages

It's a known issue that you can't run Gulp when deploying the website into GitHub pages. So, you must change the theme colors and run `gulp build` locally, then push the changes into your repo, there is no other way.

To see how your website is going to look like when you deploy it, run `bundle exec jekyll serve` locally and access `http://127.0.0.1:4000/`.

## Posts

Use the [Front Matter properties](https://github.com/thiagorossener/jekflix-template/wiki/post#front-matter-properties) to create posts.

> **Note:** In the case you're cloning this repo, you can use the available [script](https://github.com/thiagorossener/jekflix-template/wiki/post#creating-a-post) to generate posts automatically.

## License

*Jekflix Template* is available under the MIT license. See the [LICENSE](https://github.com/thiagorossener/jekflix-template/blob/master/LICENSE) file for more info.
