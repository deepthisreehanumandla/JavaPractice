# 📘 Video 22 - Class and Object Theory

## 1. Concepts

### What is OOP?

**Object-Oriented Programming (OOP)** is a programming paradigm that uses **classes** and **objects** to build programs.

Java is primarily an **Object-Oriented Programming (OOP)** language.

---

### What is a Class?

A **class** is a **blueprint** or **template** that defines what an object should have (**variables**) and what it should do (**methods**).

Example:

```java
class Student {
    int age;
    String name;
}
```

The class **does not store actual data**. It only defines the structure.

---

### What is an Object?

An **object** is an **instance of a class**.

Objects store the actual values defined by the class.

Example:

```java
Student s1 = new Student();
```

---

## 2. Why?

Suppose you want to store information for 1,000 students.

Instead of creating thousands of separate variables, you create **one class**:

```java
class Student {
    String name;
    int age;
}
```

Now you can create as many student objects as needed.

```java
Student s1 = new Student();
Student s2 = new Student();
Student s3 = new Student();
```

Each object has its **own copy** of `name` and `age`.

---

## 3. Code Explained

```java
class Student {
    int age;
    String name;
}
```

* `Student` → Class
* `age` and `name` → Instance Variables

---

```java
Student s1 = new Student();
```

* `Student` → Class name
* `s1` → Reference variable
* `new` → Keyword used to create a new object
* `Student()` → Constructor
* `new Student()` → Creates the object

---

```java
Student s2 = new Student();
```

Creates another independent object.

Changing `s1` does **not** affect `s2`.

---

## 4. Key Differences

### Class vs Object

| Class                          | Object                                 |
| ------------------------------ | -------------------------------------- |
| Blueprint or template          | Instance of a class                    |
| Defines the structure          | Stores actual data                     |
| Created once                   | Can create many objects                |
| Contains variables and methods | Has its own values for those variables |

---

### Variables in Class vs Variables in Object

| In Class                               | In Object                |
| -------------------------------------- | ------------------------ |
| Define what data an object should have | Store the actual values  |
| No actual values                       | Actual values are stored |

Example:

```java
class Student {
    String name;
}
```

```java
Student s1 = new Student();
s1.name = "Deepthi";
```

The class defines `name`; the object stores `"Deepthi"`.

---

## 5. Interview Questions

### Q1. What is a class?

**Answer:**

A class is a blueprint or template used to create objects.

---

### Q2. What is an object?

**Answer:**

An object is an instance of a class.

---

### Q3. Why do we create a class before creating an object?

**Answer:**

A class defines the structure of an object. Java uses this structure to know what variables and methods the object should have.

---

### Q4. Can one class create multiple objects?

**Answer:**

Yes. One class can create any number of objects.

---

### Q5. What does `new` do?

**Answer:**

The `new` keyword creates a new object in memory.

---

### Q6. Identify the following:

```java
Student s1 = new Student();
```

**Answer:**

* `Student` → Class
* `s1` → Reference variable
* `new` → Keyword
* `Student()` → Constructor
* `new Student()` → Creates the object

---

## 6. Practice

### Practice 1

Create a class named `Car` with:

* `company`
* `model`

Create two objects of the `Car` class.

---

### Practice 2

Identify the following:

```java
Student s1 = new Student();
```

* Class = ?
* Object = ?
* Reference Variable = ?
* Constructor = ?

---

### Practice 3

True or False?

* A class can create multiple objects.
* Every object has its own copy of instance variables.
* A class stores the actual values of variables.

---

## 7. Key Takeaways

* Java is an OOP language.
* A class is a blueprint.
* An object is an instance of a class.
* One class can create multiple objects.
* Objects have their own data.
* `new` creates an object.
* `s1` stores the reference to the object.

---

## 8. Common Mistakes

❌ Thinking a class stores actual data.

✔️ The class defines the structure; **objects store the actual data**.

---

❌ Thinking all objects share the same variable values.

✔️ Every object has its **own copy** of instance variables.

---

❌ Thinking `s1` is the object.

✔️ `s1` is a **reference variable** that refers to the object.

---

## 📝 30-Second Revision

* OOP = Object-Oriented Programming.
* Class = Blueprint/template.
* Object = Instance of a class.
* Variables define an object's state.
* Methods define an object's behavior.
* `new` creates an object.
* `Student s1 = new Student();`

  * `Student` → Class
  * `s1` → Reference variable
  * `new` → Creates the object
  * `Student()` → Constructor
