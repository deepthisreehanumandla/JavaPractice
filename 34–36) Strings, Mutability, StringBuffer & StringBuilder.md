# 📘 Videos 34–36 - Strings, Mutability, StringBuffer & StringBuilder

## 1. Concepts

### What is a String?

A **String** is an object in Java used to store a sequence of characters.

Example:

```java
String name = "Deepthi";
```

Although it looks like a primitive data type, **String is actually a class**.

---

### String Creation

```java
String s1 = "Java";
String s2 = new String("Java");
```

Both create String objects, but they are stored differently in memory.

---

### What is Immutability?

A **String is immutable**, meaning its value **cannot be changed** after it is created.

Example:

```java
String name = "Java";
name = "Programming";
```

The original `"Java"` String is not modified. A **new String object** is created.

---

### Why are Strings Immutable?

* Better security
* Better performance
* Allows String Pool optimization
* Thread-safe

---

### StringBuffer

`StringBuffer` is a mutable class.

It allows modifying the same object without creating new String objects.

Example:

```java
StringBuffer sb = new StringBuffer("Java");

sb.append(" Programming");

System.out.println(sb);
```

Output:

```text
Java Programming
```

---

### StringBuilder

`StringBuilder` is also mutable.

It works like `StringBuffer` but is **not synchronized**, making it faster in single-threaded programs.

---

## 2. Why?

Since Strings are immutable, modifying them repeatedly creates many objects.

`StringBuffer` and `StringBuilder` solve this by modifying the existing object.

---

## 3. Key Differences

### String vs StringBuffer vs StringBuilder

| String                              | StringBuffer         | StringBuilder              |
| ----------------------------------- | -------------------- | -------------------------- |
| Immutable                           | Mutable              | Mutable                    |
| Slower for frequent modifications   | Thread-safe          | Faster but not thread-safe |
| Creates new objects on modification | Modifies same object | Modifies same object       |

---

### StringBuffer vs StringBuilder

| StringBuffer    | StringBuilder    |
| --------------- | ---------------- |
| Synchronized    | Not synchronized |
| Thread-safe     | Not thread-safe  |
| Slightly slower | Faster           |

---

## 4. Interview Questions

### Q1. Is String a primitive data type?

**Answer:**

No. String is a class.

---

### Q2. What does immutable mean?

**Answer:**

Once a String object is created, its value cannot be changed.

---

### Q3. Why is String immutable?

**Answer:**

For security, performance, String Pool optimization, and thread safety.

---

### Q4. Difference between StringBuffer and StringBuilder?

**Answer:**

StringBuffer is thread-safe (synchronized), whereas StringBuilder is faster but not thread-safe.

---

## 5. Practice

Create:

* A String object.
* A StringBuffer object.
* A StringBuilder object.

Append text and observe the output.

---

## 6. Key Takeaways

* String is a class.
* Strings are immutable.
* StringBuffer and StringBuilder are mutable.
* Use StringBuilder for better performance in single-threaded applications.

---

## 7. Common Mistakes

❌ Thinking Strings are primitive data types.

✔️ Strings are objects.

---

❌ Thinking a String changes after modification.

✔️ A new String object is created.

---

## 📝 30-Second Revision

* String → Immutable.
* StringBuffer → Mutable + Thread-safe.
* StringBuilder → Mutable + Faster.
* String is a class, not a primitive type.
