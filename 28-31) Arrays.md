# 📘 Videos 28–31 - Arrays (Need, Creation, Multi-Dimensional, Jagged & Drawbacks)

## 1. Concepts

### What is an Array?

An **array** is a collection of elements of the **same data type** stored under a single variable name.

Instead of creating multiple variables, we use an array to store related data in an organized manner.

---

### Need for an Array

Without arrays:

```java
int mark1;
int mark2;
int mark3;
...
```

With arrays:

```java
int[] marks = new int[100];
```

Arrays make the code:

* Shorter
* Easier to read
* Easier to maintain

---

### Creating an Array

#### Method 1

```java
int[] nums = new int[5];
```

* Creates an array of size **5**.
* Default values are assigned.

#### Method 2

```java
int[] nums = {10, 20, 30, 40, 50};
```

* Java automatically determines the size.
* Elements are initialized immediately.

---

### Index

Each element in an array is accessed using an **index**.

```java
System.out.println(nums[0]);
```

* Index starts from **0**.

---

### Multi-Dimensional Array (2D)

A **2D array** is an array containing other arrays.

Example:

```java
int[][] nums = new int[3][4];
```

Think of it as a **table** with rows and columns.

---

### Jagged Array

A **Jagged Array** is a 2D array where each row can have a **different number of columns**.

Example:

```java
int[][] nums = new int[3][];

nums[0] = new int[3];
nums[1] = new int[2];
nums[2] = new int[4];
```

---

### 3D Array

A **3D array** is an array of 2D arrays.

Example:

```java
int[][][] nums = new int[2][3][4];
```

It is used when data has three dimensions.

---

## 2. Why?

Arrays help us store multiple values of the same data type using one variable.

They reduce code repetition and make programs easier to manage.

---

## 3. Key Differences

### Variables vs Array

| Variables                 | Array                           |
| ------------------------- | ------------------------------- |
| One value per variable    | Multiple values in one variable |
| More code                 | Less code                       |
| Hard to manage large data | Easy to manage large data       |

---

### Creating an Array

| `new int[5]`            | `{10,20,30,40,50}`          |
| ----------------------- | --------------------------- |
| Specify size            | Java determines size        |
| Default values assigned | Values assigned immediately |

---

### 1D vs 2D vs Jagged

| 1D Array | 2D Array         | Jagged Array                     |
| -------- | ---------------- | -------------------------------- |
| One row  | Rows and columns | Rows with different column sizes |

---

## 4. Default Values

| Data Type     | Default Value |
| ------------- | ------------- |
| int           | 0             |
| double        | 0.0           |
| boolean       | false         |
| char          | '\u0000'      |
| String/Object | null          |

---

## 5. Drawbacks of Arrays

* Fixed size (cannot be changed after creation).
* Can store only one data type.
* Insertion and deletion are costly because elements may need to be shifted.

---

## 6. Interview Questions

### Q1. Why do we need arrays?

**Answer:**

To store multiple values of the same data type using a single variable in an organized manner.

---

### Q2. What is an index?

**Answer:**

An index is the position of an element in an array. It starts from **0**.

---

### Q3. What is the difference between a 2D array and a jagged array?

**Answer:**

A 2D array has the same number of columns in every row, whereas a jagged array allows different rows to have different numbers of columns.

---

### Q4. Can we increase the size of an array?

**Answer:**

No. Once an array is created, its size is fixed.

---

### Q5. What are the main drawbacks of arrays?

**Answer:**

* Fixed size
* Same data type only
* Costly insertion and deletion

---

## 7. Practice

### Practice 1

Create an integer array of size 5 and print all its elements.

---

### Practice 2

Create a 2D array with 3 rows and 4 columns.

---

### Practice 3

Create a jagged array where each row has a different number of elements.

---

## 8. Key Takeaways

* Arrays store multiple values of the same data type.
* Arrays use **zero-based indexing**.
* A 2D array consists of rows and columns.
* A jagged array allows different row sizes.
* Array size is fixed after creation.

---

## 📝 30-Second Revision

* Array → Stores multiple values of the same data type.
* Index starts from **0**.
* `new int[5]` → Size specified.
* `{...}` → Values initialized directly.
* 2D Array → Same columns in every row.
* Jagged Array → Different columns in different rows.
* Drawbacks → Fixed size, one data type, costly insertion/deletion.
