# 📘 Video 21 - Which Loop to Use

## 1. Concepts

### Which Loop Should You Use?

Java provides three loops:

* `while`
* `do-while`
* `for`

All three can perform repeated execution, but each is best suited for different situations.

---

### `while` Loop

Use a **while loop** when the **number of iterations is not known**.

The condition is checked **before** execution.

Example:

```java
int i = 1;

while (i <= 5) {
    System.out.println(i);
    i++;
}
```

---

### `do-while` Loop

Use a **do-while loop** when the code **must execute at least once**.

The condition is checked **after** execution.

Example:

```java
int i = 10;

do {
    System.out.println(i);
} while (i <= 5);
```

**Output**

```text
10
```

---

### `for` Loop

Use a **for loop** when the **number of iterations is known**.

Example:

```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

---

## 2. Why?

Choosing the right loop makes code:

* Easier to read
* Easier to maintain
* More suitable for the problem

All three loops can often solve the same problem, but one is usually a better choice.

---

## 3. Code Explained

### Known Number of Iterations

```java
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
}
```

✔️ Best choice: **for loop**

---

### Unknown Number of Iterations

```java
while (userChoice != 0) {
    // continue until user exits
}
```

✔️ Best choice: **while loop**

---

### Execute At Least Once

```java
do {
    System.out.println("Menu");
} while (choice != 0);
```

✔️ Best choice: **do-while loop**

---

## 4. Key Differences

| `for`                                                | `while`                                 | `do-while`                        |
| ---------------------------------------------------- | --------------------------------------- | --------------------------------- |
| Known iterations                                     | Unknown iterations                      | Execute at least once             |
| Initialization, condition and increment in one place | Initialization usually outside the loop | Condition checked after execution |
| Entry-controlled                                     | Entry-controlled                        | Exit-controlled                   |

---

## 5. Interview Questions

### Q1. Which loop should be used when the number of iterations is known?

**Answer:**

`for` loop.

---

### Q2. Which loop is used when the number of iterations is unknown?

**Answer:**

`while` loop.

---

### Q3. Which loop executes at least once?

**Answer:**

`do-while` loop.

---

### Q4. Can all three loops perform the same task?

**Answer:**

Yes. They can often solve the same problem, but one may be more appropriate depending on the situation.

---

## 6. Practice

### Practice 1

Which loop would you use to print numbers from **1 to 100**?

---

### Practice 2

Which loop would you use to repeatedly ask the user for input until they enter **0**?

---

### Practice 3

Which loop would you use to display a menu that should appear at least once?

---

## 7. Key Takeaways

* Use `for` when the number of iterations is known.
* Use `while` when the number of iterations is unknown.
* Use `do-while` when the loop must execute at least once.
* Choose the loop that best matches the problem.

---

## 8. Common Mistakes

❌ Using a `do-while` loop when the code should not execute if the condition is false.

✔️ Use a `while` loop instead.

---

❌ Using a `while` loop when the number of iterations is fixed.

✔️ A `for` loop is usually cleaner.

---

❌ Thinking one loop is "better" than the others.

✔️ Each loop has its own use case.

---

## 📝 30-Second Revision

* `for` → Known number of iterations.
* `while` → Unknown number of iterations.
* `do-while` → Executes at least once.
* `for` and `while` are **entry-controlled** loops.
* `do-while` is an **exit-controlled** loop.
