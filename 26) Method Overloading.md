# 📘 Video 26 - Method Overloading

## 1. Concepts

### What is Method Overloading?

**Method Overloading** means creating **multiple methods with the same name but different parameters** in the same class.

Java decides which method to execute based on the arguments passed.

---

### Valid Overloading

```java
class Calculator {

    void add(int a, int b) { }

    void add(int a, int b, int c) { }

}
```

---

## 2. Why?

Method overloading lets us perform **similar operations** using the same method name while accepting different inputs.

This makes code easier to read and maintain.

---

## 3. Code Explained

```java
class Calculator {

    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

}
```

Calling:

```java
Calculator c = new Calculator();

System.out.println(c.add(10, 20));
System.out.println(c.add(10, 20, 30));
```

**Output**

```text
30
60
```

Java selects the correct method based on the number (or type) of parameters.

---

## 4. Key Differences

### Method vs Method Overloading

| Method             | Method Overloading                          |
| ------------------ | ------------------------------------------- |
| One method         | Multiple methods                            |
| One parameter list | Different parameter lists                   |
| One implementation | Multiple implementations with the same name |

---

### Valid vs Invalid Overloading

| Valid                          | Invalid                       |
| ------------------------------ | ----------------------------- |
| Different number of parameters | Same name and same parameters |
| Different parameter types      | Only changing the method name |

---

## 5. Interview Questions

### Q1. What is method overloading?

**Answer:**

Method overloading is having multiple methods with the same name but different parameter lists.

---

### Q2. Can overloaded methods have the same name?

**Answer:**

Yes.

---

### Q3. What must be different in overloaded methods?

**Answer:**

Their parameter list (number or type of parameters).

---

### Q4. Is changing only the return type considered method overloading?

**Answer:**

No.

The parameter list must be different.

---

## 6. Practice

### Practice 1

Create overloaded methods:

```java
add(int a, int b)
add(int a, int b, int c)
```

---

### Practice 2

Write overloaded methods for:

```text
multiply(int, int)
multiply(int, int, int)
```

---

### Practice 3

Identify whether these are overloaded:

```java
add(int a)
add(int a, int b)
```

```java
add(int a)
add(int a)
```

---

## 7. Key Takeaways

* Method overloading uses the **same method name**.
* The **parameter list must be different**.
* Java chooses the correct method based on the arguments.
* It improves readability and flexibility.

---

## 8. Common Mistakes

❌ Thinking changing only the return type is overloading.

```java
int add(int a)
double add(int a)
```

This is **not valid**.

---

❌ Writing two methods with the same name and identical parameters.

```java
add(int a, int b)
add(int a, int b)
```

This causes a compilation error.

---

## 📝 30-Second Revision

* Method overloading = Same method name, different parameters.
* Parameter list must change.
* Return type alone cannot overload a method.
* Java picks the correct method based on the arguments passed.
