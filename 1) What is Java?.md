# 📘 Video 1 - What is Java?

## 1. Concepts

### What is Java?

* Java is a **high-level**, **object-oriented**, and **platform-independent** programming language.
* It was developed by **Sun Microsystems** (now owned by **Oracle**).
* It is used to build desktop applications, web applications, enterprise software, Android applications (legacy), and more.

### Features of Java

* High-Level Language
* Object-Oriented
* Platform Independent
* Secure
* Robust
* Simple
* Portable

---

## 2. Why?

### Why was Java created?

Java was designed with one major goal:

> **Write Once, Run Anywhere (WORA).**

Instead of writing different programs for Windows, Linux, and macOS, Java allows you to write one program that can run on all of them (using the JVM, which we'll learn later).

### Why is Java called a High-Level Language?

Because it is easy for humans to read and write.

Example:

```java
System.out.println("Hello");
```

---

## 3. Code Explained

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

| Part                   | Meaning                                                     |
| ---------------------- | ----------------------------------------------------------- |
| `public`               | Access modifier (accessible from anywhere).                 |
| `class`                | Keyword used to create a class.                             |
| `Hello`                | Class name (identifier).                                    |
| `main()`               | Entry point of every Java program.                          |
| `static`               | Allows the JVM to call `main()` without creating an object. |
| `void`                 | The method does not return any value.                       |
| `String[] args`        | Stores command-line arguments.                              |
| `System.out.println()` | Prints output and moves to the next line.                   |

---

## 4. Interview Questions

### Q1. What is Java?

**Answer:**

Java is a high-level, object-oriented, and platform-independent programming language.

---

### Q2. Who developed Java?

**Answer:**

Sun Microsystems (now Oracle).

---

### Q3. Why is Java platform independent?

**Answer:**

Because Java code is converted into bytecode, which can run on any operating system that has a JVM.

---

### Q4. Where does Java execution begin?

**Answer:**

Execution begins from the `main()` method.

---

### Q5. Why is `main()` static?

**Answer:**

Because the JVM can call it directly without creating an object.

---

## 5. Coding Exercises

### Exercise 1

Print:

```text
Hello Java
```

---

### Exercise 2

Print:

```text
My name is Deepthi.
I am learning Java.
```

---

### Exercise 3

Predict the output:

```java
System.out.print("Hello ");
System.out.println("Java");
```

---

## 6. Key Takeaways

* Java is a high-level, object-oriented, and platform-independent language.
* The `main()` method is the entry point of every Java program.
* `print()` prints on the same line.
* `println()` prints and moves to the next line.
* `public`, `class`, `static`, and `void` are Java keywords.
* `Hello` is an identifier (class name).

---

## 7. Common Mistakes

❌ Thinking `main` is a Java keyword.

✔️ `main` is **not** a keyword. It is the name of the entry-point method.

---

❌ Thinking `print()` and `println()` are the same.

✔️ `println()` moves to the next line, while `print()` does not.

---

❌ Thinking `Hello` is a keyword.

✔️ `Hello` is an **identifier** (class name).

---

## 💡 Interview Insight

Freshers are commonly asked:

* What is Java?
* Why is Java platform independent?
* Explain `public static void main(String[] args)`.
* Difference between `print()` and `println()`.
* What is a keyword?
* What is an identifier?

---

## 📝 30-Second Revision

* Java = High-Level + Object-Oriented + Platform Independent.
* Developed by Sun Microsystems (now Oracle).
* Execution starts from the `main()` method.
* `static` allows the JVM to call `main()` directly.
* `print()` vs `println()`.
* Keywords vs Identifiers.
