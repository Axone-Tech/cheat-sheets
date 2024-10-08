# JavaScript Variables Cheat Sheet

## Variable Declarations

### `let`
- Block-scoped
- Can be reassigned
```javascript
let x = 10;
x = 20; // OK
```

### `const`
- Block-scoped
- Cannot be reassigned
```javascript
const PI = 3.14159;
// PI = 3.14; // Error
```

### `var` (not recommended)
- Function-scoped or globally-scoped
- Can be reassigned
```javascript
var y = 30;
y = 40; // OK
```

## Variable Types

JavaScript is dynamically typed, so variables can hold any type of value:

```javascript
let name = "John";
let age = 30;
let isStudent = true;
let hobbies = ["reading", "coding"];
```

## Type Coercion

JavaScript performs automatic type coercion:

```javascript
let num = 5;
let str = "10";
console.log(num + str); // Outputs: "510"
```

## Undefined and Null

```javascript
let undefinedVar;
console.log(undefinedVar); // Outputs: undefined

let nullVar = null;
console.log(nullVar); // Outputs: null
```
Remember, JavaScript is loosely typed, so variables can change types during runtime. Use consistent naming conventions and be mindful of scope to write clean, maintainable code!