# 📘 44) Default vs Parameterized Constructor

## 1. Concepts

### Default Constructor

A **default constructor** is a constructor that **does not accept any parameters**.

Example:

```java id="8d7kpl"
class Student {

    Student() {
        System.out.println("Default Constructor");
    }

}
```

Object creation:

```java id="5up49o"
Student s1 = new Student();
```

---

### Parameterized Constructor

A **parameterized constructor** accepts one or more parameters to initialize an object with different values.

Example:

```java id="dztgb4"
class Student {

    String name;
    int age;

    Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

}
```

Object creation:

```java id="13rr7m"
Student s1 = new Student("Deepthi", 20);
```

Now the object is initialized during creation.

---

## 2. Why?

Without a parameterized constructor:

```java id="9dd4vt"
Student s1 = new Student();

s1.name = "Deepthi";
s1.age = 20;
```

With a parameterized constructor:

```java id="e6nrr4"
Student s1 = new Student("Deepthi", 20);
```

This is shorter, cleaner, and ensures the object starts with valid values.

---

## 3. Code Explained

```java id="jlwmn8"
class Student {

    String name;
    int age;

    Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

}
```

When Java executes:

```java id="kqn1gz"
Student s1 = new Student("Deepthi", 20);
```

It automatically calls:

```java id="7wnizj"
Student("Deepthi", 20);
```

and initializes the object's fields.

---

## 4. Key Differences

### Default vs Parameterized Constructor

| Default Constructor                              | Parameterized Constructor              |
| ------------------------------------------------ | -------------------------------------- |
| No parameters                                    | One or more parameters                 |
| Initializes with default or fixed values         | Initializes with user-provided values  |
| Same values for every object (if coded that way) | Different values for different objects |

---

## 5. Interview Questions

### Q1. What is a default constructor?

**Answer:**

A constructor that does not accept any parameters.

---

### Q2. What is a parameterized constructor?

**Answer:**

A constructor that accepts parameters to initialize an object.

---

### Q3. Why do we use parameterized constructors?

**Answer:**

To initialize objects with different values at the time of creation.

---

### Q4. Can a class have both a default and a parameterized constructor?

**Answer:**

Yes. This is an example of **constructor overloading**.

---

## 6. Practice

Create a class:

```java id="vt5hcu"
class Employee {

    String name;
    int id;

    Employee(String name, int id) {
        this.name = name;
        this.id = id;
    }

}
```

Create two objects with different values and print their details.

---

## 7. Key Takeaways

* Default constructor → No parameters.
* Parameterized constructor → Accepts parameters.
* Constructors initialize objects.
* Multiple constructors in the same class are called **constructor overloading**.

---

## 8. Common Mistakes

❌ Thinking Java always creates a default constructor.

✔️ Java provides a default constructor **only if you don't write any constructor yourself**.

---

❌ Forgetting `this` when parameter names and instance variable names are the same.

```java id="65d20l"
name = name;
```

✔️ Correct:

```java id="nq9tji"
this.name = name;
```

---

## 📝 30-Second Revision

* Default constructor → No parameters.
* Parameterized constructor → Accepts parameters.
* Used to initialize objects.
* A class can have multiple constructors (constructor overloading).
