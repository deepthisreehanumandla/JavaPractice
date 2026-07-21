# 📘 41) Getters & Setters

## 1. Concepts

### What are Getters and Setters?

**Getters** and **Setters** are public methods used to access and modify **private variables** of a class.

They are the most common way to implement **encapsulation** in Java.

Example:

```java
class Student {

    private int age;

    public void setAge(int age) {
        this.age = age;
    }

    public int getAge() {
        return age;
    }

}
```

---

## 2. Why?

Since private variables cannot be accessed directly from outside the class, getters and setters provide a controlled way to read and modify them.

This allows:

* Data security
* Data validation
* Better maintainability

---

## 3. Code Explained

### Private Variable

```java
private int age;
```

Cannot be accessed directly outside the class.

---

### Setter

```java
public void setAge(int age) {
    this.age = age;
}
```

* Used to assign or update a value.
* Usually does not return anything (`void`).

---

### Getter

```java
public int getAge() {
    return age;
}
```

* Used to retrieve the value.
* Returns the variable.

---

### Using Getter & Setter

```java
Student s1 = new Student();

s1.setAge(20);

System.out.println(s1.getAge());
```

**Output**

```text
20
```

---

## 4. Key Differences

### Getter vs Setter

| Getter            | Setter                 |
| ----------------- | ---------------------- |
| Reads a value     | Updates a value        |
| Returns data      | Usually returns `void` |
| Starts with `get` | Starts with `set`      |

---

### Direct Access vs Getter & Setter

| Direct Access        | Getter & Setter        |
| -------------------- | ---------------------- |
| Less secure          | More secure            |
| No validation        | Validation possible    |
| Breaks encapsulation | Supports encapsulation |

---

## 5. Interview Questions

### Q1. What is a Getter?

**Answer:**

A getter is a public method used to return the value of a private variable.

---

### Q2. What is a Setter?

**Answer:**

A setter is a public method used to assign or update the value of a private variable.

---

### Q3. Why do we use Getters and Setters?

**Answer:**

To access private variables safely while maintaining encapsulation.

---

### Q4. Can a class have only a Getter?

**Answer:**

Yes.

If the value should only be read and not modified.

---

### Q5. Can a class have only a Setter?

**Answer:**

Yes.

If the value only needs to be updated and not read directly.

---

## 6. Practice

Create a class `Employee` with:

```java
private String name;
private double salary;
```

Create:

* `setName()`
* `getName()`
* `setSalary()`
* `getSalary()`

Create an object and print the values.

---

## 7. Key Takeaways

* Getters read private variables.
* Setters update private variables.
* They help implement encapsulation.
* Validation can be added inside setter methods.

---

## 8. Common Mistakes

❌ Accessing private variables directly.

```java
employee.salary = 50000;
```

✔️ Use:

```java
employee.setSalary(50000);
```

---

❌ Returning a value from a setter.

✔️ Setters usually return `void`.

---

## 📝 30-Second Revision

* Getter → Reads a private variable.
* Setter → Updates a private variable.
* Both are public methods.
* Used to implement encapsulation and protect data.
