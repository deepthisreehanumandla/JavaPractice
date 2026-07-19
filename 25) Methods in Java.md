# 📘 Video 25 - Methods in Java

## 1. Concepts

### What is a Method?

A **method** is a block of code that performs a **specific task**.

Instead of writing the same code multiple times, we write it once inside a method and call it whenever needed.

---

### Syntax

```java
class Calculator {

    void add() {
        System.out.println("Addition");
    }

}
```

---

## 2. Why?

Methods help us:

* Avoid code repetition.
* Organize code into smaller tasks.
* Improve readability and reusability.

---

## 3. Code Explained

```java
class Calculator {

    void add() {
        System.out.println(2 + 3);
    }

}
```

Create an object:

```java
Calculator calc = new Calculator();
```

Call the method:

```java
calc.add();
```

**Output**

```text
5
```

---

## 4. Key Differences

### Variables vs Methods

| Variables                    | Methods                         |
| ---------------------------- | ------------------------------- |
| Store data                   | Perform tasks                   |
| Represent the object's state | Represent the object's behavior |

---

### Class vs Object vs Method

| Class     | Object              | Method                         |
| --------- | ------------------- | ------------------------------ |
| Blueprint | Instance of a class | Action performed by the object |

---

## 5. Interview Questions

### Q1. What is a method?

**Answer:**

A method is a block of code that performs a specific task.

---

### Q2. Why do we use methods?

**Answer:**

To avoid code repetition, improve readability, and reuse code.

---

### Q3. How do you call a method?

**Answer:**

Using an object and the dot (`.`) operator.

Example:

```java
calc.add();
```

---

### Q4. Can a class have multiple methods?

**Answer:**

Yes.

---

## 6. Practice

### Practice 1

Create a `Calculator` class with a method `add()`.

---

### Practice 2

Create an object and call the `add()` method.

---

### Practice 3

Identify:

```java
Calculator c = new Calculator();

c.add();
```

* Class = ?
* Object = ?
* Method = ?

---

## 7. Key Takeaways

* A method performs a specific task.
* Methods reduce code duplication.
* Methods are called using objects.
* A class can contain multiple methods.

---

## 8. Common Mistakes

❌ Thinking methods store data.

✔️ Variables store data; methods perform actions.

---

❌ Forgetting to call a method.

Defining a method does **not** execute it.

---

## 📝 30-Second Revision

* Method = Block of code.
* Performs one task.
* Called using `object.method()`.
* Improves code reuse and readability.
