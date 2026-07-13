# 📘 Video 10 - Relational Operators

## 1. Concepts

### What is a Relational Operator?

A **relational operator** is used to compare two values.

The result of a relational operation is always a **boolean** value:

* `true`
* `false`

---

### Types of Relational Operators

| Operator | Meaning                  |
| -------- | ------------------------ |
| `==`     | Equal to                 |
| `!=`     | Not equal to             |
| `>`      | Greater than             |
| `<`      | Less than                |
| `>=`     | Greater than or equal to |
| `<=`     | Less than or equal to    |

---

## 2. Why?

Relational operators help us compare values and make decisions in a program.

They are mainly used with:

* `if`
* `if-else`
* Loops

---

## 3. Code Explained

### Equal To (`==`)

```java
int x = 6;
int y = 4;

System.out.println(x == y);
```

**Output**

```text
false
```

---

### Not Equal To (`!=`)

```java
System.out.println(x != y);
```

**Output**

```text
true
```

---

### Greater Than (`>`)

```java
System.out.println(x > y);
```

**Output**

```text
true
```

---

### Less Than (`<`)

```java
System.out.println(x < y);
```

**Output**

```text
false
```

---

### Greater Than or Equal To (`>=`)

```java
System.out.println(x >= y);
```

**Output**

```text
true
```

---

### Less Than or Equal To (`<=`)

```java
System.out.println(x <= y);
```

**Output**

```text
false
```

---

## 4. Key Differences

### `=` vs `==`

| `=`                            | `==`                      |
| ------------------------------ | ------------------------- |
| Assignment operator            | Relational operator       |
| Assigns a value                | Compares two values       |
| Does not return `true`/`false` | Returns `true` or `false` |

Example:

```java
int a = 10;
```

Here `=` assigns `10` to `a`.

```java
System.out.println(a == 10);
```

Here `==` checks whether `a` is equal to `10`.

---

## 5. Interview Questions

### Q1. What is a relational operator?

**Answer:**

A relational operator compares two values and returns either `true` or `false`.

---

### Q2. What is the difference between `=` and `==`?

**Answer:**

`=` assigns a value, whereas `==` compares two values.

---

### Q3. What is the output?

```java
int a = 10;
int b = 20;

System.out.println(a > b);
```

**Answer**

```text
false
```

---

### Q4. What is the return type of a relational operator?

**Answer:**

`boolean`

---

## 6. Practice

### Practice 1

Predict the output.

```java
int x = 15;
int y = 15;

System.out.println(x == y);
```

---

### Practice 2

Predict the output.

```java
int x = 12;
int y = 20;

System.out.println(x != y);
```

---

### Practice 3

Predict the output.

```java
int a = 7;
int b = 9;

System.out.println(a >= b);
```

---

### Practice 4

Write a program that compares two integers using all six relational operators.

---

## 7. Key Takeaways

* Relational operators compare two values.
* The result is always `true` or `false`.
* `==` checks equality.
* `!=` checks inequality.
* `>`, `<`, `>=`, `<=` compare values.
* Commonly used in decision-making statements.

---

## 8. Common Mistakes

❌ Using `=` instead of `==`

```java
if (a = b)
```

✔️

```java
if (a == b)
```

---

❌ Expecting a relational operator to return a number.

✔️ It always returns a **boolean** (`true` or `false`).

---

## 📝 30-Second Revision

* Relational operators compare two values.
* Return type is always `boolean`.
* `==` → Equal to
* `!=` → Not equal to
* `>` → Greater than
* `<` → Less than
* `>=` → Greater than or equal to
* `<=` → Less than or equal to
* Don't confuse `=` with `==`.
