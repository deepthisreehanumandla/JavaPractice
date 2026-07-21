# 📘 Videos 37–39 - Static Variable, Static Method & Static Block

## 1. Concepts

### Static Variable

A **static variable** belongs to the **class**, not to individual objects.

Only **one copy** exists, and it is shared by all objects.

Example:

```java
class Student {

    String name;
    static String college = "MRU";

}
```

Every `Student` object shares the same `college`.

---

### Static Method

A **static method** belongs to the class and can be called **without creating an object**.

Example:

```java
class Demo {

    static void show() {
        System.out.println("Hello");
    }

}
```

Call:

```java
Demo.show();
```

---

### Static Block

A **static block** executes **only once**, when the class is loaded into memory.

Example:

```java
class Demo {

    static {
        System.out.println("Static Block");
    }

}
```

---

## 2. Why?

Static members are used when a value or method should be **shared by all objects**.

Example:

* Company name
* College name
* PI value
* Utility methods

---

## 3. Key Differences

### Instance Variable vs Static Variable

| Instance Variable            | Static Variable                |
| ---------------------------- | ------------------------------ |
| Belongs to object            | Belongs to class               |
| Each object has its own copy | One copy shared by all objects |
| Access using object          | Access using class name        |

---

### Instance Method vs Static Method

| Instance Method             | Static Method                           |
| --------------------------- | --------------------------------------- |
| Requires object             | No object required                      |
| Can access instance members | Can directly access only static members |

---

## 4. Execution Order

```text
Class Loaded
      ↓
Static Block
      ↓
main()
      ↓
Objects Created
```

---

## 5. Interview Questions

### Q1. What is a static variable?

**Answer:**

A variable that belongs to the class and is shared by all objects.

---

### Q2. Can a static method be called without creating an object?

**Answer:**

Yes.

Example:

```java
Demo.show();
```

---

### Q3. When is a static block executed?

**Answer:**

Once, when the class is loaded into memory.

---

### Q4. Can a static method directly access instance variables?

**Answer:**

No.

It can directly access only static members.

---

## 6. Practice

Create:

* One static variable.
* One instance variable.
* One static method.
* One static block.

Observe the execution order.

---

## 7. Key Takeaways

* Static members belong to the class.
* One copy of a static variable is shared.
* Static methods can be called using the class name.
* Static block executes only once.

---

## 8. Common Mistakes

❌ Thinking every object gets its own static variable.

✔️ Static variables are shared.

---

❌ Calling static methods using objects unnecessarily.

✔️ Prefer:

```java
ClassName.methodName();
```

---

❌ Expecting the static block to execute every time an object is created.

✔️ It executes only once when the class is loaded.

---

## 📝 30-Second Revision

* Static variable → Shared by all objects.
* Static method → Call using class name.
* Static block → Executes once during class loading.
* Static belongs to the class, not the object.
