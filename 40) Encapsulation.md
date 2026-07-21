# 📘 40) Encapsulation

## 1. Concepts

### What is Encapsulation?

**Encapsulation** is the process of **wrapping data (variables) and methods into a single unit (class)** while **restricting direct access to the data**.

Instead of allowing direct access to variables, we use **private variables** and provide access through **public methods (getters and setters)**.

Example:

```java id="3q1wme"
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

Without encapsulation:

```java id="yewr4d"
student.age = -10;
```

Anyone can assign invalid values.

With encapsulation:

```java id="3gr4kp"
student.setAge(20);
```

The class controls how data is accessed and modified.

This improves:

* Data security
* Data validation
* Code maintainability

---

## 3. Code Explained

Private variable:

```java id="50mzgz"
private int age;
```

Cannot be accessed directly from outside the class.

Setter:

```java id="ycvxiv"
public void setAge(int age) {
    this.age = age;
}
```

Used to assign a value.

Getter:

```java id="p9jb3u"
public int getAge() {
    return age;
}
```

Used to read the value.

---

## 4. Key Differences

### Public Variable vs Private Variable

| Public                   | Private                            |
| ------------------------ | ---------------------------------- |
| Accessible from anywhere | Accessible only inside the class   |
| Less secure              | More secure                        |
| No control over values   | Can validate values before storing |

---

## 5. Interview Questions

### Q1. What is encapsulation?

**Answer:**

Encapsulation is wrapping data and methods into a single class while restricting direct access to the data.

---

### Q2. Why do we make variables private?

**Answer:**

To protect data and control how it is accessed or modified.

---

### Q3. How do we access private variables?

**Answer:**

Using public getter and setter methods.

---

## 6. Practice

Create a class `Employee` with:

* `private int salary`

Create:

* `setSalary()`
* `getSalary()`

Use them in `main()`.

---

## 7. Key Takeaways

* Encapsulation protects data.
* Variables are usually declared `private`.
* Access is provided using getters and setters.
* Improves security and maintainability.

---

## 8. Common Mistakes

❌ Declaring important data as `public`.

✔️ Use `private` and expose it through methods.

---

❌ Accessing private variables directly.

✔️ Use getter and setter methods.

---

## 📝 30-Second Revision

* Encapsulation = Data hiding.
* Variables → `private`.
* Access → Getters & Setters.
* Protects data and improves code quality.
