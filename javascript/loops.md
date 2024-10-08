# JavaScript Loops Cheat Sheet

## for Loop

Basic syntax:
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
````

Loop with step value:
````javascript
for (let i = 0; i < 10; i += 2) {
    console.log(i);
}
````

## while Loop

Basic syntax:
````javascript
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}
````

## do...while Loop

Basic syntax:
````javascript
let i = 0;
do {
    console.log(i);
    i++;
} while (i < 5);
````

## for...of Loop

Iterating over arrays or other iterable objects:
````javascript
let arr = [1, 2, 3, 4, 5];
for (let value of arr) {
    console.log(value);
}
````

## for...in Loop

Iterating over object properties:
````javascript
let obj = { a: 1, b: 2, c: 3 };
for (let key in obj) {
    console.log(key, obj[key]);
}
````

## forEach Method (for Arrays)

Using arrow function:
````javascript
let arr = [1, 2, 3, 4, 5];
arr.forEach((value, index) => {
    console.log(index, value);
});
````

## map Method (for Arrays)

Creating a new array based on the original:
````javascript
let arr = [1, 2, 3, 4, 5];
let doubled = arr.map(value => value * 2);
````

## filter Method (for Arrays)

Creating a new array with elements that pass a test:
````javascript
let arr = [1, 2, 3, 4, 5];
let evens = arr.filter(value => value % 2 === 0);
````

## reduce Method (for Arrays)

Reducing an array to a single value:
````javascript
let arr = [1, 2, 3, 4, 5];
let sum = arr.reduce((acc, value) => acc + value, 0);
````

## Breaking and Continuing

Using break:
````javascript
for (let i = 0; i < 5; i++) {
    if (i === 3) break;
    console.log(i);
}
````

Using continue:
````javascript
for (let i = 0; i < 5; i++) {
    if (i === 2) continue;
    console.log(i);
}
````

## Labeled Statements

Using labels with break:
````javascript
outerLoop: for (let i = 0; i < 3; i++) {
    for (let j = 0; j < 3; j++) {
        if (i === 1 && j === 1) break outerLoop;
        console.log(i, j);
    }
}
````

## for...await...of Loop (for async iteration)

Iterating over async iterable objects:
````javascript
async function* asyncGenerator() {
    yield 1;
    yield 2;
    yield 3;
}

(async () => {
    for await (let value of asyncGenerator()) {
        console.log(value);
    }
})();
````

Remember, JavaScript is dynamically typed, so be cautious when working with different data types in loops. Always consider potential type coercion and unexpected behavior when looping through mixed data structures.
``````

This cheat sheet covers various looping constructs in JavaScript, including traditional loops, array methods, and modern JavaScript features like `for...of` and async iteration.
`````
