# JavaScript Decision Making Cheat Sheet

## if Statement

Basic syntax:
```javascript
if (condition) {
    // code to execute if condition is true
}
````

With else:
````javascript
if (condition) {
    // code to execute if condition is true
} else {
    // code to execute if condition is false
}
````

Multiple conditions:
````javascript
if (condition1) {
    // code to execute if condition1 is true
} else if (condition2) {
    // code to execute if condition2 is true
} else {
    // code to execute if all conditions are false
}
````

## Ternary Operator

Shorthand for simple if-else statements:
````javascript
let result = condition ? valueIfTrue : valueIfFalse;
````

## switch Statement

For multiple branching based on a value:
````javascript
switch (expression) {
    case value1:
        // code to execute if expression === value1
        break;
    case value2:
        // code to execute if expression === value2
        break;
    default:
        // code to execute if no case matches
        break;
}
````

## Nullish Coalescing Operator (??)

For null or undefined checks:
````javascript
let result = someValue ?? defaultValue;
````

## Optional Chaining Operator (?.)

For safe property access:
````javascript
let value = obj?.property?.nestedProperty;
````

## Type Checking

Using typeof:
````javascript
if (typeof variable === "string") {
    // code to execute if variable is a string
}
````

Using instanceof:
````javascript
if (variable instanceof ClassName) {
    // code to execute if variable is an instance of ClassName
}
````

## Truthy and Falsy Checks

Implicit boolean conversion:
````javascript
if (value) {
    // code to execute if value is truthy
} else {
    // code to execute if value is falsy
}
````

## Short-circuit Evaluation

Using && for conditional execution:
````javascript
condition && executeFunction();
````

Using || for default values:
````javascript
let name = inputName || "Anonymous";
````

## try...catch Statement

For error handling:
````javascript
try {
    // code that might throw an error
} catch (error) {
    // code to handle the error
} finally {
    // code that will run regardless of whether an error occurred
}
````

## Conditional (Ternary) Operator with Short-circuit

For conditional assignment with a default:
````javascript
let result = condition && value;
````

Remember, JavaScript is a dynamically typed language, so type checking is done at runtime. Always consider type coercion and falsy values when making decisions in JavaScript.
`````

This cheat sheet covers various decision-making constructs in JavaScript, including traditional control flow statements, modern operators for null checking and safe property access, and JavaScript-specific practices like truthy/falsy checks and short-circuit evaluation.
`````
