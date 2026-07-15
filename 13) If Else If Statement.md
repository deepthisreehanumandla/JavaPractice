# 📘 Video 13 - If Else If Statement

## 1. Concepts

### What is an `if-else if` Statement?

The `if-else if` statement is used when there are **multiple conditions** to check.

Java checks the conditions **from top to bottom**.

* If the first condition is `true`, its block executes.
* Otherwise, Java checks the next condition.
* If none of the conditions are `true`, the `else` block executes.

---

### Syntax

```java id="6p4h8k"
if (condition1) {
    // code
}
else if (condition2) {
    // code
}
else if (condition3) {
    // code
}
else {
    // code
}
```

---

## 2. Why?

`if-else if` helps choose **one block** from many possible options.

It avoids writing multiple separate `if` statements when only one result is needed.

---

## 3. Code Explained

### Example

```java id="m2v9d5"
int marks = 82;

if (marks >= 90)
    System.out.println("Grade A");
else if (marks >= 75)
    System.out.println("Grade B");
else if (marks >= 60)
    System.out.println("Grade C");
else
    System.out.println("Fail");
```

**Output**

```text id="j8w2r6"
Grade B
```

Explanation:

* `marks >= 90` → ❌ False
* `marks >= 75` → ✅ True

Java prints **Grade B** and **stops checking** the remaining conditions.

---

## 4. Key Differences

| `if-else`               | `if-else if`                                  |
| ----------------------- | --------------------------------------------- |
| Used for two choices    | Used for multiple choices                     |
| One `if` and one `else` | One `if`, multiple `else if`, optional `else` |
| Checks one condition    | Checks multiple conditions                    |

---

## 5. Interview Questions

### Q1. When should we use `if-else if`?

**Answer:**

When there are multiple conditions and only one block should execute.

---

### Q2. Does Java check all `else if` conditions?

**Answer:**

No.

Java stops checking as soon as it finds the first `true` condition.

---

### Q3. What is the output?

```java id="g3u7x9"
int x = 25;

if (x > 30)
    System.out.println("A");
else if (x > 20)
    System.out.println("B");
else
    System.out.println("C");
```

**Answer**

```text id="z5r8m1"
B
```

---

### Q4. Is the `else` block mandatory?

**Answer:**

No.

The `else` block is optional.

---

## 6. Practice

### Practice 1

Write a program to print grades based on marks.

* 90 and above → A
* 75–89 → B
* 60–74 → C
* Below 60 → Fail

---

### Practice 2

Predict the output.

```java id="n4k1b7"
int age = 18;

if (age > 18)
    System.out.println("Adult");
else if (age == 18)
    System.out.println("Just Adult");
else
    System.out.println("Minor");
```

---

### Practice 3

Predict the output.

```java id="p9v6j2"
int num = 5;

if (num > 10)
    System.out.println("A");
else if (num > 3)
    System.out.println("B");
else if (num > 1)
    System.out.println("C");
```

---

## 7. Key Takeaways

* `if-else if` is used for multiple conditions.
* Conditions are checked from top to bottom.
* Java executes only the first matching block.
* The `else` block is optional.

---

## 8. Common Mistakes

❌ Writing conditions in the wrong order.

Example:

```java id="h2c8y5"
if (marks >= 35)
```

before

```java id="x7m4p1"
if (marks >= 90)
```

The first condition would become `true` for almost all passing marks.

✔️ Write **more specific conditions first**.

---

❌ Expecting Java to check all conditions.

✔️ Java stops after the first `true` condition.

---

## 📝 30-Second Revision

* `if-else if` → Multiple conditions.
* Conditions are checked from top to bottom.
* Only the first matching block executes.
* `else` is optional.
* Write specific conditions before general ones.
