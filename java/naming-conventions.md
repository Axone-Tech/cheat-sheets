# Java Naming Conventions Cheat Sheet

## Variables

### camelCase
Use for variable names
```java
String firstName = "John";
int maxCount = 100;
boolean isVisible = true;
```

## Methods

### camelCase
Use for method names
```java
public void calculateTotal() { /* ... */ }
public String getFullName() { /* ... */ }
```

## Classes and Interfaces

### PascalCase
Use for class and interface names
```java
public class UserAccount { /* ... */ }
public interface Printable { /* ... */ }
```

## Constants

### UPPER_CASE_WITH_UNDERSCORES
Use for constants (static final variables)
```java
public static final int MAX_USERS = 100;
public static final String API_BASE_URL = "https://api.example.com";
```

## Packages

### all.lowercase
Use lowercase for package names, separated by dots
```java
package com.example.myproject;
package org.myorganization.myapp;
```

## Enum Types

### PascalCase for enum name, UPPER_CASE for enum constants
```java
public enum DaysOfWeek {
    MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY
}
```

## Generic Type Parameters

### Single uppercase letter or descriptive name
```java
public class Box<T> { /* ... */ }
public interface Comparable<T> { /* ... */ }
public <E extends Enum<E>> void processEnum(Class<E> enumClass) { /* ... */ }
```

## File Names

### PascalCase.java
Match the public class or interface name
```
UserAccount.java
Printable.java
```

## Acronyms in Names

### Capitalize only the first letter if it's not the start of the name
```java
String url = "https://example.com";
HttpURLConnection connection;
class XmlHttpRequest { /* ... */ }
```

## Boolean Methods and Variables

### Prefix with 'is', 'has', 'can', etc.
```java
boolean isReady = true;
boolean hasPermission = false;
public boolean canEdit() { /* ... */ }
```

## Getters and Setters

### Prefix with 'get' and 'set'
```java
public String getName() { return name; }
public void setName(String name) { this.name = name; }
```

## Collection Naming

### Use plural nouns for collections
```java
List<String> names = new ArrayList<>();
Map<Integer, String> userMap = new HashMap<>();
```

Remember, these conventions are widely accepted in the Java community, but the most important aspect is maintaining consistency within your project or organization. Always adhere to your team's or company's specific guidelines if they differ from these general conventions.