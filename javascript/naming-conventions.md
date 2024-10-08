# JavaScript Naming Conventions Cheat Sheet

## Variables and Functions

### camelCase
Use for variables, function names, and object methods
```javascript
let firstName = "John";
const maxCount = 100;
function calculateTotal() { /* ... */ }
const user = {
  getFullName() { /* ... */ }
};
```

## Classes and Constructor Functions

### PascalCase
Use for class names and constructor functions
```javascript
class UserAccount { /* ... */ }
function Person(name) { this.name = name; }
```

## Constants

### UPPER_CASE
Use for global constants and configuration values
```javascript
const MAX_ITEMS = 50;
const API_BASE_URL = "https://api.example.com";
```

## Private Properties (Convention)

### _camelCase
Use underscore prefix for properties intended to be private (not enforced)
```javascript
class Example {
  constructor() {
    this._internalValue = 0;
  }
}
```

## File Names

### kebab-case.js
Use kebab-case for file names
```
user-account.js
validation-utils.js
```

## Folders

### kebab-case
Use kebab-case for folder names
```
src/
  components/
  utils/
  services/
```

## Naming Boolean Variables

### is, has, can
Prefix with verbs that suggest a boolean
```javascript
let isActive = true;
let hasPermission = false;
let canEdit = true;
```

## Naming Arrays

### Plural nouns
Use plural form for arrays
```javascript
const users = [];
const productList = [];
```

## Naming Functions

### Verb or verb phrase
Start with a verb that describes the action
```javascript
function getUserData() { /* ... */ }
function validateInput() { /* ... */ }
```

## Modules (ES6+)

### camelCase or PascalCase
Use camelCase for default exports, PascalCase for constructor-like modules
```javascript
// file: myModule.js
export default function myFunction() { /* ... */ }

// file: MyClass.js
export default class MyClass { /* ... */ }
```

## Event Handlers

### onEventName
Prefix with 'on' for event handler functions
```javascript
function onButtonClick() { /* ... */ }
element.addEventListener('click', onButtonClick);
```

## Acronyms and Initialisms

### Capitalize normally
Treat acronyms as words in names
```javascript
let userId = 1;
function parseHtml() { /* ... */ }
class HttpRequest { /* ... */ }
```

Remember, while these conventions are widely used, the most important thing is to maintain consistency within your project or team. Always follow the established conventions in your codebase.