# 📘 52) Method Overriding

## 1. What is Method Overriding?

**Method Overriding** is an OOP feature where a **child class provides its own implementation of a method that is already defined in the parent class.**

The child class **overrides** the inherited method.

Example:

```java
class A {

    public void show() {
        System.out.println("Inside A");
    }

}

class B extends A {

    @Override
    public void show() {
        System.out.println("Inside B");
    }

}
```

```java
public class Main {

    public static void main(String[] args) {

        B obj = new B();
        obj.show();

    }

}
```

**Output**

```text
Inside B
```

---

# 2. Why Do We Use Method Overriding?

Method overriding allows a child class to **change the behavior** of an inherited method according to its own requirements.

Example:

```java
class Animal {

    void sound() {
        System.out.println("Animal makes a sound");
    }

}

class Dog extends Animal {

    @Override
    void sound() {
        System.out.println("Dog barks");
    }

}
```

Now every child class can have its own implementation of `sound()`.

---

# 3. Rules for Method Overriding

* Method name must be the **same**.
* Parameters must be the **same**.
* Return type must be the **same** (or covariant).
* The child method **cannot have more restrictive access** than the parent method.
* Only **inherited methods** can be overridden.
* Constructors **cannot** be overridden.
* Static methods are **hidden**, not overridden.

---

# 4. `@Override` Annotation

```java
@Override
public void show() {

}
```

The `@Override` annotation tells the compiler that the method is intended to override a parent class method.

### Benefits

* Detects mistakes at compile time.
* Improves code readability.
* Recommended in Java.

---

# 5. Method Overloading vs Method Overriding

| Method Overloading        | Method Overriding      |
| ------------------------- | ---------------------- |
| Same class                | Parent & Child classes |
| Same method name          | Same method name       |
| Different parameters      | Same parameters        |
| Compile-time Polymorphism | Run-time Polymorphism  |

---

# 6. Interview Questions

### Q1. What is method overriding?

**Answer:**

Method overriding is when a child class provides a new implementation of an inherited method.

---

### Q2. Which annotation is used for overriding?

**Answer:**

`@Override`

---

### Q3. Can constructors be overridden?

**Answer:**

No. Constructors are not inherited.

---

### Q4. Can static methods be overridden?

**Answer:**

No. Static methods are **method hidden**, not overridden.

---

### Q5. Why is method overriding important?

**Answer:**

It allows child classes to provide their own implementation of inherited methods and is the basis of **run-time polymorphism**.

---

# 7. Practice

```java
class Vehicle {

    void start() {
        System.out.println("Vehicle Started");
    }

}

class Bike extends Vehicle {

    @Override
    void start() {
        System.out.println("Bike Started");
    }

}

public class Main {

    public static void main(String[] args) {

        Bike obj = new Bike();
        obj.start();

    }

}
```

**Output**

```text
Bike Started
```

---

# 8. Key Takeaways

* Method overriding occurs between a **parent** and **child** class.
* The child class provides a new implementation of an inherited method.
* Use `@Override` for better readability and compiler checking.
* Constructors cannot be overridden.
* Static methods are hidden, not overridden.
* Method overriding enables **run-time polymorphism**.

---

## 📝 30-Second Revision

* Child class redefines a parent class method.
* Method name and parameters must be the same.
* Use `@Override`.
* Constructors cannot be overridden.
* Static methods are hidden, not overridden.
* Foundation of **run-time polymorphism**.
