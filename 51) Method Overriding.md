# 📘 51) Method Overriding

## 1. What is Method Overriding?

**Method Overriding** is the process where a **child class provides its own implementation of a method that already exists in the parent class.**

The child class **overrides** the parent's method.

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
B obj = new B();
obj.show();
```

**Output**

```text
Inside B
```

The child class method is executed instead of the parent class method.

---

# 2. Why Do We Use Method Overriding?

Method overriding allows a child class to **change or customize the behavior inherited from the parent class**.

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

Different child classes can provide their own implementation of the same method.

---

# 3. Rules for Method Overriding

* The method name must be the **same**.
* The parameter list must be the **same**.
* The return type must be the **same** (or compatible).
* The child method **cannot reduce the visibility** of the parent method.
* Only **inherited methods** can be overridden.

---

# 4. `@Override` Annotation

```java
@Override
public void show() {

}
```

The `@Override` annotation tells the compiler that you intend to override a parent method.

### Advantages

* Detects mistakes at compile time.
* Makes code easier to read.
* Recommended but **not mandatory**.

---

# 5. Method Overloading vs Method Overriding

| Method Overloading        | Method Overriding      |
| ------------------------- | ---------------------- |
| Same class                | Parent & Child classes |
| Same method name          | Same method name       |
| Different parameters      | Same parameters        |
| Compile-time polymorphism | Run-time polymorphism  |

---

# 6. Interview Questions

### Q1. What is method overriding?

**Answer:**

Method overriding is when a child class provides its own implementation of a method already defined in the parent class.

---

### Q2. Which annotation is commonly used while overriding?

**Answer:**

`@Override`

---

### Q3. Can constructors be overridden?

**Answer:**

No. Constructors are not inherited, so they cannot be overridden.

---

### Q4. What is the difference between overloading and overriding?

**Answer:**

Overloading uses methods with the same name but different parameters in the same class, while overriding redefines an inherited method in a child class.

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
* Use `@Override` for better readability and compiler checks.
* Method overriding is the foundation of **run-time polymorphism**.

---

## 📝 30-Second Revision

* Child class redefines a parent class method.
* Method name and parameters must be the same.
* `@Override` is recommended.
* Constructors cannot be overridden.
* Used to achieve **run-time polymorphism**.
