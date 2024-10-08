# TypeScript Decision Making Cheat Sheet

## if Statement

Basic syntax:
```typescript
if (condition) {
    // code to execute if condition is true
}
````

With else:
````typescript
if (condition) {
    // code to execute if condition is true
} else {
    // code to execute if condition is false
}
````

Multiple conditions:
````typescript
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
````typescript
let result = condition ? valueIfTrue : valueIfFalse;
````

## switch Statement

For multiple branching based on a value:
````typescript
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
````typescript
let result = someValue ?? defaultValue;
````

## Optional Chaining Operator (?.)

For safe property access:
````typescript
let value = obj?.property?.nestedProperty;
````

## Type Guards

Using typeof:
````typescript
if (typeof variable === "string") {
    // variable is treated as a string in this block
}
````

Using instanceof:
````typescript
if (variable instanceof ClassName) {
    // variable is treated as an instance of ClassName in this block
}
````

Custom type guard:
````typescript
function isString(value: any): value is string {
    return typeof value === "string";
}

if (isString(variable)) {
    // variable is treated as a string in this block
}
````

## Discriminated Unions

For type-safe handling of different shapes:
````typescript
type Shape = 
    | { kind: "circle"; radius: number }
    | { kind: "rectangle"; width: number; height: number };

function area(shape: Shape): number {
    switch (shape.kind) {
        case "circle":
            return Math.PI * shape.radius ** 2;
        case "rectangle":
            return shape.width * shape.height;
    }
}
````

## Assertion Functions

For runtime type checks:
````typescript
function assertIsString(value: any): asserts value is string {
    if (typeof value !== "string") {
        throw new Error("Value is not a string");
    }
}

function processString(value: any) {
    assertIsString(value);
    // value is treated as a string after the assertion
    console.log(value.toUpperCase());
}
````

Remember, TypeScript provides compile-time type checking, but these decision-making constructs allow for runtime type checking and control flow based on types and values.
```

