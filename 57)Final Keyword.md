# Java Notes – Video #57: Final Keyword

## What is the `final` Keyword?

The `final` keyword is used to **restrict modification**.

It can be used with:
- Variables
- Methods
- Classes

---

# 1. Final Variable

A `final` variable can be assigned **only once**.

```java
final int age = 20;

// age = 25; ❌ Error
```

Once initialized, its value cannot be changed.

---

# 2. Final Method

A `final` method **cannot be overridden** by a child class.

```java
class A {
    final void show() {
        System.out.println("Hello");
    }
}

class B extends A {

    // void show() { } ❌ Error
}
```

---

# 3. Final Class

A `final` class **cannot be inherited**.

```java
final class A {

}

// class B extends A { } ❌ Error
```

Example:
- `String` is a final class.

---

# Why Use `final`?

- Prevent accidental changes.
- Improve code security.
- Protect important methods and classes.

---

# Key Points

- `final` variable → Value cannot change.
- `final` method → Cannot be overridden.
- `final` class → Cannot be extended.

---

# Interview Questions

### Can a final variable be changed?

**No.**

---

### Can a final method be overridden?

**No.**

---

### Can a final class be inherited?

**No.**

---

# Summary

| final with | Meaning |
|------------|---------|
| Variable | Cannot be reassigned |
| Method | Cannot be overridden |
| Class | Cannot be inherited |

---

# Quick Revision

- `final` = Restriction
- Final variable → Constant value
- Final method → No overriding
- Final class → No inheritance
