## Status

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/BlackrockDigital/startbootstrap-simple-sidebar/master/LICENSE)
[![npm version](https://img.shields.io/npm/v/startbootstrap-simple-sidebar.svg)](https://www.npmjs.com/package/startbootstrap-simple-sidebar)
[![Build Status](https://travis-ci.org/BlackrockDigital/startbootstrap-simple-sidebar.svg?branch=master)](https://travis-ci.org/BlackrockDigital/startbootstrap-simple-sidebar)
[![dependencies Status](https://david-dm.org/BlackrockDigital/startbootstrap-simple-sidebar/status.svg)](https://david-dm.org/BlackrockDigital/startbootstrap-simple-sidebar)
[![devDependencies Status](https://david-dm.org/BlackrockDigital/startbootstrap-simple-sidebar/dev-status.svg)](https://david-dm.org/BlackrockDigital/startbootstrap-simple-sidebar?type=dev)


## How to write a new blog post

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


## Making changes to website

* Fork and clone the repo
* install npm and gulp via command line on your terminal
* Run `npm install` (you may get ~3 warnings but that is okay)
* Edit the HTML and CSS files included with the template in your favorite text editor to make changes. These are the only files you need to worry about, you can ignore everything else!
* Run `gulp dev` which will open up a preview of the template in your default browser, watch for changes to core template files, and live reload the browser when changes are saved.


You must have npm and Gulp installed globally on your machine in order to use these features.

## Colors:
Ada Bot Outline Blue - #39B7FC <br/>
Ada Bot inner Blue - #496E80


## Troubleshooting and Help

Email adasteam@ualberta.ca if you have questions!

## Bugs and Issues

See a bug? Open an issue on the repository!

## Copyright and License

Copyright 2013-2018 Blackrock Digital LLC. Code released under the [MIT](https://github.com/BlackrockDigital/startbootstrap-simple-sidebar/blob/gh-pages/LICENSE) license.
Copyright 2018 Ada's Team.
