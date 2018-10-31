---
layout: post
title:  "Structure"
date:   2018-07-26 17:16:51 -0400
categories: bookiza superbook pages leafs
---
Quick look into project structure here. 

Let's create a fresh barebones project `test`, something like this:

```

$ bookiza new test -l 4 -t comics

Initializing…  [ manuscript=abba | leafs=4 | template=comics ]
License.txt… :added.
.gitignoring /build /node_modules… :done.
README initialization… :success.
Applying a comics layout… :success.
Mobilizing crust… :success.
Server setup… :completed.
PackageJson configured… :standing by for installation.
Setting bookrc values… :done.
Generating [ 8 ] blank page(s)… : done.

…
…

Installed npm modules… :successfully.

Publish new repo as marvindanig/test? (Y/n)

// skip

```


```

$ cd test && ls -ltra

README.md         crust             node_modules        trash
assets            gulpfile.js       package-lock.json   .bookrc
build             license.txt       package.json        .gitignore
cover             manuscript        templates           .git

```

## Manuscript
As an author or maker, most of your time creating the book will be spent inside the `manuscript` folder. Here you'll see a directory for each page of the book with a number appended to its foldername, like so: `page-1`, `page-2`, `page-3`… and so on until page-2N. 

Inside each page directory, you'll find a file called `body.html` and `style.css`. Additionally, you can also add a `scripts.js` and `head.html` file inside each page if you need to apply additional components on your page. Bookiza will process and combine all the [components of a page](https://bubblin.io/docs/structure.html) and render it on your book.   

See how to use [preprocessors]({{ site.baseurl }}{% link _posts/2018-07-26-preprocessors.md %}) instead of plain markup and style by altering Bookiza's mode.



## Layout



## 

Using web fonts and typography from the web in your book.


## CDN resources

