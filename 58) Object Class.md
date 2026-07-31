# 58) Object Class

## What is the Object Class?

The `Object` class is the **parent class of all classes** in Java.

Every class directly or indirectly inherits from `Object`.

---

## Why is it Important?

Since every class extends `Object`, all objects have access to its methods.

Some commonly used methods are:

- `toString()`
- `equals()`
- `hashCode()`

---

## 1. toString()

Returns the **string representation** of an object.

```java
class Student {

}

public class Demo {
    public static void main(String[] args) {
        Student obj = new Student();
        System.out.println(obj);
    }
}
```

### Output

```
Student@15db9742
```

By default, it prints:

```
ClassName@HexadecimalHashCode
```

You can override `toString()` to display meaningful information.

```java
class Student {
    String name = "Deepthi";

    @Override
    public String toString() {
        return name;
    }
}
```

### Output

```
Deepthi
```

---

## 2. equals()

Used to compare **two objects**.

By default, it compares **references (memory locations)**.

```java
Student s1 = new Student();
Student s2 = new Student();

System.out.println(s1.equals(s2));
```

### Output

```
false
```

You can override `equals()` to compare object data instead.

---

## 3. hashCode()

Returns a unique integer value (hash code) for an object.

It is mainly used in collections like:

- HashMap
- HashSet

---

## Key Points

- Every class extends `Object`.
- `Object` is the root of Java's class hierarchy.
- `toString()` returns a string representation.
- `equals()` compares objects.
- `hashCode()` returns an integer hash value.

---

## Interview Questions

### Which class is the parent of all classes in Java?

**Object**

### Can we override `toString()`?

**Yes.**

### What does `equals()` compare by default?

**Object references (memory addresses).**

---

## Summary

| Method | Purpose |
|--------|---------|
| `toString()` | Returns string representation of an object |
| `equals()` | Compares two objects |
| `hashCode()` | Returns hash value of an object |

---

## Quick Revision

- `Object` is the parent of every class.
- Every object inherits `Object` methods.
- Override `toString()` for meaningful output.
- Override `equals()` to compare object data.
- `hashCode()` is commonly used in collections.
