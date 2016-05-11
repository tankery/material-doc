---
layout: doc
title: How to Use
permalink: /docs/usage/

---

Here is a introduction for how to use the [Material Doc][material-doc].

## Installation

[Material Doc][material-doc] is a Jekyll powered site, with can be host directly on [GitHub Pages][github-pages].

Al things you need to do is to [fork][material-doc-code] this Project. Then you can visit your own site on `http://<username>.github.io/material-doc/`.

Anything you can on branch `gh-pages` will be displayed on your site.

For more details about site hosting (eg. Change site name, use your own domain, etc.) visit [GitHub Pages][github-pages].

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


## Custom Theme

## Develop

[material-doc]: http://tankery.github.io/material-doc/
[material-doc-code]: https://github.com/tankery/material-doc
[github-pages]: https://pages.github.com/
