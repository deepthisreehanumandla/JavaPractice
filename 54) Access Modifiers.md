<img width="2720" height="1348" alt="image" src="https://github.com/user-attachments/assets/75e21688-3f35-441b-8fa0-7ae66b998472" />

## 1. What are Access Modifiers?

**Access Modifiers** are keywords used to **control the accessibility (visibility)** of classes, methods, variables, and constructors.

They help in:

* Data Hiding
* Encapsulation
* Security
* Controlling access to class members

Java has **4 access modifiers**:

* `public`
* `protected`
* `default` *(package-private)*
* `private`

---

# 2. Types of Access Modifiers

## A. `public`

A `public` member can be accessed **from anywhere**.

```java
public class Student {

    public void display() {
        System.out.println("Hello");
    }

}
```

✔ Accessible from any class and any package.

---

## B. `private`

A `private` member can be accessed **only within the same class**.

```java
class Student {

    private int age;

}
```

Used to hide data and implement **encapsulation**.

---

## C. `protected`

A `protected` member can be accessed:

* Within the same package.
* By subclasses, even if they are in different packages.

```java
protected void show() {

}
```

---

## D. Default (Package-Private)

If no access modifier is specified, Java uses **default** access.

```java
class Student {

    void print() {

    }

}
```

Accessible **only within the same package**.

---

# 3. Accessibility Table

| Access Modifier | Same Class | Same Package | Subclass (Different Package) | Different Package |
| --------------- | :--------: | :----------: | :--------------------------: | :---------------: |
| `public`        |      ✅     |       ✅      |               ✅              |         ✅         |
| `protected`     |      ✅     |       ✅      |               ✅              |         ❌         |
| `default`       |      ✅     |       ✅      |               ❌              |         ❌         |
| `private`       |      ✅     |       ❌      |               ❌              |         ❌         |

---

# 4. Access Modifiers for Classes

A **top-level class** can have only:

* `public`
* `default` (no modifier)

Examples:

```java
public class Demo {

}
```

```java
class Test {

}
```

❌ `private` and `protected` **cannot** be used with top-level classes.

---

# 5. Why Do We Use Access Modifiers?

* Protect important data.
* Hide implementation details.
* Implement encapsulation.
* Improve security.
* Control access to members.

---

# 6. Interview Questions

### Q1. How many access modifiers are there in Java?

**Answer:**

Four: `public`, `protected`, `default`, and `private`.

---

### Q2. Which access modifier has the highest accessibility?

**Answer:**

`public`

---

### Q3. Which access modifier has the least accessibility?

**Answer:**

`private`

---

### Q4. Which modifier is mainly used for encapsulation?

**Answer:**

`private`

---

### Q5. Can a top-level class be declared as `private`?

**Answer:**

No. A top-level class can only be `public` or `default`.

---

# 7. Practice

```java
class Student {

    private String name;

    public void setName(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }

}
```

```java
public class Main {

    public static void main(String[] args) {

        Student s = new Student();

        s.setName("Deepthi");

        System.out.println(s.getName());

    }

}
```

**Output**

```text
Deepthi
```

---

# 8. Key Takeaways

* Access modifiers control the visibility of members.
* `public` → Accessible everywhere.
* `protected` → Same package + subclasses.
* `default` → Same package only.
* `private` → Same class only.
* Top-level classes can only be `public` or `default`.

---

## 📝 30-Second Revision

* **public** → Everywhere.
* **protected** → Same package + subclasses.
* **default** → Same package only.
* **private** → Same class only.
* `private` supports encapsulation.
* Top-level classes → `public` or `default` only.
