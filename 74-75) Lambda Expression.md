## 74-75) Lambda Expression & Lambda Expression with Return

### What is a Lambda Expression?
- A lambda expression is a shorter way to implement a **Functional Interface**.
- It removes the need to create a separate class or anonymous inner class.

### Syntax
```java
(parameters) -> {
    // code
}
```

### Example
```java id="k8m4zw"
@FunctionalInterface
interface A {
    void show();
}

A obj = () -> System.out.println("Hello");
obj.show();
```

---

### Lambda with Parameters
```java id="v2h7qe"
@FunctionalInterface
interface A {
    void show(int i);
}

A obj = (i) -> System.out.println(i);
```

---

### Lambda with Return Value
```java id="n4p8sj"
@FunctionalInterface
interface Add {
    int add(int a, int b);
}

Add obj = (a, b) -> a + b;

System.out.println(obj.add(5, 10));
```

### Key Points
- Works only with **Functional Interfaces**.
- Makes code shorter and more readable.
- `->` is called the **lambda operator**.
- `return` keyword can be omitted for single-expression lambdas.
- Parameter types are usually inferred by the compiler.
