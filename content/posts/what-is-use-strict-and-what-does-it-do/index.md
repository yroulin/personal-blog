---
title: "JS - What Is Use Strict and What Does It Do"
date: 2019-09-23T22:34:52-06:00
draft: false
categories: ["JS"]
resources:
- name: featuredImage
  src: "js.jpg"
  params: "JavaScript logo"
---

The keyword <strong>'use strict'</strong> means that the JavaScript engine will be pickier about certain things we do when we write code.


It turns on the strict mode operating context wherever you place it (inside of a function will activate strict mode on the function level scope) including:

* Using a variable before it’s defined now causes an error.
* It stops you from using words that are reserved for future versions of JS.
* You cannot delete functions, variables or functions arguments in  “use strict” mode
* Makes eval a bit safer to use (doesn’t let variables escape)
* So, in strict mode, if <strong>this</strong> was not defined by the execution context, it remains <span style="color: #f92672">undefined</span>.
