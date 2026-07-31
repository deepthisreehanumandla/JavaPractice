# 62) Inner Class

## What is an Inner Class?

An **Inner Class** is a class declared **inside another class**.

```java
class Outer {

    class Inner {

    }
}
```

The class `Inner` belongs to `Outer`.

---

## Why Use an Inner Class?

Inner classes are used when a class is **closely related** to another class and is not required independently.

Examples:
- Car → Engine
- House → Room
- Computer → Processor

---

## Creating an Object

### Non-Static Inner Class

```java
class Outer {

    class Inner {

    }
}

Outer obj = new Outer();
Outer.Inner in = obj.new Inner();
```

An object of the outer class is required.

---

## Static Inner Class

```java
class Outer {

    static class Inner {

    }
}
```

Object creation:

```java
Outer.Inner obj = new Outer.Inner();
```

No outer class object is required.

---

## Accessing Outer Class Members

An inner class can directly access the members of its outer class.

```java
class Outer {

    int x = 10;

    class Inner {
        void show() {
            System.out.println(x);
        }
    }
}
```

### Output

```
10
```

---

## Types of Inner Classes

- Regular (Non-static) Inner Class
- Static Inner Class
- Anonymous Inner Class
- Local Inner Class

---

## Key Points

- An inner class is declared inside another class.
- A non-static inner class requires an outer class object.
- A static inner class can be instantiated directly.
- Inner classes can access members of the outer class.

---

## Interview Questions

### Can an inner class access the outer class members?

**Yes.**

---

### Does a static inner class require an outer class object?

**No.**

---

### Does a non-static inner class require an outer class object?

**Yes.**

---

## Summary

| Type | Outer Object Required |
|------|------------------------|
| Non-static Inner Class | ✅ Yes |
| Static Inner Class | ❌ No |

---

## Quick Revision

- Inner class = Class inside another class.
- Used for closely related classes.
- Non-static inner class → Requires outer object.
- Static inner class → No outer object needed.
- Inner classes can access outer class members.
