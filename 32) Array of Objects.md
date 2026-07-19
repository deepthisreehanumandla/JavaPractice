# 📘 32) Array of Objects

## 1. Concepts

### What is an Array of Objects?

An **Array of Objects** is an array where each element stores the **reference of an object**.

Example:

```java
class Student {
    String name;
    int age;
}

Student[] students = new Student[3];
```

Here, `students` is an array that can hold references to **3 Student objects**.

---

## 2. Why?

Instead of creating multiple object variables:

```java
Student s1 = new Student();
Student s2 = new Student();
Student s3 = new Student();
```

We can manage them using one array:

```java
Student[] students = new Student[3];
```

---

## 3. Code Explained

Create the array:

```java
Student[] students = new Student[3];
```

Create the objects:

```java
students[0] = new Student();
students[1] = new Student();
students[2] = new Student();
```

Assign values:

```java
students[0].name = "Deepthi";
students[0].age = 20;
```

Access values:

```java
System.out.println(students[0].name);
```

---

## 4. Key Differences

### Array of Primitive vs Array of Objects

| Primitive Array               | Object Array              |
| ----------------------------- | ------------------------- |
| Stores values                 | Stores object references  |
| Example: `int[]`              | Example: `Student[]`      |
| Elements are primitive values | Elements refer to objects |

---

## 5. Interview Questions

### Q1. What is an Array of Objects?

**Answer:**

An array that stores references to objects of the same class.

---

### Q2. Does

```java
Student[] students = new Student[3];
```

create 3 objects?

**Answer:**

No.

It creates an array capable of storing **3 object references**.

Objects must be created separately using `new`.

---

### Q3. What is stored inside an object array?

**Answer:**

Object references.

---

## 6. Practice

Create a `Student` class with:

* name
* age

Create an array of 3 students and print their details.

---

## 7. Key Takeaways

* Array of Objects stores object references.
* Objects are created separately.
* Access object members using the dot (`.`) operator.

---

## 8. Common Mistakes

❌ Thinking:

```java
Student[] students = new Student[3];
```

creates 3 objects.

✔️ It only creates an array of references.

---

## 📝 30-Second Revision

* Array of Objects = Array storing object references.
* Objects must be created individually.
* Use `students[i].member` to access object data.
