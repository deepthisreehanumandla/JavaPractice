# 📘 Video 3 - JShell

## 1. Concepts

### What is JShell?

**JShell** is Java's interactive command-line tool introduced in **Java 9**.

It allows you to write and execute Java statements **without creating a `.java` file**.

JShell is mainly used for:

* Learning Java
* Testing small pieces of code
* Experimenting with Java features
* Quick debugging

---

### Why was JShell introduced?

Before Java 9, every Java program required:

1. Creating a `.java` file
2. Compiling it
3. Running it

For small experiments, this process was slow.

JShell makes learning and testing much faster.

---

## 2. Why?

### Why use JShell?

Imagine you just want to check:

```java
10 + 20
```

Without JShell, you would have to:

* Create a Java file
* Write a class
* Write the `main()` method
* Compile
* Run

With JShell, simply type:

```java
10 + 20
```

and press **Enter**.

JShell immediately displays the result.

---

## 3. Common Commands

### Start JShell

```bash
jshell
```

---

### Print Output

```java
System.out.println("Hello Java");
```

---

### Perform Calculations

```java
10 + 20
```

Output:

```text
30
```

---

### Create a Variable

```java
int age = 20;
```

Display the value:

```java
age
```

Output:

```text
20
```

---

### Exit JShell

```java
/exit
```

---

## 4. Interview Questions

### Q1. What is JShell?

**Answer:**

JShell is Java's interactive command-line tool that allows us to execute Java code without creating a `.java` file.

---

### Q2. In which Java version was JShell introduced?

**Answer:**

Java 9.

---

### Q3. Why do we use JShell?

**Answer:**

To quickly test and execute Java code without creating, compiling, and running a Java file.

---

### Q4. Is JShell mainly used for developing large Java applications?

**Answer:**

No.

It is mainly used for learning, experimenting, and testing small pieces of code.

---

## 5. Practice

### Practice 1

Start JShell:

```bash
jshell
```

---

### Practice 2

Execute:

```java
System.out.println("Hello Java");
```

---

### Practice 3

Create a variable:

```java
int num = 50;
```

Display it:

```java
num
```

---

### Practice 4

Perform:

```java
25 + 75
```

Observe the output.

---

## 6. Key Takeaways

* JShell was introduced in **Java 9**.
* It is an interactive Java shell.
* No `.java` file is required.
* No manual compilation is required.
* Best for learning and testing small programs.

---

## 7. Common Mistakes

❌ Thinking JShell replaces Java files.

✔️ JShell is mainly for quick testing and learning.

---

❌ Using JShell for large projects.

✔️ Large applications should be developed using Java source files (`.java`).

---

❌ Forgetting how to exit JShell.

✔️ Use:

```java
/exit
```

---

## 💡 Interview Insight

Freshers may be asked:

* What is JShell?
* Which Java version introduced JShell?
* Why was JShell introduced?
* Difference between JShell and a `.java` program.

---

## 📝 30-Second Revision

* JShell = Interactive Java Shell.
* Introduced in **Java 9**.
* Execute Java code without creating a `.java` file.
* Useful for learning and quick testing.
* Start using `jshell`.
* Exit using `/exit`.
