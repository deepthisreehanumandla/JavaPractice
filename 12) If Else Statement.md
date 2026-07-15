# 📘 Video 12 - If Else Statement

## 1. Concepts

### What is an `if` Statement?

An `if` statement is used to execute a block of code **only when a condition is true**.

Syntax:

```java id="o5k9j2"
if (condition) {
    // code
}
```

---

### What is an `if-else` Statement?

An `if-else` statement is used when there are **two possible outcomes**.

* If the condition is `true`, the `if` block executes.
* Otherwise, the `else` block executes.

Syntax:

```java id="0j6l9e"
if (condition) {
    // true block
} else {
    // false block
}
```

---

## 2. Why?

Decision-making is an essential part of programming.

The `if-else` statement allows a program to choose between two different paths based on a condition.

---

## 3. Code Explained

### Example 1

```java id="i1k8b4"
int age = 20;

if (age >= 18)
    System.out.println("Eligible");
```

**Output**

```text id="yx2g8s"
Eligible
```

Since the condition is `true`, the `if` block executes.

---

### Example 2

```java id="uf7v3n"
int age = 16;

if (age >= 18)
    System.out.println("Eligible");
else
    System.out.println("Not Eligible");
```

**Output**

```text id="r7w4m1"
Not Eligible
```

Since the condition is `false`, the `else` block executes.

---

### Using Curly Braces

```java id="g8e2q5"
if (age >= 18) {
    System.out.println("Eligible");
    System.out.println("Welcome");
}
```

Curly braces `{}` are used when executing **multiple statements**.

---

## 4. Key Differences

| `if`                                        | `if-else`                  |
| ------------------------------------------- | -------------------------- |
| Executes code only if the condition is true | Chooses between two blocks |
| No alternative block                        | Has an `else` block        |
| May execute nothing                         | Exactly one block executes |

---

## 5. Interview Questions

### Q1. What is an `if` statement?

**Answer:**

An `if` statement executes a block of code only when the given condition is `true`.

---

### Q2. What is an `if-else` statement?

**Answer:**

An `if-else` statement executes one block if the condition is `true` and another block if it is `false`.

---

### Q3. What is the output?

```java id="l9r4t7"
int x = 10;

if (x > 5)
    System.out.println("Java");
else
    System.out.println("Python");
```

**Answer**

```text id="u4m7z9"
Java
```

---

### Q4. What type of value must an `if` condition return?

**Answer:**

A **boolean** value (`true` or `false`).

---

## 6. Practice

### Practice 1

Write a program to check whether a number is positive.

---

### Practice 2

Write a program to check whether a person is eligible to vote.

---

### Practice 3

Predict the output.

```java id="y3c8v6"
int num = 8;

if (num % 2 == 0)
    System.out.println("Even");
else
    System.out.println("Odd");
```

---

## 7. Key Takeaways

* `if` executes code only when the condition is `true`.
* `if-else` chooses between two blocks.
* The condition must evaluate to a **boolean**.
* Curly braces `{}` are recommended when writing multiple statements.

---

## 8. Common Mistakes

❌ Using a non-boolean condition.

```java id="m8t5p1"
if (10)
```

✔️ Correct

```java id="p6n4q8"
if (10 > 5)
```

---

❌ Forgetting braces when multiple statements should execute.

```java id="r2j7x4"
if (age >= 18)
    System.out.println("Eligible");
    System.out.println("Welcome");
```

Only the first statement belongs to the `if`.

✔️ Correct

```java id="v5k1n9"
if (age >= 18) {
    System.out.println("Eligible");
    System.out.println("Welcome");
}
```

---

## 📝 30-Second Revision

* `if` → Executes only if the condition is `true`.
* `if-else` → Chooses between two blocks.
* Conditions must return `true` or `false`.
* Use `{}` for multiple statements.
* Commonly used for decision making.
