# 📘 Video 20 - For Loop

## 1. Concepts

### What is a For Loop?

A **for loop** is used to execute a block of code repeatedly when the **number of iterations is known**.

Unlike a `while` loop, the **initialization, condition, and increment/decrement** are written in one place.

---

### Syntax

```java id="y2v8km"
for (initialization; condition; increment/decrement) {
    // code
}
```

---

## 2. Why?

A `for` loop makes the code:

* Shorter
* More organized
* Easier to read

It is commonly used when we know how many times the loop should run.

---

## 3. Code Explained

### Example 1

```java id="g8p4rt"
for (int i = 1; i <= 5; i++) {
    System.out.println("Hi");
}
```

**Output**

```text id="j5m7qw"
Hi
Hi
Hi
Hi
Hi
```

Explanation:

* `int i = 1` → Initialization (runs once)
* `i <= 5` → Condition (checked before every iteration)
* `i++` → Increment (runs after every iteration)

---

### Example 2

```java id="u3n9xd"
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

**Output**

```text id="h2r8ty"
1
2
3
4
5
```

---

### Nested For Loop

```java id="b6q1mv"
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 2; j++) {
        System.out.println("Hi");
    }
}
```

**Output**

```text id="c4w9zp"
Hi
Hi
Hi
Hi
Hi
Hi
```

The inner loop completes all its iterations before the outer loop continues.

---

## 4. Key Differences

### While vs For

| While Loop                       | For Loop                          |
| -------------------------------- | --------------------------------- |
| Initialization is separate       | Initialization is inside the loop |
| Best when iterations are unknown | Best when iterations are known    |
| Can be longer                    | More compact                      |

---

### For vs Do-While

| For Loop                | Do-While Loop                     |
| ----------------------- | --------------------------------- |
| Condition checked first | Condition checked after execution |
| May execute zero times  | Executes at least once            |

---

## 5. Interview Questions

### Q1. What is a for loop?

**Answer:**

A for loop is used to repeat a block of code when the number of iterations is known.

---

### Q2. What are the three parts of a for loop?

**Answer:**

* Initialization
* Condition
* Increment/Decrement

---

### Q3. What is the output?

```java id="d7x5pf"
for (int i = 1; i <= 3; i++) {
    System.out.println(i);
}
```

**Answer**

```text id="m9t6zk"
1
2
3
```

---

### Q4. Can we write nested for loops?

**Answer:**

Yes. A `for` loop can be placed inside another `for` loop.

---

## 6. Practice

### Practice 1

Print numbers from **1 to 10** using a `for` loop.

---

### Practice 2

Print the multiplication table of **5**.

---

### Practice 3

Predict the output.

```java id="w8k2qy"
for (int i = 5; i >= 1; i--) {
    System.out.println(i);
}
```

---

### Practice 4

Write a nested `for` loop to print:

```text id="x4p8nm"
*
**
***
```

---

## 7. Key Takeaways

* A `for` loop is best when the number of iterations is known.
* It contains:

  * Initialization
  * Condition
  * Increment/Decrement
* All three parts are written in one statement.
* Nested `for` loops are used for repeated patterns.

---

## 8. Common Mistakes

❌ Forgetting to update the loop variable.

This can create an **infinite loop**.

---

❌ Writing the wrong condition.

```java id="v2m7jd"
for (int i = 1; i >= 5; i++)
```

The loop will never execute because the condition is false initially.

---

❌ Using `<=` instead of `<` (or vice versa) when the required number of iterations is different.

Always check whether the last value should be included.

---

## 📝 30-Second Revision

* `for` loop is used when the number of iterations is known.
* Syntax:

```java id="k1q9zr"
for (initialization; condition; increment)
```

* Initialization runs once.
* Condition is checked before every iteration.
* Increment runs after every iteration.
* Nested `for` loops are used for repeated patterns.
