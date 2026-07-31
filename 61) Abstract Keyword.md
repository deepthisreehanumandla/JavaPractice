# 61) Abstract Keyword

## What is an Abstract Class?

An **abstract class** is a class that **cannot be instantiated**, meaning you cannot create its object.

```java
abstract class Animal {

}
```

❌ Invalid

```java
Animal obj = new Animal();
```

---

## Why Use an Abstract Class?

An abstract class is used when a parent class provides a **common blueprint**, but the implementation should be provided by its child classes.

Example:

```java
abstract class Animal {
    abstract void sound();
}
```

Each child class provides its own implementation of `sound()`.

---

## Abstract Method

An **abstract method** is a method **without a body**.

```java
abstract void sound();
```

- No implementation
- Ends with a semicolon (`;`)
- Must be implemented by child classes

---

## Implementing an Abstract Method

```java
abstract class Animal {
    abstract void sound();
}

class Dog extends Animal {

    @Override
    void sound() {
        System.out.println("Bark");
    }
}
```

Object creation:

```java
Animal obj = new Dog();

obj.sound();
```

### Output

```
Bark
```

---

## Rules

- An abstract class **cannot** be instantiated.
- An abstract class **can have** constructors.
- An abstract class **can have** normal methods.
- An abstract class **can have** variables.
- A child class **must implement** all abstract methods.
- If it doesn't, the child class must also be declared `abstract`.

---

## Why Use Abstract Classes?

- To provide a common blueprint.
- To achieve abstraction.
- To force child classes to implement required methods.

---

## Key Points

- Use the `abstract` keyword for abstract classes and methods.
- Abstract methods have no implementation.
- Abstract classes can contain both abstract and normal methods.
- Objects can only be created for concrete (non-abstract) child classes.

---

## Interview Questions

### Can we create an object of an abstract class?

**No.**

---

### Can an abstract class have a constructor?

**Yes.**

---

### Can an abstract class contain normal methods?

**Yes.**

---

### What happens if a child class doesn't implement all abstract methods?

It must also be declared `abstract`.

---

## Summary

| Feature | Abstract Class |
|---------|----------------|
| Object Creation | ❌ Not Allowed |
| Constructors | ✅ Allowed |
| Normal Methods | ✅ Allowed |
| Abstract Methods | ✅ Allowed |

---

## Quick Revision

- Abstract class → Cannot create objects.
- Abstract method → No body.
- Child class must implement abstract methods.
- If not implemented, child class becomes abstract.
- Used to provide a common blueprint for child classes.
