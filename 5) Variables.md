# 📘 Video 5 - Variables

## 1. Concepts

### What is a Variable?

A **variable** is a named memory location used to store data.

The value stored in a variable can change during program execution.

---

### Syntax

```java
dataType variableName = value;
```

Example:

```java
int num = 10;
```

* `int` → Data type
* `num` → Variable name
* `10` → Value

---

## 2. Why?

Variables allow us to store values and reuse them whenever required.

Instead of writing the same value repeatedly, we store it in a variable and use the variable name.

Example:

Without Variable:

```java
System.out.println(10);
System.out.println(10);
```

With Variable:

```java
int num = 10;

System.out.println(num);
System.out.println(num);
```

---

## 3. Code Explained

```java
public class Demo {
    public static void main(String[] args) {

        int num = 10;

        System.out.println(num);

    }
}
```

| Code  | Meaning                        |
| ----- | ------------------------------ |
| `int` | Data type                      |
| `num` | Variable name                  |
| `=`   | Assignment operator            |
| `10`  | Value assigned to the variable |

---

## 4. Interview Questions

### Q1. What is a variable?

**Answer:**

A variable is a named memory location used to store data.

---

### Q2. Why do we use variables?

**Answer:**

Variables help store and reuse data in a program.

---

### Q3. What is the syntax for declaring a variable?

**Answer:**

```java
dataType variableName = value;
```

---

## 5. Practice

### Practice 1

Create a variable named `age` and store `20`.

---

### Practice 2

Create a variable named `marks` and store `95`.

---

### Practice 3

Print the value of both variables.

---

## 6. Key Takeaways

* A variable stores data.
* Every variable has a name.
* Every variable has a data type.
* Values can be changed during program execution.

---

## 7. Common Mistakes

❌ Using a variable without declaring it.

❌ Giving two variables the same name in the same scope.

❌ Forgetting to assign a value before using the variable.

---

## 📝 30-Second Revision

* Variable = Named memory location.
* Syntax: `dataType variableName = value;`
* Variables store and reuse data.
* Every variable has a name, data type, and value.
