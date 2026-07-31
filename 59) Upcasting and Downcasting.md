# 59) Upcasting and Downcasting

## What is Upcasting?

**Upcasting** is the process of converting a **child class object** into a **parent class reference**.

It happens **automatically**.

```java
class A {

}

class B extends A {

}

A obj = new B();
```

Here:
- `B` → Child class
- `A` → Parent class

This is called **Upcasting**.

---

## Why Use Upcasting?

Upcasting allows us to achieve:

- Runtime Polymorphism
- Dynamic Method Dispatch
- Code flexibility

---

## Method Access

```java
class A {
    void show() {
        System.out.println("A");
    }
}

class B extends A {
    void show() {
        System.out.println("B");
    }

    void display() {
        System.out.println("Display");
    }
}

A obj = new B();

obj.show();      // ✅ Allowed
// obj.display(); // ❌ Error
```

The parent reference can access **only the methods available in the parent class**.

If a method is overridden, the **child's implementation** is executed.

---

## What is Downcasting?

**Downcasting** is the process of converting a **parent reference** back into a **child reference**.

It must be done **explicitly**.

```java
A obj = new B();

B b = (B) obj;
```

Now child-specific methods can be accessed.

```java
b.display();
```

---

## Why Do We Need Downcasting?

Downcasting is useful when you want to access methods or properties that exist only in the child class.

---

## Key Points

- Upcasting → Child object to Parent reference.
- Upcasting is automatic.
- Downcasting → Parent reference to Child reference.
- Downcasting requires explicit casting.
- Invalid downcasting throws `ClassCastException`.

---

## Interview Questions

### Is Upcasting automatic?

**Yes.**

---

### Does Downcasting require explicit casting?

**Yes.**

---

### Which exception occurs during invalid downcasting?

**ClassCastException**

---

## Summary

| Upcasting | Downcasting |
|-----------|-------------|
| Child → Parent | Parent → Child |
| Automatic | Explicit |
| Used for Polymorphism | Used to access child-specific members |

---

## Quick Revision

- Upcasting = Child object → Parent reference.
- Downcasting = Parent reference → Child reference.
- Upcasting enables runtime polymorphism.
- Downcasting allows access to child-specific methods.
- Invalid downcasting results in `ClassCastException`.
