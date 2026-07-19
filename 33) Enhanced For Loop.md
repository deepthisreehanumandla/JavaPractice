# 📘 33) Enhanced For Loop

## 1. Concepts

### What is an Enhanced For Loop?

The **Enhanced For Loop (for-each loop)** is used to iterate through every element of an array without using an index.

Syntax:

```java
for(dataType variable : array)
{
    // code
}
```

---

## 2. Why?

Compared to a normal `for` loop:

```java
for(int i = 0; i < nums.length; i++)
```

the enhanced for loop is:

* Shorter
* Easier to read
* Less error-prone

---

## 3. Code Explained

Normal for loop:

```java
int[] nums = {10,20,30};

for(int i = 0; i < nums.length; i++)
{
    System.out.println(nums[i]);
}
```

Enhanced for loop:

```java
int[] nums = {10,20,30};

for(int n : nums)
{
    System.out.println(n);
}
```

Output:

```text
10
20
30
```

---

## 4. Key Differences

### Normal For Loop vs Enhanced For Loop

| Normal For                | Enhanced For                 |
| ------------------------- | ---------------------------- |
| Uses index                | No index                     |
| Can modify index          | Cannot access index directly |
| Best when index is needed | Best for simple traversal    |

---

## 5. Interview Questions

### Q1. What is an Enhanced For Loop?

**Answer:**

It is a loop used to traverse arrays (or collections) without using an index.

---

### Q2. When should you use an Enhanced For Loop?

**Answer:**

When you only need to read every element and do not require the index.

---

### Q3. Can you access the index in an Enhanced For Loop?

**Answer:**

No.

---

## 6. Practice

Print all elements of:

```java
int[] nums = {5,10,15,20};
```

using:

* Normal for loop
* Enhanced for loop

---

## 7. Key Takeaways

* Enhanced for loop simplifies array traversal.
* No need to manage an index.
* Best for reading elements.

---

## 8. Common Mistakes

❌ Trying to access an index inside an enhanced for loop.

✔️ The loop directly provides the element, not its index.

---

❌ Using an enhanced for loop when the index is required.

✔️ Use a normal `for` loop if you need the position of each element.

---

## 📝 30-Second Revision

* Enhanced for loop = For-each loop.
* Used to traverse arrays.
* No index required.
* Simple and readable.
* Use a normal `for` loop when you need the index.
