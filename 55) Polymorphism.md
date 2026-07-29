# 📘 55) Polymorphism

## 1. What is Polymorphism?

**Polymorphism** means **"many forms."**

In Java, the same method or object can behave differently depending on the situation.

Example:

* A person can be a **student**, **employee**, or **customer**.
* Same person → Different roles.

Similarly, in Java, the same method call can perform different actions.

---

# 2. Types of Polymorphism

Java supports two types:

### 1. Compile-Time Polymorphism

Achieved using **Method Overloading**.

The compiler decides which method to call.

```java
class Calculator {

    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

}
```

---

### 2. Run-Time Polymorphism

Achieved using **Method Overriding**.

The JVM decides which method to execute while the program is running.

```java
class Animal {

    void sound() {
        System.out.println("Animal Sound");
    }

}

class Dog extends Animal {

    @Override
    void sound() {
        System.out.println("Dog Barks");
    }

}
```

---

# 3. Why Do We Need Polymorphism?

Polymorphism helps us:

* Write flexible code.
* Reuse existing code.
* Reduce duplication.
* Make programs easier to maintain.

---

# 4. Compile-Time vs Run-Time Polymorphism

| Compile-Time        | Run-Time                                       |
| ------------------- | ---------------------------------------------- |
| Method Overloading  | Method Overriding                              |
| Decided by Compiler | Decided by JVM                                 |
| Faster              | Slightly slower due to dynamic method dispatch |

---

# 5. Real-Life Example

Think about a **Remote Control**.

You press the **Power** button.

* TV → Turns on the TV.
* AC → Turns on the AC.
* Speaker → Turns on the Speaker.

Same action, different behavior.

This is the idea behind **polymorphism**.

---

# 6. Interview Questions

### Q1. What is polymorphism?

**Answer:**

Polymorphism means **one interface, many forms**, allowing the same method or object to behave differently.

---

### Q2. How many types of polymorphism are there in Java?

**Answer:**

Two:

* Compile-Time Polymorphism
* Run-Time Polymorphism

---

### Q3. Which feature provides compile-time polymorphism?

**Answer:**

Method Overloading.

---

### Q4. Which feature provides run-time polymorphism?

**Answer:**

Method Overriding.

---

### Q5. Which is decided by the JVM?

**Answer:**

Run-Time Polymorphism.

---

# 7. Practice

```java
class Animal {

    void sound() {
        System.out.println("Animal Sound");
    }

}

class Dog extends Animal {

    @Override
    void sound() {
        System.out.println("Dog Barks");
    }

}

public class Main {

    public static void main(String[] args) {

        Animal obj = new Dog();

        obj.sound();

    }

}
```

**Output**

```text
Dog Barks
```

---

# 8. Key Takeaways

* Polymorphism means **many forms**.
* Compile-Time Polymorphism → Method Overloading.
* Run-Time Polymorphism → Method Overriding.
* Improves flexibility and code reusability.
* Run-time polymorphism is resolved by the JVM.

---

## 📝 30-Second Revision

* **Polymorphism = Many Forms**
* **Compile-Time → Method Overloading**
* **Run-Time → Method Overriding**
* Compiler resolves overloading.
* JVM resolves overriding.
* Makes code flexible and reusable.
