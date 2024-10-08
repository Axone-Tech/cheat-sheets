# Java Loops Cheat Sheet

## for Loop

Basic syntax:
```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```

Loop with step value:
```java
for (int i = 0; i < 10; i += 2) {
    System.out.println(i);
}
```

## while Loop

Basic syntax:
```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
```

## do...while Loop

Basic syntax:
```java
int i = 0;
do {
    System.out.println(i);
    i++;
} while (i < 5);
```

## Enhanced for Loop (for-each)

Iterating over arrays or collections:
```java
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

## Iterator

Using Iterator interface:
```java
List<String> list = Arrays.asList("A", "B", "C");
Iterator<String> iterator = list.iterator();
while (iterator.hasNext()) {
    System.out.println(iterator.next());
}
```

## Stream forEach (Java 8+)

Using streams for iteration:
```java
List<String> list = Arrays.asList("A", "B", "C");
list.stream().forEach(System.out::println);
```

## Parallel Stream forEach (Java 8+)

Parallel processing of elements:
```java
List<String> list = Arrays.asList("A", "B", "C");
list.parallelStream().forEach(System.out::println);
```

## Breaking and Continuing

Using break:
```java
for (int i = 0; i < 5; i++) {
    if (i == 3) break;
    System.out.println(i);
}
```

Using continue:
```java
for (int i = 0; i < 5; i++) {
    if (i == 2) continue;
    System.out.println(i);
}
```

## Labeled Breaks and Continues

Using labels with break:
```java
outerLoop: for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i == 1 && j == 1) break outerLoop;
        System.out.println(i + " " + j);
    }
}
```

## Infinite Loop

Creating an infinite loop:
```java
while (true) {
    // This will run indefinitely
    // Use break to exit when needed
}
```

## for Loop with Multiple Variables

Initializing multiple variables:
```java
for (int i = 0, j = 10; i < j; i++, j--) {
    System.out.println(i + " " + j);
}
```

Remember, Java is statically typed, so ensure that your loop variables and iterated elements are of the correct type. Also, be cautious of potential infinite loops and ensure proper termination conditions.
``````

This cheat sheet covers various looping constructs in Java, including traditional loops, enhanced for-each loops, and modern Java features like streams for iteration.
`````
