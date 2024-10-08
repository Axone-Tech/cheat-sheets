# JavaScript Operators Cheat Sheet

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

```javascript
condition ? expressionIfTrue : expressionIfFalse
````


## Nullish Coalescing Operator

````javascript
a ?? b
// Returns 'a' if it's not null/undefined, otherwise 'b'
````


## Optional Chaining Operator

````javascript
obj?.prop
obj?.[expr]
func?.()
// Accesses an object's property or calls a function safely
````


## typeof Operator

````javascript
typeof operand
// Returns a string indicating the type of the operand
````


## instanceof Operator

````javascript
object instanceof constructor
// Tests whether the object has the constructor in its prototype chain
````


## Spread Operator

````javascript
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5]; // [1, 2, 3, 4, 5]
````


## Rest Operator

````javascript
function sum(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}
````


## Comma Operator

````javascript
let x = (2, 3);
// Returns 3
````


## delete Operator

````javascript
delete object.property
// Deletes an object's property
````


## in Operator

````javascript
'property' in object
// Returns true if the property is in the object or its prototype chain
````


## void Operator

````javascript
void expression
// Evaluates the expression and returns undefined
````


JavaScript is a dynamically typed language, so operators may behave differently based on the types of the operands. Always consider type coercion when using operators in JavaScript.