# 📘 Video 11 - Logical Operators

## 1. Concepts

### What are Logical Operators?

**Logical operators** are used to combine or reverse boolean expressions.

The result of a logical operation is always a **boolean** value:

* `true`
* `false`

---

### Types of Logical Operators

| Operator | Meaning     |
| -------- | ----------- |
| `&&`     | Logical AND |
| `\|\|`   | Logical OR  |
| `!`      | Logical NOT |

---

## 2. Why?

Logical operators help us check **multiple conditions** at the same time.

They are commonly used in:

* `if`
* `if-else`
* Loops
* Decision making

---

## 3. Code Explained

### Logical AND (`&&`)

Returns `true` only if **both conditions are true**.

```java id="d2l1m9"
int x = 7;
int y = 5;

System.out.println(x > 5 && y < 10);
```

**Output**

```text id="m0w2n8"
true
```

---

### Logical OR (`||`)

Returns `true` if **at least one condition is true**.

```java id="0m0o9f"
int x = 7;
int y = 5;

System.out.println(x > 10 || y < 10);
```

**Output**

```text id="r3t2e5"
true
```

---

### Logical NOT (`!`)

Reverses the boolean value.

```java id="6r8j7v"
boolean result = true;

System.out.println(!result);
```

**Output**

```text id="v7c6d4"
false
```

---

## 4. Key Differences

| `&&` (AND) | `||` (OR) | `!` (NOT) |
|-------------|-----------|-----------|
| Both conditions must be `true` | At least one condition must be `true` | Reverses a boolean value |
| Returns `false` if any condition is `false` | Returns `false` only if both are `false` | `true` → `false`, `false` → `true` |

---

## 5. Interview Questions

### Q1. What is a logical operator?

**Answer:**

A logical operator is used to combine or reverse boolean expressions.

---

### Q2. Which logical operator returns `true` only when both conditions are true?

**Answer:**

`&&`

---

### Q3. Which logical operator returns `true` if at least one condition is true?

**Answer:**

`||`

---

### Q4. What is the output?

```java id="s8q4j2"
System.out.println(true && false);
```

**Answer**

```text id="t6v1o3"
false
```

---

### Q5. What is the output?

```java id="k1z9p8"
System.out.println(!false);
```

**Answer**

```text id="w2e4h1"
true
```

---

## 6. Practice

### Practice 1

Predict the output.

```java id="j5n4b7"
int a = 10;
int b = 20;

System.out.println(a < b && a > 5);
```

---

### Practice 2

Predict the output.

```java id="q9m7x6"
int a = 10;
int b = 20;

System.out.println(a > b || b > 15);
```

---

### Practice 3

Predict the output.

```java id="c4v8l2"
boolean flag = false;

System.out.println(!flag);
```

---

## 7. Key Takeaways

* Logical operators work with boolean expressions.
* `&&` → Both conditions must be true.
* `||` → At least one condition must be true.
* `!` → Reverses the boolean value.
* Result is always `true` or `false`.

---

## 8. Common Mistakes

❌ Confusing `&&` with `&`.

✔️ `&&` is the logical AND operator used with boolean expressions.

---

❌ Confusing `||` with `|`.

✔️ `||` is the logical OR operator used with boolean expressions.

---

❌ Applying `!` to non-boolean values.

```java id="n8x2p6"
!10
```

✔️ `!` can only be used with boolean expressions.

---

## 📝 30-Second Revision

* `&&` → Logical AND
* `||` → Logical OR
* `!` → Logical NOT
* `&&` requires both conditions to be `true`.
* `||` requires at least one condition to be `true`.
* `!` reverses `true` and `false`.
