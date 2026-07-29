# 📘 52) Packages

## 1. What is a Package?

A **package** is a way to **group related classes and interfaces** in Java.

It helps organize code and avoids naming conflicts between classes.

Example:

```java id="p1k8m4"
package tools;

public class Calculator {

}
```

Here, `Calculator` belongs to the `tools` package.

---

# 2. Why Do We Use Packages?

Packages help to:

* Organize large projects.
* Avoid class name conflicts.
* Improve code reusability.
* Control access using access modifiers.

---

# 3. Types of Packages

### A. Built-in Packages

These are provided by Java.

Examples:

```java id="n8f5xr"
java.lang
java.util
java.io
java.sql
```

---

### B. User-defined Packages

Packages created by programmers.

Example:

```java id="v2d4ks"
package student;

public class Student {

}
```

---

# 4. Creating a Package

```java id="x7h1ba"
package mypackage;

public class Demo {

    public void show() {
        System.out.println("Hello");
    }

}
```

The `package` statement must be the **first line** of the Java file.

---

# 5. Importing a Package

To use a class from another package:

```java id="c5w9te"
import mypackage.Demo;
```

or

```java id="g9q3lr"
import mypackage.*;
```

Example:

```java id="f3k7zo"
import mypackage.Demo;

public class Main {

    public static void main(String[] args) {

        Demo obj = new Demo();
        obj.show();

    }

}
```

---

# 6. Package Naming Convention

Package names are written in **lowercase**.

Examples:

```java id="z6m2pn"
com.telusko
com.company.project
java.util
```

---

# 7. Interview Questions

### Q1. What is a package?

**Answer:**

A package is a collection of related classes and interfaces used to organize Java programs.

---

### Q2. Why are packages used?

**Answer:**

To organize code, avoid naming conflicts, improve reusability, and manage access.

---

### Q3. Which statement is used to include classes from another package?

**Answer:**

The `import` statement.

---

### Q4. Where should the `package` statement be written?

**Answer:**

It should be the **first statement** in the Java source file.

---

# 8. Practice

Create a package named:

```java id="d4v7qm"
package college;
```

Create a class:

```java id="a8n6xy"
public class Student {

    public void display() {
        System.out.println("Student Details");
    }

}
```

Import it into another class and call `display()`.

---

# 9. Key Takeaways

* Packages organize related classes.
* They help avoid naming conflicts.
* Java provides built-in and user-defined packages.
* Use `package` to declare a package.
* Use `import` to access classes from another package.

---

## 📝 30-Second Revision

* Package = Collection of related classes/interfaces.
* `package` → Declares a package.
* `import` → Uses classes from another package.
* Built-in packages → `java.util`, `java.io`, `java.sql`.
* User-defined packages help organize large projects.
