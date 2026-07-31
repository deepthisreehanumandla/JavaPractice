# 63) Anonymous Inner Class

## What is an Anonymous Inner Class?

An **Anonymous Inner Class** is an inner class **without a name**.

It is used when you need a class **only once**.

---

## Without Anonymous Inner Class

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

A obj = new B();
obj.show();
```

### Output

```
In B
```

---

## Using Anonymous Inner Class

Instead of creating a separate child class, we can write:

```java
class A {
    public void show() {
        System.out.println("In A");
    }
}

A obj = new A() {

    @Override
    public void show() {
        System.out.println("In Anonymous Class");
    }

};

obj.show();
```

### Output

```
In Anonymous Class
```

---

## Why Use It?

- No need to create a separate class.
- Useful when the class is needed only once.
- Reduces unnecessary code.

---

## Characteristics

- Has **no class name**.
- Created and instantiated at the same time.
- Cannot be reused later.
- Can override methods of the parent class or implement an interface.

---

## Key Points

- Anonymous = No name.
- Used for one-time implementation.
- Creates an object immediately.
- Cannot create another object of the same anonymous class later.

---

## Interview Questions

### Why is it called an Anonymous Inner Class?

Because it **does not have a class name**.

---

### Can an Anonymous Inner Class be reused?

**No.**

---

### Can it override methods?

**Yes.**

---

## Summary

| Feature | Anonymous Inner Class |
|---------|------------------------|
| Class Name | ❌ No |
| Reusable | ❌ No |
| One-time Use | ✅ Yes |
| Method Overriding | ✅ Yes |

---

## Quick Revision

- Anonymous Inner Class = Class without a name.
- Used only once.
- No separate child class required.
- Cannot be reused.
- Commonly used to override methods or implement interfaces.
