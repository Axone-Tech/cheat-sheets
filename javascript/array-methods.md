# Array Methods in JavaScript

## What are Array Methods?

Array methods are built-in functions in JavaScript that help you work with lists (arrays). Think of them as tools for organizing, searching, and modifying collections of items - like having a magic toolbox for managing your shopping list, photo album, or any group of things.

Just like you might sort your clothes, add new items to a list, or find something specific in a drawer, array methods help you organize, add, remove, search, and transform collections of data in your programs.

---

## Popular Array Methods

### 1. **push()**
**What it does:** Adds one or more items to the end of an array.

```javascript
let fruits = ["apple", "banana"];
fruits.push("orange");
console.log(fruits); // Output: ["apple", "banana", "orange"]

fruits.push("grape", "kiwi");
console.log(fruits); // Output: ["apple", "banana", "orange", "grape", "kiwi"]
```
*Like adding items to the end of your shopping list.*

---

### 2. **pop()**
**What it does:** Removes and returns the last item from an array.

```javascript
let fruits = ["apple", "banana", "orange"];
let removed = fruits.pop();
console.log(removed); // Output: "orange"
console.log(fruits); // Output: ["apple", "banana"]
```
*Like taking the last item off your shopping list.*

---

### 3. **unshift()**
**What it does:** Adds one or more items to the beginning of an array.

```javascript
let fruits = ["banana", "orange"];
fruits.unshift("apple");
console.log(fruits); // Output: ["apple", "banana", "orange"]
```
*Like adding items to the top of your shopping list.*

---

### 4. **shift()**
**What it does:** Removes and returns the first item from an array.

```javascript
let fruits = ["apple", "banana", "orange"];
let removed = fruits.shift();
console.log(removed); // Output: "apple"
console.log(fruits); // Output: ["banana", "orange"]
```
*Like crossing off the first item on your shopping list.*

---

### 5. **length**
**What it does:** Tells you how many items are in an array.

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits.length); // Output: 3
```
*Like counting how many items are on your list.*

---

### 6. **indexOf()**
**What it does:** Finds the position of an item in the array.

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits.indexOf("banana")); // Output: 1
console.log(fruits.indexOf("grape")); // Output: -1 (not found)
```
*Like finding which position something is in your list. Returns -1 if not found.*

---

### 7. **includes()**
**What it does:** Checks if an array contains a specific item.

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits.includes("banana")); // Output: true
console.log(fruits.includes("grape")); // Output: false
```
*Like asking "Is this item on my list?" - answers yes (true) or no (false).*

---

### 8. **slice()**
**What it does:** Creates a copy of a part of an array.

```javascript
let fruits = ["apple", "banana", "orange", "grape"];
console.log(fruits.slice(1, 3)); // Output: ["banana", "orange"]
console.log(fruits.slice(2)); // Output: ["orange", "grape"]
console.log(fruits); // Original unchanged: ["apple", "banana", "orange", "grape"]
```
*Like photocopying a section of your list - doesn't change the original.*

---

### 9. **splice()**
**What it does:** Adds, removes, or replaces items in an array (changes the original).

```javascript
let fruits = ["apple", "banana", "orange"];

// Remove 1 item starting at index 1
fruits.splice(1, 1);
console.log(fruits); // Output: ["apple", "orange"]

// Add items at index 1
fruits.splice(1, 0, "grape", "kiwi");
console.log(fruits); // Output: ["apple", "grape", "kiwi", "orange"]
```
*Like editing your list - you can add, remove, or replace items anywhere.*

---

### 10. **join()**
**What it does:** Combines all array items into a single string.

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits.join()); // Output: "apple,banana,orange"
console.log(fruits.join(" - ")); // Output: "apple - banana - orange"
console.log(fruits.join("")); // Output: "applebananaorange"
```
*Like reading your list out loud with separators between items.*

---

### 11. **reverse()**
**What it does:** Reverses the order of items in an array.

```javascript
let numbers = [1, 2, 3, 4];
numbers.reverse();
console.log(numbers); // Output: [4, 3, 2, 1]
```
*Like flipping your list upside down - last becomes first.*

---

### 12. **sort()**
**What it does:** Sorts array items in alphabetical/numerical order.

```javascript
let fruits = ["orange", "apple", "banana"];
fruits.sort();
console.log(fruits); // Output: ["apple", "banana", "orange"]

let numbers = [3, 1, 4, 1, 5];
numbers.sort((a, b) => a - b); // For proper number sorting
console.log(numbers); // Output: [1, 1, 3, 4, 5]
```
*Like organizing your list alphabetically or numerically.*

---

### 13. **concat()**
**What it does:** Combines two or more arrays into a new array.

```javascript
let fruits = ["apple", "banana"];
let vegetables = ["carrot", "lettuce"];
let food = fruits.concat(vegetables);
console.log(food); // Output: ["apple", "banana", "carrot", "lettuce"]
```
*Like stapling two lists together to make one bigger list.*

---

### 14. **forEach()**
**What it does:** Runs a function for each item in the array.

```javascript
let fruits = ["apple", "banana", "orange"];
fruits.forEach(function(fruit, index) {
    console.log(index + ": " + fruit);
});
// Output:
// 0: apple
// 1: banana
// 2: orange
```
*Like going through your list item by item and doing something with each one.*

---

### 15. **map()**
**What it does:** Creates a new array by transforming each item.

```javascript
let numbers = [1, 2, 3, 4];
let doubled = numbers.map(function(num) {
    return num * 2;
});
console.log(doubled); // Output: [2, 4, 6, 8]
console.log(numbers); // Original unchanged: [1, 2, 3, 4]
```
*Like making a new list where each item is changed in some way.*

---

### 16. **filter()**
**What it does:** Creates a new array with only items that pass a test.

```javascript
let numbers = [1, 2, 3, 4, 5, 6];
let evenNumbers = numbers.filter(function(num) {
    return num % 2 === 0;
});
console.log(evenNumbers); // Output: [2, 4, 6]
```
*Like making a new list with only the items that meet your criteria.*

---

### 17. **find()**
**What it does:** Returns the first item that passes a test.

```javascript
let numbers = [1, 2, 3, 4, 5];
let found = numbers.find(function(num) {
    return num > 3;
});
console.log(found); // Output: 4
```
*Like finding the first item on your list that matches what you're looking for.*

---

### 18. **reduce()**
**What it does:** Reduces an array to a single value by combining all items.

```javascript
let numbers = [1, 2, 3, 4];
let sum = numbers.reduce(function(total, num) {
    return total + num;
}, 0);
console.log(sum); // Output: 10

// Or with arrow function
let sum2 = numbers.reduce((total, num) => total + num, 0);
```
*Like adding up all the numbers on your list to get a total.*

---

### 19. **some()**
**What it does:** Checks if at least one item passes a test.

```javascript
let numbers = [1, 2, 3, 4, 5];
let hasEven = numbers.some(function(num) {
    return num % 2 === 0;
});
console.log(hasEven); // Output: true
```
*Like asking "Does at least one item on my list meet this condition?"*

---

### 20. **every()**
**What it does:** Checks if all items pass a test.

```javascript
let numbers = [2, 4, 6, 8];
let allEven = numbers.every(function(num) {
    return num % 2 === 0;
});
console.log(allEven); // Output: true
```
*Like asking "Do ALL items on my list meet this condition?"*

---

## Quick Reference Table

| Method | What It Does | Changes Original? | Example |
|--------|--------------|-------------------|---------|
| `push(item)` | Add to end | Yes | `arr.push("new")` |
| `pop()` | Remove from end | Yes | `arr.pop()` |
| `unshift(item)` | Add to start | Yes | `arr.unshift("new")` |
| `shift()` | Remove from start | Yes | `arr.shift()` |
| `length` | Count items | No | `arr.length` |
| `indexOf(item)` | Find position | No | `arr.indexOf("apple")` |
| `includes(item)` | Check if contains | No | `arr.includes("apple")` |
| `slice(start, end)` | Copy section | No | `arr.slice(1, 3)` |
| `splice(start, count)` | Add/remove items | Yes | `arr.splice(1, 2)` |
| `join(separator)` | Combine to string | No | `arr.join(", ")` |
| `reverse()` | Flip order | Yes | `arr.reverse()` |
| `sort()` | Arrange order | Yes | `arr.sort()` |
| `concat(arr2)` | Combine arrays | No | `arr1.concat(arr2)` |
| `forEach(fn)` | Do something with each | No | `arr.forEach(console.log)` |
| `map(fn)` | Transform each item | No | `arr.map(x => x * 2)` |
| `filter(fn)` | Keep items that pass test | No | `arr.filter(x => x > 5)` |
| `find(fn)` | Find first match | No | `arr.find(x => x > 5)` |
| `reduce(fn, start)` | Combine to single value | No | `arr.reduce((a,b) => a+b)` |
| `some(fn)` | Check if any pass test | No | `arr.some(x => x > 5)` |
| `every(fn)` | Check if all pass test | No | `arr.every(x => x > 0)` |

---

## Important Notes

1. **Mutating vs Non-Mutating Methods:**
   ```javascript
   // These CHANGE the original array:
   push(), pop(), shift(), unshift(), splice(), reverse(), sort()
   
   // These DON'T change the original array:
   slice(), concat(), map(), filter(), find(), reduce(), etc.
   ```

2. **Array indexing starts at 0:**
   ```javascript
   let fruits = ["apple", "banana", "orange"];
   // "apple" is at index 0
   // "banana" is at index 1  
   // "orange" is at index 2
   ```

3. **Callback functions:**
   ```javascript
   // Traditional function
   arr.map(function(item) { return item * 2; });
   
   // Arrow function (shorter)
   arr.map(item => item * 2);
   ```

---

## Practical Examples

### Shopping Cart Operations
```javascript
let cart = [];

// Add items
cart.push("laptop", "mouse");
console.log(cart); // ["laptop", "mouse"]

// Check if item exists
if (cart.includes("laptop")) {
    console.log("Laptop is in cart");
}

// Remove last item
cart.pop();
console.log(cart); // ["laptop"]
```

### Data Processing
```javascript
let prices = [19.99, 25.50, 12.00, 30.25];

// Calculate total
let total = prices.reduce((sum, price) => sum + price, 0);
console.log("Total: $" + total.toFixed(2)); // Total: $87.74

// Find expensive items
let expensive = prices.filter(price => price > 20);
console.log(expensive); // [25.50, 30.25]

// Add tax to all prices
let withTax = prices.map(price => price * 1.1);
console.log(withTax); // [21.989, 28.05, 13.2, 33.275]
```

### List Management
```javascript
let todos = ["buy milk", "walk dog", "write code"];

// Add new todo
todos.unshift("wake up"); // Add to beginning
console.log(todos); // ["wake up", "buy milk", "walk dog", "write code"]

// Mark first todo as done (remove it)
let completed = todos.shift();
console.log("Completed: " + completed); // Completed: wake up

// Sort remaining todos
todos.sort();
console.log(todos); // ["buy milk", "walk dog", "write code"]
```

---

## Practice Exercise

Try these examples:
```javascript
let numbers = [5, 2, 8, 1, 9, 3];

// 1. Add 10 to the end
numbers.push(10);

// 2. Sort the array
numbers.sort((a, b) => a - b);

// 3. Find all numbers greater than 5
let bigNumbers = numbers.filter(num => num > 5);

// 4. Double all numbers
let doubled = numbers.map(num => num * 2);

// 5. Calculate the sum
let sum = numbers.reduce((total, num) => total + num, 0);

// 6. Check if any number is greater than 10
let hasLarge = numbers.some(num => num > 10);

console.log("Original:", numbers);
console.log("Big numbers:", bigNumbers);
console.log("Doubled:", doubled);
console.log("Sum:", sum);
console.log("Has number > 10:", hasLarge);
```

Happy array manipulation! 📋
