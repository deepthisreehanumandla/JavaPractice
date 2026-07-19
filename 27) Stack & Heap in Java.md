# 📘 27) Stack & Heap in Java

## 1. Concepts

### What is Stack Memory?

**Stack Memory** stores:

* Method calls
* Local variables
* Reference variables

Every time a method is called, a **stack frame** is created. When the method finishes, its stack frame is removed automatically.

---

### What is Heap Memory?

**Heap Memory** stores:

* Objects
* Instance variables (variables inside objects)

Objects remain in heap memory until they are no longer referenced and are removed by the **Garbage Collector (GC)**.

---

## 2. Why?

Java separates memory into **Stack** and **Heap** for efficient memory management.

* **Stack** manages method execution.
* **Heap** manages dynamically created objects.

---

## 3. Code Explained

```java
class Student {
    String name;
}

public class Demo {

    public static void main(String[] args) {

        Student s1 = new Student();
        s1.name = "Deepthi";

    }

}
```

### Memory Representation

### Stack Memory

```text
main()

s1  ─────────────┐
                 │
```

### Heap Memory

```text
Student Object
--------------
name = "Deepthi"
```

`s1` is stored in the **Stack**.

The actual `Student` object is stored in the **Heap**.

---

## 4. Local vs Instance Variables

```java
class Student {

    String name;          // Instance Variable

    void study() {

        int hours = 2;    // Local Variable

    }

}
```

### Instance Variable

* Belongs to an object.
* Stored in **Heap Memory**.
* Exists as long as the object exists.

---

### Local Variable

* Declared inside a method.
* Stored in **Stack Memory**.
* Exists only while the method is executing.

---

## 5. Key Differences

### Stack vs Heap

| Stack                                        | Heap                         |
| -------------------------------------------- | ---------------------------- |
| Stores method calls                          | Stores objects               |
| Stores local variables                       | Stores instance variables    |
| Faster memory                                | Larger memory                |
| Automatically cleared after method execution | Cleared by Garbage Collector |

---

### Local Variable vs Instance Variable

| Local Variable                 | Instance Variable              |
| ------------------------------ | ------------------------------ |
| Inside a method                | Inside a class                 |
| Stored in Stack                | Stored in Heap                 |
| Exists during method execution | Exists while the object exists |

---

## 6. Interview Questions

### Q1. What is Stack Memory?

**Answer:**

Stack Memory stores method calls, local variables, and reference variables.

---

### Q2. What is Heap Memory?

**Answer:**

Heap Memory stores objects and their instance variables.

---

### Q3. Where are objects stored?

**Answer:**

Objects are stored in **Heap Memory**.

---

### Q4. Where are local variables stored?

**Answer:**

Local variables are stored in **Stack Memory**.

---

### Q5. What is the Garbage Collector?

**Answer:**

The Garbage Collector automatically removes objects from Heap Memory when they are no longer referenced.

---

## 7. Practice

### Practice 1

Identify where each is stored:

```java
Student s1 = new Student();
```

* `s1`
* `Student Object`

---

### Practice 2

Identify:

```java
int age = 20;
```

Inside a method.

Where is `age` stored?

---

### Practice 3

Identify:

```java
class Student {

    String name;

}
```

Where is `name` stored after creating an object?

---

## 8. Key Takeaways

* Stack stores method calls, local variables, and reference variables.
* Heap stores objects and instance variables.
* Objects are created using `new` and stored in Heap.
* Reference variables point to objects.
* Garbage Collector cleans unused objects from Heap.

---

## 9. Common Mistakes

❌ Thinking reference variables are objects.

✔️ Reference variables store the **reference (address)** of an object.

---

❌ Thinking objects are stored in Stack.

✔️ Objects are always stored in **Heap Memory**.

---

❌ Thinking local variables exist forever.

✔️ Local variables are removed when the method finishes.

---

## 📝 30-Second Revision

* **Stack** → Method calls, local variables, reference variables.
* **Heap** → Objects and instance variables.
* `new` creates an object in Heap.
* Reference variables are stored in Stack and point to Heap objects.
* Local variables live only during method execution.
* Garbage Collector removes unused objects from Heap.
