---
author: "makovako"
title: "PaperMode cheatheet"
date: "2021-08-26"
description: "Cheatsheet of features from PaperMod theme, which I use for this blog."
summary: "Cheatsheet of features from PaperMod theme, which I use for this blog."
categories: ["general"]
tags: ["cheatsheet", "hugo", "papermod"]
---

After a long time searching for the right theme for my blog, with the right set of features, I decided to use the PaperMod theme. This decision also picked the hugo SSG[^1] for me. I was okay with any, but I already have some experience with hugo, so it might be easier for me to customize it, if there is something I am not satisfied with.

[^1]: SSG - static site generator. You provide content, it generates the site from it. A static site already rendered. You don't need the server for site generation, you just need it for file serving.

Each theme comes with its own set of features. I will mention some of them there, so I don't have to look to the original source each time I want to do something special.

## Cover image

Displays on top of the page and in the posts list.

```yml
cover:
    image: "<image path/url>"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
```

## Post front matter

```yml
author: "makovako"
title: "Some title"
date: "2021-08-25"
description: "Some description" # what will be shown below title
summary: "Some summary" # what will be shown in posts list
categories: ["category1"] # list of categories
series: ["series1"] # list of series
tags: ["tag1"] # list of tags
draft: true # mark as draft
ShowBreadCrumbs: true # show page navigation
ShowToc: true # show table of content on page
TocOpen: true # open table of content by default
searchHidden: true # hide from search
ShowPostNavLinks: true # show prev/next article
ShowReadingTime: true # show reading time on page
weight: X # for ordering posts
```

## Access keys

```yml
c - ToC Open/Close
g - Go To Top
h - Home (according to current lang)
t - Theme toggle
/ - Jumps to search page if in menu
```

## Pin post

Add `weight=X` to page.

## Rich content

### YouTube

```
{{</* youtube ZJthWmvUzzc */>}}
```

### Twitter

```
{{</* twitter_simple 1085870671291310081 */>}}
```

### Vimeo

```
{{</* vimeo_simple 48912912 */>}}
```