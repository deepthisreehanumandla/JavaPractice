# 64) Abstract and Anonymous Inner Class

## Can We Create an Object of an Abstract Class?

❌ No.

```java
abstract class A {

}

A obj = new A(); // Error
```

An abstract class cannot be instantiated.

---

## Anonymous Inner Class with an Abstract Class

Although we cannot create an object of an abstract class directly, we **can** create an anonymous inner class that provides the implementation.

```java
abstract class A {

    public abstract void show();

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

## How Does It Work?

Java creates a temporary unnamed subclass of `A` and implements the abstract method.

The object created is actually an object of this anonymous subclass.

---

## Why Use It?

- Avoid creating a separate child class.
- Useful when the implementation is needed only once.
- Makes the code shorter and cleaner.

---

## Key Points

- Abstract classes cannot be instantiated directly.
- Anonymous inner classes can extend abstract classes.
- Abstract methods must be implemented.
- No separate subclass is required.

---

## Interview Questions

### Can we create an object of an abstract class?

**No.**

---

### Can an anonymous inner class extend an abstract class?

**Yes.**

---

### Why is an anonymous inner class used with an abstract class?

To provide a one-time implementation of abstract methods without creating a separate subclass.

---

## Summary

| Feature | Abstract Class | Anonymous Inner Class |
|---------|----------------|-----------------------|
| Object Creation | ❌ Directly Not Allowed | ✅ Allowed |
| Class Name | Yes | ❌ No |
| One-time Implementation | ❌ | ✅ |

---

## Quick Revision

- Cannot create an object of an abstract class directly.
- Anonymous inner class provides the implementation.
- No separate child class is needed.
- Useful for one-time implementations.
