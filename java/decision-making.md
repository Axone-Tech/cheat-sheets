# Java Decision Making Cheat Sheet

## if Statement

Basic syntax:
```java
if (condition) {
    // code to execute if condition is true
}
````

With else:
````java
if (condition) {
    // code to execute if condition is true
} else {
    // code to execute if condition is false
}
````

Multiple conditions:
````java
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
````java
result = (condition) ? valueIfTrue : valueIfFalse;
````

## switch Statement

For multiple branching based on a value:
````java
switch (expression) {
    case value1:
        // code to execute if expression == value1
        break;
    case value2:
        // code to execute if expression == value2
        break;
    default:
        // code to execute if no case matches
        break;
}
````

## Enhanced switch Statement (Java 14+)

Pattern matching for switch:
````java
switch (variable) {
    case IntegerValue i -> System.out.println("Integer: " + i);
    case String s -> System.out.println("String: " + s);
    default -> System.out.println("Unknown type");
}
````

## instanceof Operator

For type checking:
````java
if (obj instanceof String) {
    String str = (String) obj;
    // code to execute if obj is an instance of String
}
````

Pattern Matching for instanceof (Java 16+):
````java
if (obj instanceof String str) {
    // str is already cast to String
    System.out.println(str.length());
}
````

## try-catch-finally Statement

For exception handling:
````java
try {
    // code that might throw an exception
} catch (ExceptionType1 e1) {
    // code to handle ExceptionType1
} catch (ExceptionType2 e2) {
    // code to handle ExceptionType2
} finally {
    // code that will always execute
}
````

## assert Statement

For debugging and testing:
````java
assert condition : "Error message if condition is false";
````

## Null Checking

Using null check:
````java
if (obj != null) {
    obj.method();
}
````

Using Optional (Java 8+):
````java
Optional<String> optional = Optional.ofNullable(nullableString);
optional.ifPresent(s -> System.out.println(s.length()));
````

## Short-circuit Evaluation

Using && for conditional execution:
````java
if (obj != null && obj.isValid()) {
    // code to execute if obj is not null and is valid
}
````

Using || for default values:
````java
String name = inputName != null ? inputName : "Anonymous";
````

Remember, Java is a statically typed language, so type checking is done at compile-time. However, runtime checks are still necessary for certain operations, especially when dealing with object references and type casting.