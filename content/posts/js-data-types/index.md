---
title: "JS - Data Types"
date: 2019-09-27T14:06:25-06:00
draft: false
categories: ["JS"]
dropCap: false
resources:
- name: featuredImage
  src: "js.jpg"
  params: "JavaScript logo"
---

JavaScript has 8 built-in data types (with the latest ECMAScript standard):

* We have the **Primitives** ones: 
    * Null 
    * Boolean
    * Undefined
    * Number
    * BigInt
    * String
    * Symbol

* and the **Objects**.

And you can check the type of each data type with the **[typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof)** operator:

```javascript
let helloMessage = "Hello World";
typeof(helloMessage); //Output: "string"

let myAge = 32;
typeof(myAge); //Output: "number"

const myPerson = {
    name: 'Yves',
    age: 32,
}
typeof(myPerson); //Output: "object"
```
 We have also have __undefined__ and __undeclared__ which is basically when you define a variable without a value (the default value is <span style="color: #f92672">**undefined**</span>). And __undeclared__ is just that the value hasn't been never declared.

<em>Useful Resources</em>:

* [MDN JS Data Structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
* [You Don't Know JS Yet: Types & Grammar Second Edition (WIP)](https://github.com/getify/You-Dont-Know-JS/tree/2nd-ed/types-grammar)