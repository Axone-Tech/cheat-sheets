# TypeScript Loops Cheat Sheet

## for Loop

Basic syntax:
```typescript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
````

Loop with step value:
````typescript
for (let i = 0; i < 10; i += 2) {
    console.log(i);
}
````

## while Loop

Basic syntax:
````typescript
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}
````

## do...while Loop

Basic syntax:
````typescript
let i = 0;
do {
    console.log(i);
    i++;
} while (i < 5);
````

## for...of Loop

Iterating over arrays or other iterable objects:
````typescript
let arr: number[] = [1, 2, 3, 4, 5];
for (let value of arr) {
    console.log(value);
}
````

## for...in Loop

Iterating over object properties:
````typescript
let obj = { a: 1, b: 2, c: 3 };
for (let key in obj) {
    console.log(key, obj[key]);
}
````

## forEach Method (for Arrays)

Using arrow function:
````typescript
let arr: number[] = [1, 2, 3, 4, 5];
arr.forEach((value, index) => {
    console.log(index, value);
});
````

## map Method (for Arrays)

Creating a new array based on the original:
````typescript
let arr: number[] = [1, 2, 3, 4, 5];
let doubled: number[] = arr.map(value => value * 2);
````

## filter Method (for Arrays)

Creating a new array with elements that pass a test:
````typescript
let arr: number[] = [1, 2, 3, 4, 5];
let evens: number[] = arr.filter(value => value % 2 === 0);
````

## reduce Method (for Arrays)

Reducing an array to a single value:
````typescript
let arr: number[] = [1, 2, 3, 4, 5];
let sum: number = arr.reduce((acc, value) => acc + value, 0);
````

## Breaking and Continuing

Using break:
````typescript
for (let i = 0; i < 5; i++) {
    if (i === 3) break;
    console.log(i);
}
````

Using continue:
````typescript
for (let i = 0; i < 5; i++) {
    if (i === 2) continue;
    console.log(i);
}
````

## Labeled Statements

Using labels with break:
````typescript
outerLoop: for (let i = 0; i < 3; i++) {
    for (let j = 0; j < 3; j++) {
        if (i === 1 && j === 1) break outerLoop;
        console.log(i, j);
    }
}
````

Remember, TypeScript provides type checking for your loops, ensuring type safety when working with arrays and objects. Always consider using appropriate types for your loop variables and iterated elements.
```

