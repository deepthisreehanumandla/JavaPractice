## 71) What is Annotation in Java

### What is an Annotation?
- Annotation provides additional information (metadata) about the code.
- It is used by the compiler or JVM and does not directly change the program logic.

### Syntax
```java
@Override
void show() {
    System.out.println("Hello");
}
```

### Common Annotations
- `@Override` → Indicates that a method is overriding a parent class method.
- `@Deprecated` → Marks a method or class as outdated and not recommended for use.
- `@SuppressWarnings` → Suppresses specified compiler warnings.

### Why use Annotations?
- Improves code readability.
- Helps the compiler detect mistakes.
- Makes code easier to maintain.

### Example
```java
class A {
    void show() {}
}

class B extends A {
    @Override
    void show() {
        System.out.println("Hello");
    }
}
```

### Key Points
- Annotation is metadata about the code.
- It starts with `@`.
- It helps the compiler and developers.
- It does not directly affect the program's execution.
