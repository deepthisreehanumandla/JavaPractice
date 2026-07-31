# Java Notes – Video #56: Dynamic Method Dispatch

## What is Dynamic Method Dispatch?

Dynamic Method Dispatch is the mechanism by which Java decides **at runtime** which overridden method to execute.

It is the **runtime implementation of polymorphism**.

---

## Syntax

```java
A obj = new B();
```

- `A` → Parent class reference
- `B` → Child class object

This is called **upcasting**.

---

## Example

```java
class A {
    public void show() {
        System.out.println("In A");
    }
}

class B extends A {
    @Override
    public void show() {
        System.out.println("In B");
    }
}

public class Demo {
    public static void main(String[] args) {
        A obj = new B();
        obj.show();
    }
}
```

### Output

```
In B
```

---

## Why?

Although `obj` is a reference of type `A`, it points to an object of type `B`.

At runtime, Java checks the actual object (`B`) and calls the overridden method.

---

## Rules

- Works only with **method overriding**.
- Parent reference can point to a child object.
- Method execution depends on the **actual object**, not the reference type.

---

## Key Points

- Runtime Polymorphism
- Parent Reference → Child Object
- Method chosen at runtime
- Overriding is required

---

## Interview Questions

### Can Dynamic Method Dispatch work without method overriding?

**No.**

### Is Dynamic Method Dispatch compile-time or runtime polymorphism?

**Runtime Polymorphism.**

---

## Summary

- Java decides which overridden method to execute **at runtime**.
- The reference type controls what is accessible.
- The object type controls which overridden method runs.
