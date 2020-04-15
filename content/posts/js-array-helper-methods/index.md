---
title: "Array.prototype.Helpers"
date: 2020-04-13T22:15:08-06:00
draft: false
categories: ["JS"]
dropCap: false
resources:
  - name: featuredImage
    src: "js-array.jpg"
    params: "JavaScript Array Image"
---

Array Helper Methods are very helpful when you need to manipulate your data stored in arrays. They make life much easier, so we should know them.

# forEach Helper

The forEach() function is used to iterates through all the entries of the array.

ES5 Example:

```
var colors = ['red','blue','green'];
```

```
<script>
colors.forEach(function(color){
    console.log(color);
});
</script>
```

**Output**:

```
red
blue
green
```

ES6 Example:

```
<script>
colors.forEach(color => {
    console.log(color);
});
</script>
```

# Every Helper

The every() method tests whether **all** elements in the array pass the test implemented by the provided function, example: Check if all the values in the computers array are 16 or over:

Example:

```
const computers = [
  { name: 'Apple', ram: 24 },
  { name: 'Compaq', ram: 4 },
  { name: 'Acer', ram: 32 }
];
```

```
<script>
computers.every(computer => {
    return computer.ram > 16;
});
</script>
```

**Output**:

```
false
```

This returned false since not all the _computer.ram_ values are greater than 16.

# Some Helper

And the some() method tests whether **any** values in the computers array are 16 or over:

Example:

```
const computers = [
  { name: 'Apple', ram: 24 },
  { name: 'Compaq', ram: 4 },
  { name: 'Acer', ram: 32 }
];
```

```
<script>
computers.some(computer => {
    return computer.ram > 16;
});
</script>
```

**Output**:

```
true
```

This returned true because we have at least one _computer.ram_ value that is greater than 16.

# Filter Helper

Filters the list of fruits for those:

Example:

```
const products = [
  { name: 'cucumber', type: 'vegetable', quantity: 0, price: 1 },
  { name: 'banana', type: 'fruit', quantity: 10, price: 15 },
  { name: 'celery', type: 'vegetable', quantity: 30, price: 13 },
  { name: 'orange', type: 'fruit', quantity: 3, price: 5 }
];
```

```
<script>
let totalFruits = products.filter(fruit => {
    return product.type === 'fruit';
});
</script>
```

This will return all the _products_ that are type _fruit_, in this case **banana** and **orange**.

# Map Helper

The map() method is used to iterate through all the entries of the array, modifies them and returns a new array but the old array is not manipulated. Take in mind that the return keyword is mandatory.

Example:

```
const numbers = [1,2,3];
```

```
<script>
let doubled = numbers.map(number => {
    return number * 2;
});
</script>
```

**Output**:

```
console.log(numbers):
(3) [1, 2, 3]
console.log(doubled):
(3) [2, 4, 6]
```

# Reduce Helper

The reduce() method is used to compact all values in an array down to a single value.

This is a very basic example:

```
const bill = [39.85, 42.99, 49.99];
```

```
<script>
const sum = bill.reduce((total, amount) => {
    return total + amount;
});
</script>
```

**Output**:

```
132.83
```
