# 📘 42) this Keyword

## 1. Concepts

### What is `this`?

`this` is a **reference variable** that refers to the **current object**.

It is mainly used to distinguish **instance variables** from **local variables (or method/constructor parameters)** when they have the same name.

Example:

```java id="6g8xmw"
class Student {

    private int age;

    public void setAge(int age) {
        this.age = age;
    }

}
```

Here:

* `this.age` → Instance variable
* `age` → Parameter (local variable)

---

## 2. Why?

Without `this`:

```java id="g95trg"
public void setAge(int age) {
    age = age;
}
```

Nothing happens because the parameter assigns its value to itself.

Using `this`:

```java id="68djlwm"
public void setAge(int age) {
    this.age = age;
}
```

The parameter value is assigned to the object's variable.

---

## 3. Code Explained

```java id="t7xkrn"
class Student {

    private String name;

    public void setName(String name) {
        this.name = name;
    }

}
```

Suppose:

```java id="rx1m72"
Student s1 = new Student();

s1.setName("Deepthi");
```

Java interprets:

```java id="76wpgj"
this.name = name;
```

as:

```text id="2ftcst"
s1.name = "Deepthi";
```

---

## 4. Key Differences

### `this.variable` vs Local Variable

| `this.variable`               | Local Variable                      |
| ----------------------------- | ----------------------------------- |
| Belongs to the current object | Belongs to the current method       |
| Stored in the object          | Exists only during method execution |
| Accessed using `this`         | Accessed directly                   |

---

## 5. Interview Questions

### Q1. What is the `this` keyword?

**Answer:**

`this` is a reference to the current object.

---

### Q2. Why do we use `this`?

**Answer:**

To distinguish instance variables from local variables or parameters with the same name.

---

### Q3. Is `this` a keyword?

**Answer:**

Yes.

---

### Q4. Can `this` be used in a static method?

**Answer:**

No.

Static methods belong to the class, not to any specific object, so there is no current object for `this` to refer to.

---

## 6. Practice

Create a class:

```java id="kx2jps"
class Employee {

    private String name;

    public void setName(String name) {
        this.name = name;
    }

}
```

Create an object and assign the name.

---

## 7. Key Takeaways

* `this` refers to the current object.
* Used when parameter names and instance variable names are the same.
* Commonly used in setters and constructors.
* Makes code clearer and avoids ambiguity.

---

## 8. Common Mistakes

❌ Forgetting `this` when parameter and variable names are the same.

```java id="7t3x8v"
name = name;
```

This only assigns the parameter to itself.

---

✔️ Correct:

```java id="jlrxh4"
this.name = name;
```

Assigns the parameter value to the object's variable.

---

## 📝 30-Second Revision

* `this` → Refers to the current object.
* Used to differentiate instance variables from local variables.
* Frequently used in setters and constructors.
* Cannot be used in a static method.
