# 📘 Video 2 - JDK Installation & Setup

## 1. Concepts

### What is JDK?

**JDK (Java Development Kit)** is a collection of tools required to develop Java applications.

It helps you:

* Write Java programs
* Compile Java programs
* Run Java programs
* Test Java applications

---

### Why do we install the JDK?

A computer does not understand Java by default.

Installing the JDK provides the necessary tools to create and execute Java programs.

Without the JDK, you cannot develop Java applications.

---

### JDK Includes

* Java Compiler (`javac`)
* Java Launcher (`java`)
* JShell (introduced in Java 9)
* Other development tools

> **Note:** We'll learn about JRE and JVM in detail later in the playlist.

---

## 2. Why?

### Why do we need to install the JDK?

Imagine buying a new laptop.

It doesn't know anything about Java.

The JDK gives your computer the tools needed to understand, compile, and run Java programs.

Without installing the JDK, Java development is not possible.

---

## 3. Commands Used

### Check Java Version

```bash
java -version
```

Displays the installed Java runtime version.

---

### Check Java Compiler

```bash
javac -version
```

Displays the installed Java compiler version.

---

### Compile a Java Program

```bash
javac Hello.java
```

Compiles the Java source file.

---

### Run a Java Program

```bash
java Hello
```

Runs the compiled Java program.

> **Note:** Do **not** include `.java` while running the program.

---

## 4. Interview Questions

### Q1. What does JDK stand for?

**Answer:**

Java Development Kit.

---

### Q2. What is JDK?

**Answer:**

JDK is a collection of tools used to develop, compile, and run Java programs.

---

### Q3. Why do we install the JDK?

**Answer:**

Because it provides the tools required to create and execute Java applications.

---

### Q4. Which command checks the installed Java version?

**Answer:**

```bash
java -version
```

---

### Q5. Which command checks the Java compiler version?

**Answer:**

```bash
javac -version
```

---

## 5. Practice

### Practice 1

Open Terminal (or Command Prompt) and run:

```bash
java -version
```

Observe the installed Java version.

---

### Practice 2

Run:

```bash
javac -version
```

Verify that the Java compiler is installed.

---

### Practice 3

Think about the difference:

* `java`
* `javac`

Try explaining it in one sentence.

---

## 6. Key Takeaways

* JDK stands for **Java Development Kit**.
* JDK contains tools required for Java development.
* `javac` compiles Java source code.
* `java` runs the compiled Java program.
* Install the JDK before writing Java programs.

---

## 7. Common Mistakes

❌ Thinking `java` and `javac` are the same.

✔️ `javac` **compiles** the program.

✔️ `java` **runs** the program.

---

❌ Running:

```bash
java Hello.java
```

✔️ Correct:

```bash
java Hello
```

---

❌ Assuming JDK is only a compiler.

✔️ JDK is a **development kit** that contains multiple tools, including the Java compiler.

---

## 💡 Interview Insight

Freshers are commonly asked:

* What is JDK?
* What does JDK stand for?
* Difference between `java` and `javac`.
* Which command compiles a Java program?
* Which command runs a Java program?

---

## 📝 30-Second Revision

* JDK = Java Development Kit.
* Install the JDK to develop Java applications.
* `javac` compiles Java source code.
* `java` runs the compiled program.
* `java -version` checks the Java version.
* `javac -version` checks the compiler version.
