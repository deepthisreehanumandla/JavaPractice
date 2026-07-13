# 📘 Video 4 - How Java Works

## 1. Concepts

### Java Program Execution Flow

A Java program goes through the following steps:

```text
Hello.java
     │
     │ javac
     ▼
Hello.class (Bytecode)
     │
     │ JVM
     ▼
Machine Code
     │
     ▼
Output
```

### Source Code

* The code written by the programmer.
* Saved with the `.java` extension.

Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello");
    }
}
```

---

### Compiler (`javac`)

* The Java compiler.
* Converts **source code (`.java`)** into **bytecode (`.class`)**.

Command:

```bash
javac Hello.java
```

---

### Bytecode

* The output produced by the Java compiler.
* Stored inside the `.class` file.
* It is **not** machine code.

Example:

```text
Hello.class
```

---

### JVM (Java Virtual Machine)

* Reads the bytecode.
* Converts bytecode into machine code.
* Executes the program.

> Every operating system has its own JVM.

---

### `main()` Method

* The entry point of every Java program.
* The JVM starts execution from the `main()` method.

---

## 2. Why?

### Why do we need a compiler?

Computers cannot understand Java source code directly.

The compiler translates Java code into bytecode.

---

### Why does Java use Bytecode?

Instead of generating machine code directly, Java generates **bytecode**.

This allows the **same `.class` file** to run on different operating systems using their respective JVMs.

This is why Java follows:

> **Write Once, Run Anywhere (WORA)**

---

### Why do we need the `main()` method?

The JVM needs a starting point.

It begins executing the program from the `main()` method.

Without `main()`, the JVM doesn't know where to start.

---

## 3. Execution Flow

```text
Write Java Program
        │
        ▼
Hello.java
        │
        ▼
javac Hello.java
        │
        ▼
Hello.class (Bytecode)
        │
        ▼
JVM
        │
        ▼
Machine Code
        │
        ▼
Output
```

---

## 4. Interview Questions

### Q1. What is source code?

**Answer:**

The Java code written by the programmer.

---

### Q2. What is the job of `javac`?

**Answer:**

It compiles Java source code into bytecode.

---

### Q3. Which file contains bytecode?

**Answer:**

The `.class` file.

---

### Q4. What is the role of the JVM?

**Answer:**

The JVM converts bytecode into machine code and executes the program.

---

### Q5. Why is Java platform independent?

**Answer:**

Because Java programs are compiled into bytecode, and the same bytecode can run on any operating system that has a JVM.

---

### Q6. Where does Java execution begin?

**Answer:**

Execution begins from the `main()` method.

---

## 5. Practice

### Practice 1

Identify the source code file:

```text
Hello.java
```

---

### Practice 2

Which command compiles the program?

```bash
javac Hello.java
```

---

### Practice 3

Which command runs the program?

```bash
java Hello
```

---

### Practice 4

Explain the difference between:

* `java`
* `javac`

in one sentence.

---

## 6. Key Takeaways

* Java source code is stored in a `.java` file.
* `javac` compiles source code into bytecode.
* Bytecode is stored in the `.class` file.
* The JVM executes bytecode.
* Java is platform independent because of bytecode and the JVM.
* The `main()` method is the entry point of a Java program.

---

## 7. Common Mistakes

❌ Thinking `.class` files contain machine code.

✔️ They contain **bytecode**.

---

❌ Confusing `java` and `javac`.

✔️ `javac` compiles.

✔️ `java` runs.

---

❌ Thinking every operating system uses the same JVM.

✔️ Each operating system has its own JVM implementation.

---

## 💡 Interview Insight

Freshers are commonly asked:

* Explain the Java execution flow.
* What is bytecode?
* What is the difference between `java` and `javac`?
* Why is Java platform independent?
* What is the role of the JVM?
* Why is the `main()` method required?

---

## 📝 30-Second Revision

* Source Code → `.java`
* `javac` → Compiles source code.
* Bytecode → `.class`
* JVM → Executes bytecode.
* `java` → Runs the program.
* Execution starts from `main()`.
* Java is platform independent because of **Bytecode + JVM**.
