# 📘 45–46) Naming Convention & Anonymous Object

## 1. Naming Convention

### What are Naming Conventions?

Naming conventions are **recommended guidelines** for naming classes, variables, methods, packages, and constants in Java. They make code easier to read, understand, and maintain.

### Standard Naming Rules

#### Class Names

* Use **PascalCase** (capitalize the first letter of every word).

```java
class Student
class BankAccount
class EmployeeDetails
```

---

#### Variable Names

* Use **camelCase** (first word lowercase, subsequent words capitalized).

```java
int age;
String studentName;
double accountBalance;
```

---

#### Method Names

* Use **camelCase**.
* Method names usually describe an action (verb).

```java
displayDetails();
calculateTotal();
getName();
setAge();
```

---

#### Constant Names

* Use **UPPER_CASE** with underscores.

```java
final double PI = 3.14159;
final int MAX_SIZE = 100;
```

---

#### Package Names

* Always use **lowercase**.

```java
com.telusko
java.util
student.management
```

---

## 2. Anonymous Object

### What is an Anonymous Object?

An **anonymous object** is an object that is **created without storing its reference in a variable**.

Normally:

```java
Student s1 = new Student();
s1.show();
```

Anonymous object:

```java
new Student().show();
```

Here, the object is created, the `show()` method is called, and then the object becomes eligible for garbage collection because no reference points to it.

---

## 3. Why Use Anonymous Objects?

Use an anonymous object when:

* The object is needed only once.
* You don't need to reuse it later.
* It makes the code shorter.

---

## 4. Normal Object vs Anonymous Object

### Normal Object

```java
Student s1 = new Student();
s1.show();
s1.show();
```

The same object can be reused multiple times.

---

### Anonymous Object

```java
new Student().show();
```

The object is used only once and cannot be accessed again.

---

## 5. Comparison

| Normal Object                     | Anonymous Object                          |
| --------------------------------- | ----------------------------------------- |
| Has a reference variable          | No reference variable                     |
| Can be reused                     | Cannot be reused                          |
| Exists until no references remain | Eligible for garbage collection after use |
| Best for multiple operations      | Best for one-time use                     |

---

## 6. Interview Questions

### Q1. What is an anonymous object?

**Answer:**

An object created without assigning it to a reference variable.

---

### Q2. Why do we use anonymous objects?

**Answer:**

When an object is required only once, creating an anonymous object reduces unnecessary variables.

---

### Q3. Can we call multiple methods using the same anonymous object?

**Answer:**

No. Once the statement finishes, you lose the reference to that object. To reuse an object, store it in a reference variable.

---

### Q4. Are naming conventions mandatory in Java?

**Answer:**

No. They are recommended best practices that improve code readability and consistency.

---

## 7. Practice

### Naming Convention

Create a class:

```java
class EmployeeDetails {

    String employeeName;
    int employeeId;

    void displayDetails() {

    }

}
```

---

### Anonymous Object

```java
class Demo {

    void show() {
        System.out.println("Hello Java");
    }

    public static void main(String[] args) {
        new Demo().show();
    }

}
```

**Output**

```text
Hello Java
```

---

## 8. Key Takeaways

* Follow Java naming conventions to write clean and readable code.
* Classes → PascalCase.
* Variables & Methods → camelCase.
* Constants → UPPER_CASE.
* Packages → lowercase.
* Anonymous objects are useful when an object is needed only once.

---

## 📝 30-Second Revision

* **Class** → `StudentDetails`
* **Variable** → `studentName`
* **Method** → `displayDetails()`
* **Constant** → `MAX_LIMIT`
* **Package** → `com.example.app`
* **Anonymous Object** → `new Student().show();`
* Use anonymous objects for one-time operations.
