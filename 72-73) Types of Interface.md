## 72-73) Types of Interface & Functional Interface

### Types of Interface

#### 1. Normal Interface
- Contains two or more abstract methods.
- A class implementing it must define all its methods.

```java
interface A {
    void show();
    void display();
}
```

#### 2. Functional Interface
- Contains **exactly one abstract method**.
- Can have multiple `default` and `static` methods.
- Mainly used with Lambda Expressions.

```java
@FunctionalInterface
interface A {
    void show();
}
```

#### 3. Marker Interface
- Contains **no methods**.
- Used to provide special information to the JVM or compiler.

Example:
```java
Serializable
Cloneable
```

---

### @FunctionalInterface Annotation
- Ensures the interface contains only one abstract method.
- If another abstract method is added, the compiler throws an error.

```java
@FunctionalInterface
interface A {
    void show();
}
```

### Why Functional Interfaces?
- Makes code shorter and cleaner.
- Required for Lambda Expressions.
- Represents a single behavior or action.

### Key Points
- **Normal Interface** → Multiple abstract methods.
- **Functional Interface** → Exactly one abstract method.
- **Marker Interface** → No methods.
- `@FunctionalInterface` is optional but recommended for compiler checking.
