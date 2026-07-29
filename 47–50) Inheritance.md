# 📘 47–50) Inheritance (Need, Types & Multiple Inheritance)

## 1. What is Inheritance?

**Inheritance** is an OOP concept where one class acquires the properties and methods of another class.

* The existing class is called the **Parent (Superclass)**.
* The new class is called the **Child (Subclass)**.

It promotes **code reusability** and reduces duplicate code.

Example:

```java
class A {

    void show() {
        System.out.println("Inside A");
    }

}

class B extends A {

}
```

```java
B obj = new B();
obj.show();
```

**Output**

```text
Inside A
```

Here, class `B` inherits the `show()` method from class `A`.

---

# 2. Why Do We Need Inheritance?

Without inheritance:

```java
class Car {

    void start() {
        System.out.println("Car Started");
    }

}

class SportsCar {

    void start() {
        System.out.println("Car Started");
    }

}
```

The same code is duplicated.

With inheritance:

```java
class Car {

    void start() {
        System.out.println("Car Started");
    }

}

class SportsCar extends Car {

}
```

Now `SportsCar` automatically gets the `start()` method.

### Advantages

* Code Reusability
* Less Code Duplication
* Easier Maintenance
* Supports Method Overriding
* Builds Parent–Child Relationships

---

# 3. Types of Inheritance

## A. Single Inheritance

One child inherits from one parent.

```java
class Animal {

}

class Dog extends Animal {

}
```

```
Animal
   ↑
 Dog
```

---

## B. Multilevel Inheritance

A class inherits from another child class.

```java
class Animal {

}

class Dog extends Animal {

}

class Puppy extends Dog {

}
```

```
Animal
   ↑
 Dog
   ↑
Puppy
```

`Puppy` inherits features from both `Dog` and `Animal`.

---

## C. Hierarchical Inheritance

Multiple child classes inherit from the same parent.

```java
class Animal {

}

class Dog extends Animal {

}

class Cat extends Animal {

}
```

```
      Animal
      /    \
    Dog    Cat
```

---

## D. Multiple Inheritance

One child inherits from **multiple parent classes**.

Example (Not Allowed in Java Classes):

```
   A      B
    \    /
      C
```

Java **does not support multiple inheritance with classes** because of the **Diamond Problem**.

Instead, Java supports multiple inheritance using **interfaces**.

---

# 4. Diamond Problem

Suppose:

```text
      A
     / \
    B   C
     \ /
      D
```

If both `B` and `C` have the same method, Java cannot determine which version `D` should inherit.

To avoid this ambiguity, Java **does not allow multiple inheritance with classes**.

---

# 5. `extends` Keyword

The `extends` keyword is used to inherit a class.

```java
class Child extends Parent {

}
```

A subclass inherits:

* Variables
* Methods

Constructors are **not inherited**, but they are called during object creation.

---

# 6. Interview Questions

### Q1. What is inheritance?

**Answer:**

Inheritance is the process by which one class acquires the properties and methods of another class.

---

### Q2. Why is inheritance used?

**Answer:**

To reuse code, reduce duplication, and establish parent-child relationships between classes.

---

### Q3. Which keyword is used for inheritance?

**Answer:**

`extends`

---

### Q4. Does Java support multiple inheritance?

**Answer:**

Java does not support multiple inheritance with classes. It supports it through interfaces.

---

### Q5. What is the Diamond Problem?

**Answer:**

It is the ambiguity that occurs when a class inherits from two parent classes that contain the same method.

---

# 7. Practice

```java
class Animal {

    void eat() {
        System.out.println("Eating...");
    }

}

class Dog extends Animal {

    void bark() {
        System.out.println("Barking...");
    }

}

public class Main {

    public static void main(String[] args) {

        Dog obj = new Dog();

        obj.eat();
        obj.bark();

    }

}
```

**Output**

```text
Eating...
Barking...
```

---

# 8. Key Takeaways

* Inheritance promotes **code reusability**.
* `extends` is used to inherit a class.
* Java supports:

  * Single Inheritance
  * Multilevel Inheritance
  * Hierarchical Inheritance
* Java **does not support multiple inheritance with classes** because of the Diamond Problem.
* Multiple inheritance is possible using **interfaces**.

---

## 📝 30-Second Revision

* Inheritance → One class acquires another class's properties and methods.
* Parent → Superclass.
* Child → Subclass.
* Keyword → `extends`.
* Benefits → Reusability, less duplicate code, easier maintenance.
* Java ❌ Multiple inheritance with classes.
* Java ✅ Multiple inheritance with interfaces.
