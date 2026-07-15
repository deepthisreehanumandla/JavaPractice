# 📘 Video 23 - Class and Object Practical

## 1. Concepts

### Creating a Class

A class defines the **properties (variables)** and **behaviour (methods)** of an object.

Example:

```java
class Student {
    int age;
    String name;
}
```

---

### Creating an Object

An object is created using the `new` keyword.

```java
Student s1 = new Student();
```

Here:

* `Student` → Class
* `s1` → Reference variable
* `new` → Creates a new object
* `Student()` → Constructor

---

### Accessing Variables

Object variables are accessed using the **dot (`.`) operator**.

```java
s1.name = "Deepthi";
s1.age = 20;
```

To display the values:

```java
System.out.println(s1.name);
System.out.println(s1.age);
```

---

## 2. Why?

A class defines the structure only once.

Objects store different values based on that structure.

Example:

```java
Student s1 = new Student();
Student s2 = new Student();
```

Both objects have the same variables, but each stores its own values.

---

## 3. Code Explained

### Define the Class

```java
class Student {
    int age;
    String name;
}
```

The class tells Java that every `Student` object will have:

* `name`
* `age`

---

### Create Objects

```java
Student s1 = new Student();
Student s2 = new Student();
```

Two independent objects are created.

---

### Assign Values

```java
s1.name = "Deepthi";
s1.age = 20;

s2.name = "Rahul";
s2.age = 21;
```

Each object stores its own data.

---

### Print Values

```java
System.out.println(s1.name);
System.out.println(s1.age);

System.out.println(s2.name);
System.out.println(s2.age);
```

---

## 4. Key Differences

### Class vs Object

| Class                         | Object                          |
| ----------------------------- | ------------------------------- |
| Blueprint                     | Instance of a class             |
| Defines variables and methods | Stores actual values            |
| Created once                  | Multiple objects can be created |

---

### Object 1 vs Object 2

| `s1`                              | `s2`                              |
| --------------------------------- | --------------------------------- |
| Independent object                | Independent object                |
| Own copy of variables             | Own copy of variables             |
| Changing `s1` doesn't affect `s2` | Changing `s2` doesn't affect `s1` |

---

## 5. Interview Questions

### Q1. How do you create an object?

**Answer:**

Using the `new` keyword.

Example:

```java
Student s1 = new Student();
```

---

### Q2. How do you access object variables?

**Answer:**

Using the **dot (`.`) operator**.

Example:

```java
s1.name = "Deepthi";
```

---

### Q3. Can two objects have different values?

**Answer:**

Yes.

Each object has its own copy of instance variables.

---

### Q4. Which operator is used to access object members?

**Answer:**

The **dot (`.`) operator**.

---

## 6. Practice

### Practice 1

Create a class named `Car` with:

* `company`
* `model`

Create two objects and assign different values.

---

### Practice 2

Create a class named `Mobile` with:

* `brand`
* `price`

Create two objects and print their values.

---

### Practice 3

Identify the following:

```java
Student s1 = new Student();
```

* Class = ?
* Object = ?
* Reference Variable = ?
* Constructor = ?
* Keyword used to create the object = ?

---

## 7. Key Takeaways

* A class defines the structure.
* Objects store actual data.
* Objects are created using `new`.
* Use the dot (`.`) operator to access variables.
* Multiple objects created from the same class are independent.

---

## 8. Common Mistakes

❌ Thinking `s1` is the object.

✔️ `s1` is a **reference variable**.

---

❌ Thinking all objects share the same values.

✔️ Every object has its own copy of instance variables.

---

❌ Forgetting to use the dot operator.

```java
name = "Deepthi";
```

✔️ Correct

```java
s1.name = "Deepthi";
```

---

## 📝 30-Second Revision

* Create a class to define the structure.
* Create objects using `new`.
* Use `.` to access variables.
* One class can create many independent objects.
* Each object stores its own data.
