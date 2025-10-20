# Number Methods in JavaScript

## What are Number Methods?

Number methods are built-in functions in JavaScript that help you work with numbers. Think of them as mathematical tools in a toolbox - each one does a specific job to help you calculate, format, convert, or check numbers.

Just like you might use a calculator to do math, or a ruler to measure things, number methods help you perform mathematical operations and manipulate numbers in your programs.

---

## Popular Number Methods

### 1. **toString()**
**What it does:** Converts a number to a string.

```javascript
let num = 123;
console.log(num.toString()); // Output: "123"
console.log(typeof num.toString()); // Output: "string"
```
*Like writing a number on paper - turns it into text.*

---

### 2. **toFixed()**
**What it does:** Formats a number to a specific number of decimal places.

```javascript
let price = 19.99999;
console.log(price.toFixed(2)); // Output: "20.00"
console.log(price.toFixed(0)); // Output: "20"
```
*Like rounding money to cents - controls how many decimal places you see.*

---

### 3. **toPrecision()**
**What it does:** Formats a number to a specific length (total digits).

```javascript
let num = 123.456;
console.log(num.toPrecision(4)); // Output: "123.5"
console.log(num.toPrecision(2)); // Output: "1.2e+2"
```
*Controls the total number of significant digits.*

---

### 4. **parseInt()**
**What it does:** Converts a string to a whole number (integer).

```javascript
console.log(parseInt("123")); // Output: 123
console.log(parseInt("123.45")); // Output: 123
console.log(parseInt("123abc")); // Output: 123
console.log(parseInt("abc123")); // Output: NaN
```
*Like removing everything after the decimal point and converting text to number.*

---

### 5. **parseFloat()**
**What it does:** Converts a string to a decimal number.

```javascript
console.log(parseFloat("123.45")); // Output: 123.45
console.log(parseFloat("123.45abc")); // Output: 123.45
console.log(parseFloat("abc123.45")); // Output: NaN
```
*Converts text to numbers, keeping decimal places.*

---

### 6. **Number()**
**What it does:** Converts a value to a number (strict conversion).

```javascript
console.log(Number("123")); // Output: 123
console.log(Number("123.45")); // Output: 123.45
console.log(Number("123abc")); // Output: NaN
console.log(Number(true)); // Output: 1
console.log(Number(false)); // Output: 0
```
*The strictest way to convert something to a number.*

---

### 7. **isNaN()**
**What it does:** Checks if a value is "Not a Number".

```javascript
console.log(isNaN(123)); // Output: false
console.log(isNaN("123")); // Output: false
console.log(isNaN("abc")); // Output: true
console.log(isNaN(NaN)); // Output: true
```
*Asks "Is this NOT a number?" - answers true or false.*

---

### 8. **Number.isInteger()**
**What it does:** Checks if a number is a whole number (no decimals).

```javascript
console.log(Number.isInteger(123)); // Output: true
console.log(Number.isInteger(123.45)); // Output: false
console.log(Number.isInteger(123.0)); // Output: true
```
*Checks if a number is whole (like 1, 2, 3) or has decimal parts.*

---

### 9. **Math.round()**
**What it does:** Rounds a number to the nearest whole number.

```javascript
console.log(Math.round(4.3)); // Output: 4
console.log(Math.round(4.7)); // Output: 5
console.log(Math.round(4.5)); // Output: 5
```
*Like normal rounding in math class - .5 and above goes up.*

---

### 10. **Math.floor()**
**What it does:** Rounds DOWN to the nearest whole number.

```javascript
console.log(Math.floor(4.9)); // Output: 4
console.log(Math.floor(4.1)); // Output: 4
console.log(Math.floor(-4.1)); // Output: -5
```
*Always rounds down, like dropping to the floor.*

---

### 11. **Math.ceil()**
**What it does:** Rounds UP to the nearest whole number.

```javascript
console.log(Math.ceil(4.1)); // Output: 5
console.log(Math.ceil(4.9)); // Output: 5
console.log(Math.ceil(-4.9)); // Output: -4
```
*Always rounds up, like reaching for the ceiling.*

---

### 12. **Math.abs()**
**What it does:** Returns the absolute value (always positive).

```javascript
console.log(Math.abs(-5)); // Output: 5
console.log(Math.abs(5)); // Output: 5
console.log(Math.abs(-3.14)); // Output: 3.14
```
*Removes the negative sign - makes everything positive.*

---

### 13. **Math.max()**
**What it does:** Finds the largest number from a group.

```javascript
console.log(Math.max(1, 5, 3, 9, 2)); // Output: 9
console.log(Math.max(10, 20)); // Output: 20
```
*Like finding the tallest person in a group.*

---

### 14. **Math.min()**
**What it does:** Finds the smallest number from a group.

```javascript
console.log(Math.min(1, 5, 3, 9, 2)); // Output: 1
console.log(Math.min(10, 20)); // Output: 10
```
*Like finding the shortest person in a group.*

---

### 15. **Math.pow()**
**What it does:** Raises a number to a power (exponent).

```javascript
console.log(Math.pow(2, 3)); // Output: 8 (2 × 2 × 2)
console.log(Math.pow(5, 2)); // Output: 25 (5 × 5)
```
*Like using the ** operator - multiplies a number by itself multiple times.*

---

### 16. **Math.sqrt()**
**What it does:** Finds the square root of a number.

```javascript
console.log(Math.sqrt(9)); // Output: 3
console.log(Math.sqrt(16)); // Output: 4
console.log(Math.sqrt(2)); // Output: 1.4142135623730951
```
*Finds what number multiplied by itself gives you the original number.*

---

### 17. **Math.random()**
**What it does:** Generates a random decimal number between 0 and 1.

```javascript
console.log(Math.random()); // Output: 0.7234567891234567 (random)
console.log(Math.random()); // Output: 0.1234567891234567 (different each time)

// Random number between 1 and 10
console.log(Math.floor(Math.random() * 10) + 1);
```
*Like rolling invisible dice - gives you a different number each time.*

---

### 18. **toExponential()**
**What it does:** Converts a number to exponential notation.

```javascript
let num = 123456;
console.log(num.toExponential(2)); // Output: "1.23e+5"
console.log(num.toExponential()); // Output: "1.23456e+5"
```
*Like scientific notation - useful for very large or very small numbers.*

---

## Quick Reference Table

| Method | What It Does | Example |
|--------|--------------|---------|
| `toString()` | Number to string | `(123).toString()` → "123" |
| `toFixed(n)` | Format decimals | `(19.99).toFixed(2)` → "20.00" |
| `parseInt(str)` | String to integer | `parseInt("123")` → 123 |
| `parseFloat(str)` | String to decimal | `parseFloat("123.45")` → 123.45 |
| `Number(value)` | Convert to number | `Number("123")` → 123 |
| `isNaN(value)` | Check if not a number | `isNaN("abc")` → true |
| `Math.round(n)` | Round to nearest | `Math.round(4.7)` → 5 |
| `Math.floor(n)` | Round down | `Math.floor(4.9)` → 4 |
| `Math.ceil(n)` | Round up | `Math.ceil(4.1)` → 5 |
| `Math.abs(n)` | Absolute value | `Math.abs(-5)` → 5 |
| `Math.max(a,b,c)` | Find largest | `Math.max(1,5,3)` → 5 |
| `Math.min(a,b,c)` | Find smallest | `Math.min(1,5,3)` → 1 |
| `Math.pow(base, exp)` | Power/exponent | `Math.pow(2,3)` → 8 |
| `Math.sqrt(n)` | Square root | `Math.sqrt(9)` → 3 |
| `Math.random()` | Random 0-1 | `Math.random()` → 0.234... |

---

## Important Notes

1. **NaN (Not a Number)** - Special value when math operations fail:
   ```javascript
   console.log(0/0); // NaN
   console.log(parseInt("hello")); // NaN
   console.log(Math.sqrt(-1)); // NaN
   ```

2. **Infinity** - Special value for numbers too large:
   ```javascript
   console.log(1/0); // Infinity
   console.log(-1/0); // -Infinity
   ```

3. **Floating point precision** - Decimal math can be imprecise:
   ```javascript
   console.log(0.1 + 0.2); // 0.30000000000000004
   console.log((0.1 + 0.2).toFixed(1)); // "0.3"
   ```

4. **Method vs Function** - Some are methods (used with numbers), some are functions:
   ```javascript
   // Methods (used with numbers)
   let num = 123;
   num.toString();
   
   // Functions (standalone)
   Math.round(123.45);
   parseInt("123");
   ```

---

## Practical Examples

### Currency Formatting
```javascript
let price = 19.99999;
console.log("$" + price.toFixed(2)); // Output: "$20.00"
```

### Random Number in Range
```javascript
// Random number between 1 and 100
let random = Math.floor(Math.random() * 100) + 1;
console.log(random);
```

### Input Validation
```javascript
let userInput = "25.5";
if (!isNaN(userInput)) {
    let age = parseFloat(userInput);
    console.log("Valid age: " + age);
} else {
    console.log("Please enter a valid number");
}
```

### Safe Division
```javascript
function safeDivide(a, b) {
    if (b === 0) {
        return "Cannot divide by zero";
    }
    return (a / b).toFixed(2);
}
console.log(safeDivide(10, 3)); // "3.33"
```

---

## Practice Exercise

Try these examples:
```javascript
let myNumber = 123.456789;

// 1. Round to 2 decimal places
console.log(myNumber.toFixed(2));

// 2. Round up to nearest whole number
console.log(Math.ceil(myNumber));

// 3. Convert to string
console.log(myNumber.toString());

// 4. Find square root
console.log(Math.sqrt(myNumber));

// 5. Generate random number 1-10
console.log(Math.floor(Math.random() * 10) + 1);

// 6. Check if it's an integer
console.log(Number.isInteger(myNumber));
```

Happy calculating! 🧮
