---
title: "JS - Pass by Value or by Reference"
date: 2021-03-20T22:42:04-06:00
draft: false
dropCap: false
categories: ["JS"]
resources:
- name: featuredImage
  src: "js.jpg"
  params: "JavaScript logo"
---

Primitives types such as: Strings, numbers, boolean, undefined, null and symbol (ES6) are passed by **value** (You are passing a **COPY**) 

All objects (including functions, because yes, functions are objects) are passed by **Reference** (Something that points to the real object (same memory space))

Passing by value:
```bash
"use strict"
let a = 1;
function foo(a) {
    a = 2;
}

foo();
console.log(a);
Output: 1;
```

Passing by reference:

```bash
"use strict"
let c = { greeting: 'hi' };
let d;

d = c;
c.greeting = 'hello';
console.log(c);
console.log(d);

Output:
Object { greeting: "hello" }
Object { greeting: "hello" }
```

In JavaScript we can't change what A points to, we can only add a property or change a property. (That points to that particular memory space)


<em>Useful Resources</em>:

* [JavaScript: Understanding the Weird Parts - One of the best JS courses out there by Tony Alicea](https://www.udemy.com/course/understand-javascript/)
* [Understanding Immutability in JavaScript - CSS-Tricks](https://css-tricks.com/understanding-immutability-in-javascript/)