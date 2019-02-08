The blog is powered by [Jekyll](https://jekyllrb.com/).

To create a new post, make a new Markdown file in `_posts/` with
a filename following this pattern [(See Jekyll's
docs)](https://jekyllrb.com/docs/posts/#creating-posts):

    YYYY-MM-DD-title-slug.md

Where `YYYY` is the year, `MM` is the (zero-padded!) month, and `DD` is
the (zero-padded!) day of the month. This is the same as [ISO 8601][]
extended data format. `title-slug` is an all lowercase, hyphen-separated
version of the title. This will be in the URL, so make it good!

The Markdown file **must** start with YAML front-matter. Copy-paste the
following template!

```
---
layout: post
title: Hello, this is my title!
author: myusername
---

Hello, this is my blog post!
```

After the second `---`, write your blog post in regular Markdown. The
Markdown engine is called Kramdown, and it supports some [syntax
extensions](https://kramdown.gettalong.org/syntax.html).

Upon pushing/merging to `master`, the blog post will be automatically
generated on the site!

### Previewing changes locally

You must have Ruby installed (installed by default on macOS with Xcode installed).

Then, install the full package. You'll probably want to do something
involving [bundler](https://bundler.io/), but I honestly don't know what
that is or how to use it. Either way, with Ruby installed, install
GitHub's distribution of Jekyll and all of its approved plugins:

    gem install github-pages

Then, to run the development server, run the following:

    jekyll serve --watch

The local copy should be accessible at <http://localhost:4000/>!
Note, that while it regenerates the site when markdown posts, layouts,
and other static assets have changed, it **will not** regenerate the
site when `_config.yml` changes. Please restart the server if this is
the case.
