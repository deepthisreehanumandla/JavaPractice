# 📘 Video 14 -# 📘 Video 14 - Ternary Operator

## 1. Concepts

### What is the Ternary Operator?

The **ternary operator (`?:`)** is a shorthand way of writing an `if-else` statement.

It is called **ternary** because it uses **three operands**:

* Condition
* Value if the condition is `true`
* Value if the condition is `false`

---

### Syntax

```java id="2m7qkx"
result = (condition) ? value1 : value2;
```

If the condition is `true`, `value1` is returned.

Otherwise, `value2` is returned.

---

## 2. Why?

The ternary operator makes simple `if-else` statements shorter and more readable.

Instead of writing:

```java id="m0n3zp"
if (age >= 18)
    result = "Adult";
else
    result = "Minor";
```

You can write:

```java id="n5y4dr"
result = (age >= 18) ? "Adult" : "Minor";
```

---

## 3. Code Explained

### Example 1

```java id="n8v4jy"
int age = 20;

String result = (age >= 18) ? "Adult" : "Minor";

System.out.println(result);
```

**Output**

```text id="d8z1tr"
Adult
```

---

### Example 2

```java id="m6w2qk"
int num = 8;

String result = (num % 2 == 0) ? "Even" : "Odd";

System.out.println(result);
```

**Output**

```text id="s4p8nx"
Even
```

---

## 4. Key Differences

| `if-else`                     | Ternary Operator (`?:`)    |
| ----------------------------- | -------------------------- |
| Multiple lines                | Single line                |
| Better for complex logic      | Best for simple conditions |
| Uses `if` and `else` keywords | Uses `?` and `:`           |

Example:

```java id="j3f6mt"
if (x > y)
    max = x;
else
    max = y;
```

Equivalent to:

```java id="t5r9cv"
max = (x > y) ? x : y;
```

---

## 5. Interview Questions

### Q1. What is the ternary operator?

**Answer:**

The ternary operator is a shorthand way of writing a simple `if-else` statement.

---

### Q2. Why is it called a ternary operator?

**Answer:**

Because it uses **three operands**:

* Condition
* Value if true
* Value if false

---

### Q3. What is the output?

```java id="j9b7vl"
int a = 10;

System.out.println((a > 5) ? "Yes" : "No");
```

**Answer**

```text id="u1x5ke"
Yes
```

---

### Q4. Can the ternary operator replace every `if-else` statement?

**Answer:**

No.

It is best suited for **simple** `if-else` conditions.

---

## 6. Practice

### Practice 1

Write a program to find the larger of two numbers using the ternary operator.

---

### Practice 2

Write a program to check whether a number is even or odd using the ternary operator.

---

### Practice 3

Predict the output.

```java id="x7m3bz"
int marks = 35;

String result = (marks >= 35) ? "Pass" : "Fail";

System.out.println(result);
```

---

## 7. Key Takeaways

* The ternary operator is a shortcut for `if-else`.
* Syntax:

```java id="e2v8pn"
(condition) ? value1 : value2;
```

* Returns one value based on the condition.
* Best for simple conditions.

---

## 8. Common Mistakes

❌ Forgetting the `:`.

```java id="g5r2xw"
(condition) ? value1
```

✔️ Correct

```java id="f8t4ny"
(condition) ? value1 : value2;
```

---

❌ Using the ternary operator for very complex logic.

✔️ Use `if-else` when the logic is lengthy or difficult to read.

---

## 📝 30-Second Revision

* `?:` is the ternary operator.
* It is a shortcut for `if-else`.
* Uses three operands.
* Syntax: `(condition) ? trueValue : falseValue`
* Best for simple decision-making.


## 1. Concepts

### What is the Ternary Operator?

The **ternary operator (`?:`)** is a shorthand way of writing an `if-else` statement.

It is called **ternary** because it uses **three operands**:

* Condition
* Value if the condition is `true`
* Value if the condition is `false`

---

### Syntax

```java id="2m7qkx"
result = (condition) ? value1 : value2;
```

If the condition is `true`, `value1` is returned.

Otherwise, `value2` is returned.

---

## 2. Why?

The ternary operator makes simple `if-else` statements shorter and more readable.

Instead of writing:

```java id="m0n3zp"
if (age >= 18)
    result = "Adult";
else
    result = "Minor";
```

You can write:

```java id="n5y4dr"
result = (age >= 18) ? "Adult" : "Minor";
```

---

## 3. Code Explained

### Example 1

```java id="n8v4jy"
int age = 20;

String result = (age >= 18) ? "Adult" : "Minor";

System.out.println(result);
```

**Output**

```text id="d8z1tr"
Adult
```

---

### Example 2

```java id="m6w2qk"
int num = 8;

String result = (num % 2 == 0) ? "Even" : "Odd";

System.out.println(result);
```

**Output**

```text id="s4p8nx"
Even
```

---

## 4. Key Differences

| `if-else`                     | Ternary Operator (`?:`)    |
| ----------------------------- | -------------------------- |
| Multiple lines                | Single line                |
| Better for complex logic      | Best for simple conditions |
| Uses `if` and `else` keywords | Uses `?` and `:`           |

Example:

```java id="j3f6mt"
if (x > y)
    max = x;
else
    max = y;
```

Equivalent to:

```java id="t5r9cv"
max = (x > y) ? x : y;
```

---

## 5. Interview Questions

### Q1. What is the ternary operator?

**Answer:**

The ternary operator is a shorthand way of writing a simple `if-else` statement.

---

### Q2. Why is it called a ternary operator?

**Answer:**

Because it uses **three operands**:

* Condition
* Value if true
* Value if false

---

### Q3. What is the output?

```java id="j9b7vl"
int a = 10;

System.out.println((a > 5) ? "Yes" : "No");
```

**Answer**

```text id="u1x5ke"
Yes
```

---

### Q4. Can the ternary operator replace every `if-else` statement?

**Answer:**

No.

It is best suited for **simple** `if-else` conditions.

---

## 6. Practice

### Practice 1

Write a program to find the larger of two numbers using the ternary operator.

---

### Practice 2

Write a program to check whether a number is even or odd using the ternary operator.

---

### Practice 3

Predict the output.

```java id="x7m3bz"
int marks = 35;

String result = (marks >= 35) ? "Pass" : "Fail";

System.out.println(result);
```

---

## 7. Key Takeaways

* The ternary operator is a shortcut for `if-else`.
* Syntax:

```java id="e2v8pn"
(condition) ? value1 : value2;
```

* Returns one value based on the condition.
* Best for simple conditions.

---

## 8. Common Mistakes

❌ Forgetting the `:`.

```java id="g5r2xw"
(condition) ? value1
```

✔️ Correct

```java id="f8t4ny"
(condition) ? value1 : value2;
```

---

❌ Using the ternary operator for very complex logic.

✔️ Use `if-else` when the logic is lengthy or difficult to read.

---

## 📝 30-Second Revision

* `?:` is the ternary operator.
* It is a shortcut for `if-else`.
* Uses three operands.
* Syntax: `(condition) ? trueValue : falseValue`
* Best for simple decision-making.
