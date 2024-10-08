# Java Variables Cheat Sheet

## Variable Declarations

### Primitive Types
```java
int age = 30;
double salary = 50000.50;
boolean isEmployed = true;
char grade = 'A';
byte smallNumber = 127;
short mediumNumber = 32767;
long bigNumber = 9223372036854775807L;
float price = 19.99f;
```

### Reference Types
```java
String name = "John Doe";
Integer wrappedInt = 100;
Double wrappedDouble = 3.14;
```

## Variable Scope

### Instance Variables
- Declared in a class, outside any method
- Accessible throughout the class
```java
public class Person {
    private String name;
    private int age;
}
```

### Local Variables
- Declared inside a method
- Only accessible within that method
```java
public void doSomething() {
    int localVar = 10;
    // Use localVar
}
```

### Static Variables
- Shared among all instances of a class
```java
public class Counter {
    public static int count = 0;
}
```

## Final Variables (Constants)
- Cannot be reassigned after initialization
```java
final double PI = 3.14159;
```

## Type Inference (Java 10+)
- Use `var` for local variable type inference
```java
var message = "Hello, Java!";
var numbers = new ArrayList<Integer>();
```

## Arrays
```java
int[] numbers = {1, 2, 3, 4, 5};
String[] names = new String[3];
```

## Enums
```java
enum DaysOfWeek {
    MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY
}
```

## Type Casting
```java
// Widening casting (automatic)
int myInt = 9;
double myDouble = myInt;

// Narrowing casting (manual)
double anotherDouble = 9.78;
int anotherInt = (int) anotherDouble;
```

## Wrapper Classes
```java
Integer wrappedInt = Integer.valueOf(42);
int primitiveInt = wrappedInt.intValue();
```

Remember, Java is a statically-typed language, so variables must be declared with their type before use. Always initialize variables before using them to avoid potential null pointer exceptions!