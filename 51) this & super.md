# 📘 51) this & super Method

## 1. What is `this`?

`this` is a **reference keyword** that refers to the **current object** of a class.

It is used to access the current class's variables, methods, and constructors.

Example:

```java
class A {

    int age = 20;

    void show() {
        System.out.println(this.age);
    }

}
```

**Output**

```text
20
```

---

# 2. Uses of `this`

### A. Access Current Class Variables

Used when local variables and instance variables have the same name.

```java
class Student {

    int age;

    Student(int age) {
        this.age = age;
    }

}
```

Here:

* `this.age` → Instance variable
* `age` → Constructor parameter

---

### B. Call Current Class Methods

```java
class Demo {

    void display() {
        System.out.println("Display Method");
    }

    void show() {
        this.display();
    }

}
```

`this.display()` calls another method of the same object.

---

### C. Call Another Constructor

```java
class Student {

    Student() {
        this(20);
        System.out.println("Default Constructor");
    }

    Student(int age) {
        System.out.println(age);
    }

}
```

**Output**

```text
20
Default Constructor
```

> `this()` must be the **first statement** inside a constructor.

---

# 3. What is `super`?

`super` is a **reference keyword** that refers to the **parent class object**.

It is used to access the parent class's variables, methods, and constructors.

---

# 4. Uses of `super`

### A. Access Parent Class Variables

```java
class A {

    int age = 20;

}

class B extends A {

    int age = 30;

    void show() {
        System.out.println(super.age);
    }

}
```

**Output**

```text
20
```

---

### B. Call Parent Class Methods

```java
class A {

    void show() {
        System.out.println("Inside A");
    }

}

class B extends A {

    void show() {
        super.show();
        System.out.println("Inside B");
    }

}
```

**Output**

```text
Inside A
Inside B
```

---

### C. Call Parent Class Constructor

```java
class A {

    A() {
        System.out.println("Parent Constructor");
    }

}

class B extends A {

    B() {
        super();
        System.out.println("Child Constructor");
    }

}
```

**Output**

```text
Parent Constructor
Child Constructor
```

> If you don't write `super()`, Java **automatically inserts it** as the first statement in the child constructor.

---

# 5. `this` vs `super`

| `this`                                         | `super`                                  |
| ---------------------------------------------- | ---------------------------------------- |
| Refers to the current object                   | Refers to the parent class               |
| Accesses current class members                 | Accesses parent class members            |
| Calls current class constructor using `this()` | Calls parent constructor using `super()` |
| Used within the same class                     | Used in inheritance                      |

---

# 6. Interview Questions

### Q1. What does `this` refer to?

**Answer:**

`this` refers to the current object of the class.

---

### Q2. What does `super` refer to?

**Answer:**

`super` refers to the immediate parent class.

---

### Q3. Why do we use `super()`?

**Answer:**

To call the parent class constructor.

---

### Q4. Can `this()` and `super()` be used together in the same constructor?

**Answer:**

No. Both must be the **first statement** in a constructor, so only one can be used.

---

### Q5. What happens if `super()` is not written?

**Answer:**

Java automatically inserts `super()` if the parent class has a no-argument constructor.

---

# 7. Practice

```java
class A {

    A() {
        System.out.println("A Constructor");
    }

}

class B extends A {

    B() {
        super();
        System.out.println("B Constructor");
    }

}

public class Main {

    public static void main(String[] args) {

        B obj = new B();

    }

}
```

**Output**

```text
A Constructor
B Constructor
```

---

# 8. Key Takeaways

* `this` refers to the current object.
* `super` refers to the parent class.
* `this()` calls another constructor in the same class.
* `super()` calls the parent class constructor.
* Both `this()` and `super()` must be the **first statement** in a constructor.
* If `super()` is omitted, Java inserts it automatically (when possible).

---

## 📝 30-Second Revision

* `this` → Current object.
* `this()` → Calls another constructor in the same class.
* `super` → Parent class.
* `super()` → Calls the parent constructor.
* `super.variable` → Parent variable.
* `super.method()` → Parent method.
* Only **one** of `this()` or `super()` can appear first in a constructor.
