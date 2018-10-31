---
layout: post
title:  "Preprocessors"
date:   2018-07-26 17:16:51 -0400
categories: bookiza templates new project
---

Bookiza supports multiple flavors. 

Write your book using MarkDown, HAML (recommend), PUG, SASS, LESS, STYLUS or just plain HTML, CSS and JavaScript. You can choose different combinations for different books, and vary preprocessing pipeline at page-level. 

### Configuring Preprocessors:

There are two ways to choose preprocessing (or none) for your Superbooks:

1. Globally, using ArcBookiza `mode` i.e. property on `.bookizarc` object called `mode`, or
2. Locally, per Superbook, using the `.bookrc` `mode` object.


## Adopting preprocessors using .bookrc mode.

```json
{
  "mode": {
    "HTML": "haml",
    "CSS": "scss",
    "JS": "js",
    "HEAD": "html"
  },
  "name": "Bookiza Documentation",
  "type": "text",
  "book_id": 167
}
```


For example, this [sample book](https://github.com/marvindanig/bookiza-framework) uses `.haml` and `.scss` instead of plain html and css.

Configuring bookiza will set its `generators` and `renderers` to use the appropriate templating engine (or preprocessor) for its pages (and templates). You can also use a combination of preprocessors within the same book with a more complicated setup (discussed elsewhere). 

By default Bookiza is configured for the native web i.e. plain HTML, CSS and JavaScript. The output of the build is always HTML, CSS and JavaScript as well no matter what preprocessor logic or transformations are applied beforehand. 
