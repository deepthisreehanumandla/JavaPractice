# 📘 Video 15 & 16 - Switch Statement (Classic & New Switch)

## 1. Concepts

### What is a Switch Statement?

A **switch statement** is used to execute one block of code from multiple options based on the value of an expression.

Instead of writing multiple `if-else if` statements, `switch` provides a cleaner and more readable approach.

---

### Classic Switch Syntax

```java
switch (day) {

    case 1:
        System.out.println("Monday");
        break;

    case 2:
        System.out.println("Tuesday");
        break;

    default:
        System.out.println("Invalid Day");
}
```

---

### New Switch Expression (Java 14+)

Java introduced a cleaner switch syntax using **`->` (arrow operator)**.

```java
switch (day) {
    case 1 -> System.out.println("Monday");
    case 2 -> System.out.println("Tuesday");
    default -> System.out.println("Invalid Day");
}
```

No `break` is required.

---

## 2. Why?

Switch statements are useful when:

* One variable has multiple fixed values.
* You want cleaner code than long `if-else if` chains.

The **new switch** further reduces boilerplate and avoids accidental fall-through.

---

## 3. Code Explained

### Classic Switch

```java
int day = 3;

switch (day) {
    case 1:
        System.out.println("Monday");
        break;

    case 2:
        System.out.println("Tuesday");
        break;

    case 3:
        System.out.println("Wednesday");
        break;

    default:
        System.out.println("Invalid Day");
}
```

**Output**

```text
Wednesday
```

---

### Fall-through (No `break`)

```java
int day = 1;

switch (day) {
    case 1:
        System.out.println("Monday");

    case 2:
        System.out.println("Tuesday");

    default:
        System.out.println("Invalid");
}
```

**Output**

```text
Monday
Tuesday
Invalid
```

Since there is no `break`, execution continues into the following cases.

---

### New Switch

```java
int day = 2;

switch (day) {
    case 1 -> System.out.println("Monday");
    case 2 -> System.out.println("Tuesday");
    default -> System.out.println("Invalid Day");
}
```

**Output**

```text
Tuesday
```

---

### Switch as an Expression

The new switch can directly return a value.

```java
int day = 2;

String result = switch (day) {
    case 1 -> "Monday";
    case 2 -> "Tuesday";
    default -> "Invalid Day";
};

System.out.println(result);
```

**Output**

```text
Tuesday
```

---

## 4. Key Differences

### `if-else if` vs `switch`

| `if-else if`                           | `switch`                             |
| -------------------------------------- | ------------------------------------ |
| Best for ranges and complex conditions | Best for fixed values                |
| Conditions checked one by one          | Matches a value with a case          |
| More flexible                          | More readable for many fixed options |

---

### Classic Switch vs New Switch

| Classic Switch                         | New Switch                   |
| -------------------------------------- | ---------------------------- |
| Uses `:`                               | Uses `->`                    |
| Requires `break` to avoid fall-through | No `break` required          |
| Can accidentally fall through          | No accidental fall-through   |
| Cannot directly return a value         | Can be used as an expression |

---

## 5. Interview Questions

### Q1. Why do we use a switch statement?

**Answer:**

To choose one block of code from multiple fixed options based on the value of an expression.

---

### Q2. Why is `break` used in the classic switch?

**Answer:**

To stop execution after the matching case and prevent fall-through.

---

### Q3. What is fall-through?

**Answer:**

When `break` is omitted, Java continues executing the following cases.

---

### Q4. What is the advantage of the new switch?

**Answer:**

It is shorter, does not require `break`, prevents accidental fall-through, and can return a value.

---

## 6. Practice

### Practice 1

Write a switch statement to print the day name for values 1–7.

---

### Practice 2

Convert the above program to the new switch syntax using `->`.

---

### Practice 3

Predict the output.

```java
int num = 1;

switch (num) {
    case 1:
        System.out.println("A");
    case 2:
        System.out.println("B");
    default:
        System.out.println("C");
}
```

---

### Practice 4

Predict the output.

```java
int day = 2;

String result = switch (day) {
    case 1 -> "Monday";
    case 2 -> "Tuesday";
    default -> "Invalid";
};

System.out.println(result);
```

---

## 7. Key Takeaways

* `switch` is an alternative to multiple `if-else if` statements.
* Classic switch uses `case`, `:`, and `break`.
* Omitting `break` causes fall-through.
* New switch uses `->`.
* New switch does not require `break`.
* New switch can directly return a value.

---

## 8. Common Mistakes

❌ Forgetting `break` in the classic switch.

✔️ Use `break` unless fall-through is intended.

---

❌ Expecting the new switch to use `break`.

✔️ The arrow syntax (`->`) does not need `break`.

---

❌ Using `switch` for range-based conditions like:

```java
if (marks >= 90)
```

✔️ Use `if-else` for ranges and `switch` for fixed values.

---

## 📝 30-Second Revision

* `switch` selects one block based on a value.
* `case` → Possible value.
* `default` → Runs if no case matches.
* `break` → Stops execution in the classic switch.
* Missing `break` → Fall-through.
* New switch uses `->`.
* New switch doesn't need `break`.
* New switch can return a value.
