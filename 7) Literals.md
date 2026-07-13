# 📘 Video 7 - Literals

## 1. Concepts

### What is a Literal?

A **literal** is a fixed value written directly in a Java program.

Example:

```java
int num = 10;
```

Here, `10` is a literal.

---

### Integer Literals

Java supports different ways to represent integers.

#### Decimal (Base 10)

```java
int num = 25;
```

#### Binary (Base 2)

Starts with `0b`.

```java
int num = 0b101;
```

Output:

```text
5
```

#### Hexadecimal (Base 16)

Starts with `0x`.

```java
int num = 0x7E;
```

Output:

```text
126
```

---

### Underscore (`_`) in Numbers

Underscores improve readability.

```java
int num = 10_00_00_000;
```

Java ignores the underscores.

---

### Floating-Point Literals

```java
float num1 = 56;
double num2 = 56;
```

Both are valid because an `int` value can be stored safely in `float` and `double`.

For decimal values:

```java
float num = 12.5f;
double d = 12.5;
```

`double` is the default decimal type.

---

### Scientific Notation

```java
double num = 12e10;
```

Means:

```text
12 × 10¹⁰
```

---

### Boolean Literal

A boolean can store only:

```java
true
false
```

This is invalid:

```java
boolean b = 1;
```

---

### Character Literal

```java
char ch = 'a';
```

Characters are enclosed in **single quotes**.

Characters can also be incremented.

```java
char ch = 'a';
ch++;
```

Now:

```text
ch = 'b'
```

---

## 2. Why?

Literals allow us to write values directly in our program.

Java provides different literal formats to improve readability and support different number systems.

---

## 3. Code Explained

```java
int num1 = 0b101;
```

Binary literal.

Output:

```text
5
```

---

```java
int num2 = 0x7E;
```

Hexadecimal literal.

Output:

```text
126
```

---

```java
int num3 = 10_00_00_000;
```

Underscores improve readability.

Output:

```text
100000000
```

---

```java
double num = 12e10;
```

Scientific notation.

Equivalent to:

```text
12 × 10¹⁰
```

---

```java
char ch = 'a';
ch++;
```

Output:

```text
b
```

---

## 4. Interview Questions

### Q1. What is a literal?

**Answer:**

A literal is a fixed value written directly in a Java program.

---

### Q2. How do you write a binary literal?

**Answer:**

Using the `0b` prefix.

Example:

```java
0b101
```

---

### Q3. How do you write a hexadecimal literal?

**Answer:**

Using the `0x` prefix.

Example:

```java
0x7E
```

---

### Q4. Why do we use underscores in numbers?

**Answer:**

To improve readability.

Java ignores the underscores.

---

### Q5. What does `12e10` mean?

**Answer:**

`12 × 10¹⁰`

---

### Q6. Can a boolean store `1` or `0`?

**Answer:**

No.

A boolean can store only `true` or `false`.

---

## 5. Practice

### Practice 1

Write a binary literal representing `10`.

---

### Practice 2

Write a hexadecimal literal representing `255`.

---

### Practice 3

Store one crore using underscores.

---

### Practice 4

Increment a character:

```java
char ch = 'x';
```

Print the next character.

---

## 6. Key Takeaways

* Literal = Fixed value.
* Binary literals start with `0b`.
* Hexadecimal literals start with `0x`.
* Use `_` to improve number readability.
* Decimal literals are `double` by default.
* Scientific notation uses `e`.
* Boolean accepts only `true` and `false`.
* Characters use single quotes and can be incremented.

---

## 7. Common Mistakes

❌

```java
boolean b = 1;
```

✔️

```java
boolean b = true;
```

---

❌

```java
float f = 12.5;
```

✔️

```java
float f = 12.5f;
```

---

❌

```java
char ch = "A";
```

✔️

```java
char ch = 'A';
```

---

## 📝 30-Second Revision

* Literal = Fixed value.
* `0b` → Binary
* `0x` → Hexadecimal
* `_` → Readability
* `e` → Scientific notation
* `true` / `false` → Boolean literals
* `'A'` → Character literal
