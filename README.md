Jekyll templates
================

Atom 1.0 and RSS 2.0 templates for [Jekyll](https://github.com/mojombo/jekyll)
which pass [spec validation](http://validator.w3.org/feed/).

Feel free to copy.
[Licensed CC0](https://github.com/BigBlueHat/jekyll-feed-templates.git)

## Sample _config.yml

The `atom.xml` and `rss.xml` templates look for some extra site variables:
`author`, `email`, and `description`. Here's what that looks like in a
`_config.yml`:

```yaml
title: Fabulous Site
author: BigBlueHat
email: byoung@bigbluehat.com
description: Fabulous Site of fabulousness!
```

## _data/authors.yml

This file holds author data (shock...), and is used in the `rss.xml` file to
output email addresses of authors.

## Known Issues

There is a `/team/{{ post.author }}` URL in the `atom.xml`. It's a rash
assumption that this is where you will put your author pages. It should really
be configural. Patches welcome! :smiley_cat:
