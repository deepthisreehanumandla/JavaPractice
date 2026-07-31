# 60) Wrapper Class

## What is a Wrapper Class?

A **Wrapper Class** is a class that **wraps a primitive data type into an object**.

| Primitive | Wrapper Class |
|-----------|---------------|
| `byte` | `Byte` |
| `short` | `Short` |
| `int` | `Integer` |
| `long` | `Long` |
| `float` | `Float` |
| `double` | `Double` |
| `char` | `Character` |
| `boolean` | `Boolean` |

---

## Why Do We Need Wrapper Classes?

Primitive data types are **not objects**.

Some Java features (like the Collections Framework) work only with **objects**.

Wrapper classes allow primitive values to be used as objects.

---

## Autoboxing

**Autoboxing** is the automatic conversion of a **primitive** into its corresponding **wrapper object**.

```java
int num = 10;

Integer obj = num;
```

Java automatically converts `int` to `Integer`.

---

## Unboxing

**Unboxing** is the automatic conversion of a **wrapper object** into its corresponding **primitive**.

```java
Integer obj = 10;

int num = obj;
```

Java automatically converts `Integer` to `int`.

---

## Before Java 5

Before autoboxing and unboxing, conversion was done manually.

```java
Integer obj = Integer.valueOf(10);

int num = obj.intValue();
```

---

## Wrapper Class Methods

```java
String s = "123";

int num = Integer.parseInt(s);
```

Output:

```
123
```

Useful methods include:

- `parseInt()`
- `valueOf()`
- `toString()`

---

## Key Points

- Wrapper classes convert primitives into objects.
- Every primitive has a corresponding wrapper class.
- Autoboxing = Primitive → Object.
- Unboxing = Object → Primitive.
- Wrapper classes provide useful utility methods.

---

## Interview Questions

### What is the wrapper class for `int`?

**Integer**

---

### What is Autoboxing?

Automatic conversion of a primitive into its wrapper object.

---

### What is Unboxing?

Automatic conversion of a wrapper object into its primitive type.

---

### Can `Integer` store `null`?

**Yes.**

### Can `int` store `null`?

**No.**

---

## Summary

| Primitive | Wrapper |
|-----------|---------|
| `int` | `Integer` |
| `double` | `Double` |
| `char` | `Character` |
| `boolean` | `Boolean` |

---

## Quick Revision

- Wrapper Class = Primitive + Object
- `int` → `Integer`
- Autoboxing → Primitive to Object
- Unboxing → Object to Primitive
- Wrapper classes provide helper methods like `parseInt()`
