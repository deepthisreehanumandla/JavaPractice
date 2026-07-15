# 📘 Video 17, 18 & 19 - Need for Loop, While Loop & Do-While Loop

## 1. Concepts

### What is a Loop?

A **loop** is used to execute the same block of code repeatedly until a condition becomes false.

Instead of writing the same statement multiple times, we use a loop.

---

### What is a While Loop?

A **while loop** checks the condition **before** executing the loop body.

If the condition is `false` initially, the loop will **not execute even once**.

**Syntax**

```java
while (condition) {
    // code
}
```

---

### What is a Do-While Loop?

A **do-while loop** executes the loop body **first** and checks the condition **afterwards**.

Therefore, the loop executes **at least once**, even if the condition is false.

**Syntax**

```java
do {
    // code
} while (condition);
```

---

## 2. Why?

Loops help us:

* Avoid writing repetitive code.
* Make programs shorter and easier to maintain.
* Execute a task multiple times automatically.

Use:

* **while** → When the number of iterations is unknown.
* **do-while** → When the code must execute at least once.

---

## 3. Code Explained

### While Loop

```java
int i = 1;

while (i <= 5) {
    System.out.println("Hi");
    i++;
}
```

**Output**

```text
Hi
Hi
Hi
Hi
Hi
```

Steps:

* Initialize `i`
* Check condition
* Execute code
* Increment `i`
* Repeat until the condition becomes false.

---

### While Loop (Condition False Initially)

```java
int i = 10;

while (i <= 5) {
    System.out.println("Hi");
}
```

**Output**

```text
(No Output)
```

The condition is checked first, so the loop never executes.

---

### Do-While Loop

```java
int i = 10;

do {
    System.out.println("Hi");
} while (i <= 5);
```

**Output**

```text
Hi
```

The body executes once before checking the condition.

---

### Nested While Loop

```java
int i = 1;

while (i <= 3) {

    int j = 1;

    while (j <= 2) {
        System.out.println("Hi");
        j++;
    }

    i++;
}
```

**Output**

```text
Hi
Hi
Hi
Hi
Hi
Hi
```

The inner loop executes completely for each iteration of the outer loop.

---

## 4. Key Differences

### While vs Do-While

| While Loop              | Do-While Loop                     |
| ----------------------- | --------------------------------- |
| Condition checked first | Condition checked after execution |
| May execute zero times  | Executes at least once            |
| Entry-controlled loop   | Exit-controlled loop              |

---

### Need for Loop vs Without Loop

| Without Loop        | With Loop                          |
| ------------------- | ---------------------------------- |
| Repeated statements | Repeated execution using one block |
| More code           | Less code                          |
| Harder to maintain  | Easier to maintain                 |

---

## 5. Interview Questions

### Q1. Why do we use loops?

**Answer:**

To avoid writing repetitive code and execute a block multiple times.

---

### Q2. What is a while loop?

**Answer:**

A loop that checks the condition before executing the body.

---

### Q3. What is a do-while loop?

**Answer:**

A loop that executes the body first and checks the condition afterwards.

---

### Q4. Why is the while loop called an entry-controlled loop?

**Answer:**

Because the condition is checked before entering the loop.

---

### Q5. Why is the do-while loop called an exit-controlled loop?

**Answer:**

Because the condition is checked after executing the loop body.

---

## 6. Practice

### Practice 1

Print numbers from **1 to 10** using a while loop.

---

### Practice 2

Print `"Java"` **5 times** using a do-while loop.

---

### Practice 3

Predict the output.

```java
int i = 5;

while (i < 5) {
    System.out.println(i);
}
```

---

### Practice 4

Predict the output.

```java
int i = 5;

do {
    System.out.println(i);
} while (i < 5);
```

---

## 7. Key Takeaways

* Loops reduce code repetition.
* Every loop needs:

  * Initialization
  * Condition
  * Increment/Decrement
* `while` checks the condition first.
* `do-while` executes once before checking the condition.
* Nested loops are loops inside another loop.

---

## 8. Common Mistakes

❌ Forgetting to increment the loop variable.

```java
while (i <= 5) {
    System.out.println(i);
}
```

This creates an **infinite loop**.

---

❌ Expecting a while loop to execute at least once.

✔️ It may execute **zero times**.

---

❌ Forgetting the semicolon after `while` in a do-while loop.

```java
do {
    // code
} while (condition);
```

The semicolon is **mandatory**.

---

## 📝 30-Second Revision

* Loop → Repeats a block of code.
* `while` → Checks condition first (Entry-controlled).
* `do-while` → Executes once before checking (Exit-controlled).
* Every loop has:

  * Initialization
  * Condition
  * Increment/Decrement
* Forgetting to update the loop variable can cause an infinite loop.
