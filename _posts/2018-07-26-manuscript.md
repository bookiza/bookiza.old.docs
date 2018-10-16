---
layout: post
title:  "Manuscript"
date:   2018-07-26 17:16:51 -0400
categories: bookiza manuscript project
---

Managing your manuscript

```
$ bookiza new MY-AWESOME-BOOK -l 12 -t comics   # Creates project with 12 fresh leafs (24 pages) inside `manuscript/`.
$ cd MY-AWESOME-BOOK

$ bookiza server            # Opens http://localhost:4567 on your browser!

```

To initialize a `new` project (book, comics, magazine or blank) with exactly `2N` number of pages pass the `--leafs` option with value `N` and a `--template` option if required. Like so:

`$ bookiza new MY-AWESOME-BOOK-TITLE --leafs 2N --template comics` where N is number of leafs.

Bookiza's `new` command will set up your project, bootstrap the manuscript (leafs) along with necessary configurations and apply the layout template you passed along in the options (if any). Bookiza will also *npm install* all the dependencies your project will need, *git initialize* the project and then seek confirmation from you to check-it into Github.

Inside the `manuscript/` folder you'll find that `2N` number of blank pages, the place where you'll be spending maximum of your time writing. 
