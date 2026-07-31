# 65–67) Interfaces

## What is an Interface?

An **Interface** is a blueprint of a class that contains **abstract methods**.

It is used to achieve **abstraction** and define a contract that implementing classes must follow.

```java
interface A {

    void show();

}
```

By default:

- All methods are **public** and **abstract**.
- All variables are **public**, **static**, and **final**.

---

## Implementing an Interface

A class implements an interface using the `implements` keyword.

```java
interface A {

    void show();

}

class B implements A {

    @Override
    public void show() {
        System.out.println("In Show");
    }

}
```

Object creation:

```java
A obj = new B();

obj.show();
```

### Output

```
In Show
```

---

## Why Do We Need Interfaces?

Interfaces help to:

- Achieve abstraction.
- Define a common contract.
- Reduce coupling between classes.
- Support multiple inheritance.

Example:

```java
interface Animal {
    void sound();
}

class Dog implements Animal {

    public void sound() {
        System.out.println("Bark");
    }

}

class Cat implements Animal {

    public void sound() {
        System.out.println("Meow");
    }

}
```

Both classes follow the same contract.

---

## Multiple Interface Implementation

A class can implement multiple interfaces.

```java
interface A {
    void show();
}

interface B {
    void display();
}

class C implements A, B {

    public void show() {
        System.out.println("Show");
    }

    public void display() {
        System.out.println("Display");
    }

}
```

Java allows **multiple inheritance through interfaces**.

---

## Interface Variables

All interface variables are automatically:

- `public`
- `static`
- `final`

```java
interface Demo {

    int age = 20;

}
```

Equivalent to:

```java
public static final int age = 20;
```

Their values cannot be changed.

---

## Interface Methods

By default, every interface method is:

```java
public abstract
```

Example:

```java
interface Demo {

    void show();

}
```

Equivalent to:

```java
public abstract void show();
```

---

## Key Points

- Interface is a blueprint of a class.
- Cannot create objects of an interface.
- Classes use `implements` to implement interfaces.
- A class can implement multiple interfaces.
- Interface methods are `public abstract` by default.
- Interface variables are `public static final` by default.

---

## Interview Questions

### Can we create an object of an interface?

**No.**

---

### Which keyword is used with an interface?

**implements**

---

### Can a class implement multiple interfaces?

**Yes.**

---

### What are interface methods by default?

**public abstract**

---

### What are interface variables by default?

**public static final**

---

## Summary

| Feature | Interface |
|---------|-----------|
| Object Creation | ❌ Not Allowed |
| Keyword | `interface` |
| Implemented Using | `implements` |
| Methods | `public abstract` |
| Variables | `public static final` |
| Multiple Inheritance | ✅ Supported |

---

## Quick Revision

- Interface = Blueprint of a class.
- Cannot create interface objects.
- Classes implement interfaces using `implements`.
- One class can implement multiple interfaces.
- Methods are `public abstract`.
- Variables are `public static final`.
- Used to achieve abstraction and multiple inheritance.
