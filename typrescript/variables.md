# TypeScript Variables Cheat Sheet

## Variable Declarations

### `let`
- Block-scoped
- Can be reassigned
```typescript
let x = 10;
x = 20;
```

### `const`
- Block-scoped
- Cannot be reassigned
```typescript
const PI = 3.14159;
PI = 3.14; // Error
```

### `var` (not recommended)
- Function-scoped
- Can be reassigned
```typescript
var y = 30;
y = 40; // OK
```

## Type Annotations

### Basic Types
```typescript
let name: string = "John";
let age: number = 30;
let isStudent: boolean = true;
let hobbies: string[] = ["reading", "coding"];
let tuple: [string, number] = ["apple", 5];
```
### Union Types
```typescript
let value: string | number = "Hello";
value = 10; // OK
```

### Type Inference
```typescript
let num = 10; // TypeScript infers type as number
let str = "Hello"; // TypeScript infers type as string
```

## `any` and `unknown` Types

### `any`
- Opt-out of type checking
```typescript
let anything: any = "Hello";
anything = 10; // OK
```

### `unknown`
- More restrictive than `any`
- Requires type checking before use
```typescript
et unknownValue: unknown = 4;
unknownValue = "string"; // OK
// unknownValue.toUpperCase(); // Error: Object is of type 'unknown'
```

