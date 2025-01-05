# Unexpected behavior of the `arguments` object in JavaScript

This example demonstrates the unexpected behavior of the `arguments` object in JavaScript. The `arguments` object is not an array, but it looks like one. It has a length property, and you can access elements by index. However, it does not have array methods like `map`, `filter`, or `reduce`. 

## Bug

The bug is that the `arguments` object is not an array and doesn't have array methods. This can lead to unexpected behavior if you try to use array methods on it. 

## Solution

The solution is to convert the `arguments` object into an array before using array methods on it. This can be done using the `Array.from()` method or the spread syntax.