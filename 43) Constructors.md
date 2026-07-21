# 📘 43) Constructors

## 1. Concepts

### What is a Constructor?

A **constructor** is a special method that is **automatically called when an object is created**.

Its main purpose is to **initialize the object**.

Example:

```java
class Student {

    Student() {
        System.out.println("Object Created");
    }

}
```

When an object is created:

```java
Student s1 = new Student();
```

Output:

```text
Object Created
```

The constructor runs automatically.

---

## 2. Characteristics

* Constructor name must be the **same as the class name**.
* It has **no return type** (not even `void`).
* It is called automatically when an object is created.
* A class can have multiple constructors (Constructor Overloading).

---

## 3. Why?

Instead of assigning values after creating an object:

```java
Student s1 = new Student();

s1.name = "Deepthi";
s1.age = 20;
```

We can initialize the object directly inside the constructor.

---

## 4. Code Explained

```java
class Student {

    String name;

    Student() {
        name = "Deepthi";
    }

}
```

```java
Student s1 = new Student();

System.out.println(s1.name);
```

**Output**

```text
Deepthi
```

The constructor initializes the object automatically.

---

## 5. Key Differences

### Constructor vs Method

| Constructor          | Method                      |
| -------------------- | --------------------------- |
| Same name as class   | Can have any valid name     |
| No return type       | Has a return type or `void` |
| Called automatically | Called explicitly           |
| Initializes objects  | Performs specific tasks     |

---

## 6. Interview Questions

### Q1. What is a constructor?

**Answer:**

A constructor is a special method that is automatically called when an object is created to initialize the object.

---

### Q2. Can a constructor have a return type?

**Answer:**

No.

Not even `void`.

---

### Q3. When is a constructor called?

**Answer:**

Automatically when an object is created using the `new` keyword.

---

### Q4. Can a class have multiple constructors?

**Answer:**

Yes.

This is called **Constructor Overloading**.

---

## 7. Practice

Create a class:

```java
class Car {

    String company;

    Car() {
        company = "Toyota";
    }

}
```

Create an object and print `company`.

---

## 8. Key Takeaways

* Constructor initializes an object.
* Called automatically.
* Name must match the class name.
* Has no return type.
* Supports constructor overloading.

---

## 9. Common Mistakes

❌ Writing:

```java
void Student() {

}
```

This is **not** a constructor.

It is a normal method.

---

❌ Calling a constructor like a normal method.

```java
Student();
```

Constructors are invoked automatically during object creation.

---

## 📝 30-Second Revision

* Constructor = Special method.
* Same name as the class.
* No return type.
* Called automatically.
* Used to initialize objects.
