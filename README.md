# Blog setup for marcusmaximus.ca/blog

This folder contains a complete Jekyll blog that matches your site's design (cream/espresso,
your fonts, light/dark toggle). GitHub Pages runs Jekyll automatically — once these files are
in your repo, you publish a post just by adding a Markdown file and pushing.

## One-time setup

Copy these items into the **root of your `personal-website` repo** (same level as `index.html`):

```
_config.yml
_layouts/base.html
_layouts/post.html
_posts/2026-06-13-why-im-building-mezzo.md
blog/index.html
```

Your existing `index.html`, `og.png`, `CNAME`, and résumé stay exactly where they are and are
left untouched — Jekyll copies your hand-built homepage through verbatim.

Commit and push to `main`. GitHub Pages will build the site (takes ~1 minute). Then visit:

- **marcusmaximus.ca/blog** — the post list
- **marcusmaximus.ca/blog/why-im-building-mezzo/** — the example post

(If GitHub asks, make sure Settings → Pages → Build and deployment → Source is **"Deploy from a
branch"**, branch `main`, folder `/ (root)`. That's the default.)

## Publishing a new post (every time)

1. Create a file in `_posts/` named `YYYY-MM-DD-some-title.md` — the date and title matter.
2. Start it with this header (called "front matter"):

```
---
layout: post
title: "Your post title"
date: 2026-07-01
tags: [product, finance]
read: "4 min read"
excerpt: "One sentence that shows up in the post list and link previews."
---
```

3. Write the body below the header in plain Markdown (`## Heading`, `**bold**`, `[links](url)`, lists, etc.).
4. Commit and push. The post appears at `marcusmaximus.ca/blog/your-title/` and on the `/blog` list automatically — sorted newest first.

## Adding images

Put an image in an `assets/` folder in your repo, then reference it in a post:

```
![Description](/assets/my-screenshot.png)
```

## Linking the blog from your homepage

Your homepage nav menu can point to `/blog`. Tell me and I'll add a "Writing" link to the
dropdown so it's reachable from the main site.

## Tips

- Want to draft without publishing? Add `published: false` to the front matter.
- The blog shares your light/dark choice with the main site (same `localStorage` key).
- Delete the example post in `_posts/` whenever you like.
