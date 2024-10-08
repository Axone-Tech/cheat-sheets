# TypeScript Operators Cheat Sheet

## Arithmetic Operators

| Operator | Description           | Example     |
|----------|-----------------------|-------------|
| `+`      | Addition              | `a + b`     |
| `-`      | Subtraction           | `a - b`     |
| `*`      | Multiplication        | `a * b`     |
| `/`      | Division              | `a / b`     |
| `%`      | Modulus (Remainder)   | `a % b`     |
| `**`     | Exponentiation        | `a ** b`    |
| `++`     | Increment             | `a++` or `++a` |
| `--`     | Decrement             | `a--` or `--a` |

## Comparison Operators

| Operator | Description           | Example     |
|----------|-----------------------|-------------|
| `==`     | Equal to              | `a == b`    |
| `===`    | Strict equal to       | `a === b`   |
| `!=`     | Not equal to          | `a != b`    |
| `!==`    | Strict not equal to   | `a !== b`   |
| `>`      | Greater than          | `a > b`     |
| `<`      | Less than             | `a < b`     |
| `>=`     | Greater than or equal to | `a >= b`    |
| `<=`     | Less than or equal to | `a <= b`    |

## Logical Operators

| Operator | Description           | Example     |
|----------|-----------------------|-------------|
| `&&`     | Logical AND           | `a && b`    |
| `||`     | Logical OR            | `a || b`    |
| `!`      | Logical NOT           | `!a`        |

## Assignment Operators

| Operator | Description           | Example     |
|----------|-----------------------|-------------|
| `=`      | Assignment            | `a = b`     |
| `+=`     | Addition assignment   | `a += b`    |
| `-=`     | Subtraction assignment| `a -= b`    |
| `*=`     | Multiplication assignment | `a *= b`    |
| `/=`     | Division assignment   | `a /= b`    |
| `%=`     | Modulus assignment    | `a %= b`    |
| `**=`    | Exponentiation assignment | `a **= b`   |

## Bitwise Operators

| Operator | Description           | Example     |
|----------|-----------------------|-------------|
| `&`      | Bitwise AND           | `a & b`     |
| `|`      | Bitwise OR            | `a | b`     |
| `^`      | Bitwise XOR           | `a ^ b`     |
| `~`      | Bitwise NOT           | `~a`        |
| `<<`     | Left shift            | `a << b`    |
| `>>`     | Sign-propagating right shift | `a >> b`    |
| `>>>`    | Zero-fill right shift | `a >>> b`   |

## Conditional (Ternary) Operator

```typescript
condition ? expressionIfTrue : expressionIfFalse
```

## Nullish Coalescing Operator

```typescript
a ?? b
// Returns 'a' if it's not null/undefined, otherwise 'b'
```

## Optional Chaining Operator

```typescript
obj?.prop
obj?.[expr]
func?.()
// Accesses an object's property or calls a function safely
```

## Type Operators

```typescript
typeof v // Returns a string indicating the type of v
v instanceof F // Checks if v is an instance of F
```

## Type Assertion Operators

```typescript
<Type>value // Angle-bracket syntax
value as Type // as-syntax (preferred)
```

## Non-null Assertion Operator

```typescript
identifier! // Asserts that identifier is non-null and non-undefined
```

## Index Signature Operator

```typescript
interface StringArray {
  [index: number]: string;
}
```

## Spread Operator

```typescript
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5]; // [1, 2, 3, 4, 5]
```

## Rest Operator

```typescript
function sum(...numbers: number[]): number {
  return numbers.reduce((total, num) => total + num, 0);
}
```

TypeScript includes all JavaScript operators and adds some TypeScript-specific operators for type handling and null safety.