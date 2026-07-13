# 📘 Video 9 - Assignment, Increment & Decrement Operators

## 1. Concepts

### What is an Assignment Operator?

An **assignment operator** is used to assign or update the value of a variable.

Example:

```java
int num = 10;
```

Here, `=` is the assignment operator.

---

### Types of Assignment Operators

| Operator | Meaning             |
| -------- | ------------------- |
| `=`      | Assign              |
| `+=`     | Add and assign      |
| `-=`     | Subtract and assign |
| `*=`     | Multiply and assign |
| `/=`     | Divide and assign   |
| `%=`     | Modulus and assign  |

---

### Increment Operator (`++`)

The increment operator increases the value of a variable by **1**.

Example:

```java
int num = 10;
num++;
```

Equivalent to:

```java
num = num + 1;
```

---

### Decrement Operator (`--`)

The decrement operator decreases the value of a variable by **1**.

Example:

```java
int num = 10;
num--;
```

Equivalent to:

```java
num = num - 1;
```

---

## 2. Why?

Assignment operators provide a shorter and more readable way to update variables.

Instead of writing:

```java
num = num + 5;
```

we can simply write:

```java
num += 5;
```

Similarly, `++` and `--` provide a shorter way to increase or decrease a value by 1.

---

## 3. Code Explained

### Assignment (`=`)

```java
int num = 10;
```

Assigns `10` to `num`.

---

### Add and Assign (`+=`)

```java
num += 5;
```

Equivalent to:

```java
num = num + 5;
```

---

### Subtract and Assign (`-=`)

```java
num -= 5;
```

Equivalent to:

```java
num = num - 5;
```

---

### Multiply and Assign (`*=`)

```java
num *= 2;
```

Equivalent to:

```java
num = num * 2;
```

---

### Divide and Assign (`/=`)

```java
num /= 2;
```

Equivalent to:

```java
num = num / 2;
```

---

### Modulus and Assign (`%=`)

```java
num %= 2;
```

Equivalent to:

```java
num = num % 2;
```


### Pre Increment

```java
int num = 5;

System.out.println(++num);
```

**Output**

```text
6
```

---

### Post Increment

```java
int num = 5;

System.out.println(num++);
System.out.println(num);
```

**Output**

```text
5
6
```

---

### Pre Decrement

```java
int num = 5;

System.out.println(--num);
```

**Output**

```text
4
```

---

### Post Decrement

```java
int num = 5;

System.out.println(num--);
System.out.println(num);
```

**Output**

```text
5
4
```

---

## 4. Key Differences

### Assignment (`=`) vs Add & Assign (`+=`)

| `=`                    | `+=`                                             |
| ---------------------- | ------------------------------------------------ |
| Assigns a new value    | Adds to the existing value and stores the result |
| Replaces the old value | Uses the old value in the calculation            |

Example:

```java
int num = 10;

num = 20;   // num = 20
num += 5;   // num = 25
```

---

### Pre vs Post Increment

| Pre (`++num`)           | Post (`num++`)              |
| ----------------------- | --------------------------- |
| Increment happens first | Current value is used first |
| Returns updated value   | Returns original value      |

Example:

```java
int num = 5;

System.out.println(++num); // 6
System.out.println(num++); // 6
System.out.println(num);   // 7
```

---

## 5. Interview Questions

### Q1. What is an assignment operator?

**Answer:**

An assignment operator is used to assign or update the value of a variable.

---

### Q2. What is the difference between `=` and `+=`?

**Answer:**

`=` assigns a new value, whereas `+=` adds a value to the existing variable and stores the result.

---

### Q3. Are these two statements equivalent?

```java
num += 5;
```

```java
num = num + 5;
```

**Answer:**

Yes.

---

### Q4. What is the difference between `++num` and `num++`?

**Answer:**

`++num` increments the variable before it is used, whereas `num++` uses the current value first and increments it afterward.

---

### Q5. Predict the output.

```java
int a = 5;

System.out.println(a++);
System.out.println(a);
```

**Answer**

```text
5
6
```

---

### Q6. Predict the output.

```java
int a = 5;

System.out.println(++a);
```

**Answer**

```text
6
```

---

## 6. Practice

### Practice 1

Rewrite using `+=`

```java
num = num + 10;
```

---

### Practice 2

Rewrite using `-=`

```java
num = num - 5;
```

---

### Practice 3

Predict the output.

```java
int num = 20;

num += 5;
num *= 2;

System.out.println(num);
```

---

### Practice 4

Predict the output.

```java
int a = 10;

System.out.println(a++);
System.out.println(++a);
```

---

## 7. Key Takeaways

* `=` assigns a value.
* `+=`, `-=`, `*=`, `/=`, `%=` update the existing value.
* `++` increases a value by 1.
* `--` decreases a value by 1.
* `++num` increments first.
* `num++` uses the value first, then increments.

---

## 8. Common Mistakes

❌

```java
num =+ 5;
```

✔️

```java
num += 5;
```

---

❌ Assuming `num++` prints the incremented value.

```java
int num = 5;
System.out.println(num++);
```

**Output**

```text
5
```

The increment happens **after** the current value is used.

---

❌ Assuming `++num` and `num++` always behave the same.

They produce the same result **only when their returned value is not used**.

---

## 📝 30-Second Revision

* `=` → Assign
* `+=` → Add & Assign
* `-=` → Subtract & Assign
* `*=` → Multiply & Assign
* `/=` → Divide & Assign
* `%=` → Modulus & Assign
* `++` → Increase by 1
* `--` → Decrease by 1
* `++num` → Increment first
* `num++` → Use first, increment later
