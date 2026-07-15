# 📘 Video 6 - Data Types

## 1. Concepts

### What is a Data Type?

A **data type** specifies the type of value a variable can store.

It tells Java:

* What kind of data is being stored.
* How much memory should be allocated.

---

### Primitive Data Types

Java has **8 primitive data types**.

| Data Type | Size          | Example      |
| --------- | ------------- | ------------ |
| `byte`    | 1 byte        | `10`         |
| `short`   | 2 bytes       | `1000`       |
| `int`     | 4 bytes       | `25`         |
| `long`    | 8 bytes       | `123456789L` |
| `float`   | 4 bytes       | `12.5f`      |
| `double`  | 8 bytes       | `12.5`       |
| `char`    | 2 bytes       | `'A'`        |
| `boolean` | JVM dependent | `true`       |

---

## 2. Why?

Different kinds of data require different amounts of memory.

Examples:

* Age → `int`
* Population → `long`
* Percentage → `float` / `double`
* Grade → `char`
* Is Passed? → `boolean`

Using the correct data type improves memory usage and program efficiency.

---

## 3. Code Explained

```java
int age = 20;
long population = 1400000000L;
float percentage = 89.5f;
double pi = 3.1415926535;
char grade = 'A';
boolean isPassed = true;
```

| Code                             | Meaning                             |
| -------------------------------- | ----------------------------------- |
| `int age = 20;`                  | Stores an integer value             |
| `long population = 1400000000L;` | Stores a large whole number         |
| `float percentage = 89.5f;`      | Stores a decimal value (float)      |
| `double pi = 3.1415926535;`      | Stores a more precise decimal value |
| `char grade = 'A';`              | Stores a single character           |
| `boolean isPassed = true;`       | Stores a true/false value           |

---

## 4. Interview Questions

### Q1. What is a data type?

**Answer:**

A data type specifies the type of value a variable can store.

---

### Q2. How many primitive data types are there in Java?

**Answer:**

There are **8 primitive data types**.

---

### Q3. Which data type stores:

* Whole numbers → `int`
* Large whole numbers → `long`
* Decimal numbers → `float` / `double`
* Single character → `char`
* True or False → `boolean`

---

### Q4. Which is more precise: `float` or `double`?

**Answer:**

`double`

---

### Q5. Why do we use `f` and `L`?

**Answer:**

* `f` tells Java that a decimal literal is a **float**.
* `L` tells Java that an integer literal is a **long**.

---

## 5. Practice

### Practice 1

Declare variables for:

* Age (`int`)
* Population (`long`)
* Percentage (`float`)
* PI (`double`)
* Grade (`char`)
* Passed (`boolean`)

---

### Practice 2

Identify the data type of:

```java
100
```

```java
100L
```

```java
10.5
```

```java
10.5f
```

```java
'A'
```

```java
true
```

---

## 6. Key Takeaways

* A data type defines what kind of value a variable can store.
* Java has **8 primitive data types**.
* `double` is more precise than `float`.
* Decimal literals are `double` by default.
* Use `f` for `float` and `L` for `long`.

---

## 7. Common Mistakes

❌

```java
float price = 12.5;
```

✔️

```java
float price = 12.5f;
```

---

❌

```java
char grade = "A";
```

✔️

```java
char grade = 'A';
```

---

❌

```java
long num = 5000000000;
```

✔️

```java
long num = 5000000000L;
```

---

## 📝 30-Second Revision

* Data type = Type of value a variable stores.
* Java has **8 primitive data types**.
* `double` is the default for decimal values.
* Use `f` for `float`.
* Use `L` for `long`.
* `char` uses single quotes (`' '`).
* `String` uses double quotes (`" "`).
