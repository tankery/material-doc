---
layout: doc
title: How to Use
permalink: /docs/usage/

---

Here is a introduction for how to use the [Material Doc][material-doc].

## Installation

[Material Doc][material-doc] is a Jekyll powered site, with can be host directly on [GitHub Pages][github-pages].

All things you need to do is to [fork][material-doc-code] this Project. Then you can visit your own site on `http://<username>.github.io/material-doc/`.

Anything you can on branch `gh-pages` will be displayed on your site.

For more details about site hosting (eg. Change site name, use your own domain, etc.) visit [GitHub Pages][github-pages].


## Site configuration

Edit `_config.yml` to change the title, owner, description, social links, etc.

You can specific social links in footer of this site:

``` yml
socials:
  - name: github
    user: tankery
  - name: stack-overflow
    user: 1038900
```

Now we support following social account:

  github, twitter, weibo, google-plus, instagram, facebook, stack-overflow

To support more social links, edit url in `_data/socials.yml`. Remenber to always use a name that support by [Font Awesome Icons][font-awesome-icon], to make sure the icon is shown.


## Writing docs

Markdown is the language you can use to write the docs. A new doc can be add by following steps:

1. Write new docs with descriptions in header and put them to the folder  `_docs`.
2. Edit  `_data/docs.yml` to map your doc to navigation bar.

The header of doc is write like following:

```
---
layout: doc
title: How to Use
permalink: /docs/usage/
---
```

-  `layout` specific the page layout for different type of page. In most case, you should use  `doc` for your page.
-  `title` is the title displayed on top of page.
-  `permalink` can specific the link of this page. Make sure the link is started by  `/docs`, which is the root path of any docs. Path follow the  `/docs` is the key of this doc, that will be used to map the doc to the navigation bar in  `docs.yml`.

The config file `docs.yml` can controls structure of navigation bar. Elements in navigation including:

- `title`, to specific the category name.
- `docs`, to list docs key in category.


## Add new pages

Besides docs, you can add new pages also, all things you need to do is add a new Markdown file in any sub-folder of this site. Jekyll will find it out as a `page`, then Material Doc will add the pages to navigation below docs. See page ["About"](/about/) as a demo.

Checkout `_includes/site_pages.html` to see how it works.


## Custom Theme

Edit `_config.yml` to specific colors for the site palette:

``` yml
# Site styles
palette:
  primary: "#5c6bc0" # indigo, lighten-1
  secondary: "#7986cb" # indigo lighten-2
  tertiary: "#9fa8da" # indigo lighten-3
  colored_text: "#c5cae9" # indigo lighten-4
  highlight: "#f44336" # red
```

By using [SASS][sass-lang] (Syntactically Awesome Style Sheets), it is easy to change the style of hole site.
Whats more, If you using SVG, you can also change the color of logo when you customize the theme.


## Contribution

Feel free to post [issues][material-doc-issues] for this template, and [PR][material-doc-pr] is welcome.

[material-doc]: http://tankery.github.io/material-doc/
[material-doc-code]: https://github.com/tankery/material-doc
[material-doc-issues]: https://github.com/tankery/material-doc/issues
[material-doc-pr]: https://github.com/tankery/material-doc/pulls
[github-pages]: https://pages.github.com/
[font-awesome-icon]: http://fontawesome.io/icons/
[sass-lang]: http://sass-lang.com/
