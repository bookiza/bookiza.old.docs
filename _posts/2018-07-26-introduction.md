---
layout: post
title:  "Introduction"
date:   2018-08-1 17:16:50 -0000
categories: jekyll update
---

Welcome to [Bookiza's](http://bookiza.io) official documentation. Bookiza is a *book reification tool* for the web. 

This site is also available as a [superbook](https://bubbl.in/cover/bookiza-framework-by-marvin-danig) (UPDATED!) if you prefer to read on a tablet. 


Literature provided below is OUTDATED as of August 10th, 2018. This project is in a great state of flux, the site will be updated in a few days. 

```html
<!-- Paste at { ~/project/templates/body.html } -->

<div class="page flex">
  <div class="inner justify ">
    <h1> Hello world! </h1>
    <p> Lorem ipsum... </p>
  </div>
</div>  
```

```css

/* Responsive layout and typography with viewport units */

@import url(https://fonts.googleapis.com/css?family=ABeeZee);

body {
  font: 6vw/1.0 'ABeeZee', sans-serif;
  overflow:hidden;
  background: white;
}

.page {
  height: 100vh;
  width: 80vw;
  margin: auto;
}

.inner {
  margin: 10vh auto;
  width: 100%;
  height:80vh;
}

.flex {
  display: -webkit-box;
  display: flex !important;
  align-items: center;
  justify-content: center;
}

.justify {
  text-align: justify;
}

/* Your custom styles below */

```

```javascript
// JS inside book is way cool
console.log('Hello world');
```

Bookiza is a *book reification framework* that cuts down your book writing and publishing time by half. By **half**, no less. It lets you manage your manuscript smartly and bakes in all the goodness of the web into your book.

Go ahead, produce delightful books that work everywhere (See [support](https://bubbl.in).

On the right you’ll find some sample code (plain ol’ HTML, CSS and JS) that makes for scalable responsive books. Or sometimes, food for thought. &#x1f344;  

<aside class="notice">
  Note bookiza uses the terminal environment (shell) to work. If you're uncomfortable about using shell commands or uncertain about what the terminal app is please consider using Bubblin's "in-browser" <a href="https://bubbl.in/tools">editor</a> instead. Here's a <a href="https://marvindanig.wordpress.com/2016/03/17/how-to-write-a-superbook/">blogpost</a> to start you there.
</aside>