# TypeScript Naming Conventions Cheat Sheet

## Variables and Functions

### camelCase
Use for variables, function names, and class methods
```typescript
let firstName = "John";
const maxCount = 100;
function calculateTotal() { /* ... */ }
class User {
  getFullName() { /* ... */ }
}
```

## Classes, Interfaces, and Types

### PascalCase
Use for class names, interface names, type aliases, and enum names
```typescript
class UserAccount { /* ... */ }
interface ValidationResult { /* ... */ }
type Point = { x: number; y: number };
enum Color { Red, Green, Blue }
```

## Constants

### UPPER_CASE
Use for global constants and enum members
```typescript
const MAX_ITEMS = 50;
const API_BASE_URL = "https://api.example.com";
enum HttpStatus {
  OK = 200,
  NOT_FOUND = 404,
  INTERNAL_SERVER_ERROR = 500
}
```

## Private Properties

### _camelCase
Use underscore prefix for private properties (convention, not enforced)
```typescript
class Example {
  private _internalValue: number;
}
```

## Interfaces

### IMyInterface or MyInterface
Prefixing with 'I' is optional, both are common
```typescript
interface IShape { /* ... */ }
interface UserData { /* ... */ }
```

## Type Parameters (Generics)

### T, U, V or TPascalCase
Use single uppercase letter or PascalCase prefixed with 'T'
```typescript
function identity<T>(arg: T): T { return arg; }
class GenericClass<TData> { /* ... */ }
```

## File Names

### kebab-case.ts
Use kebab-case for file names
```
user-account.ts
validation-utils.ts
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
```typescript
let isActive = true;
let hasPermission = false;
let canEdit = true;
```

## Naming Arrays

### Plural nouns
Use plural form for arrays
```typescript
const users: User[] = [];
const productList: Product[] = [];
```

## Naming Functions

### Verb or verb phrase
Start with a verb that describes the action
```typescript
function getUserData() { /* ... */ }
function validateInput() { /* ... */ }
```

Remember, consistency is key in naming conventions. While these are common practices, the most important thing is to follow the conventions established in your project or team.