# 📘 Video 8 - Type Conversion & Type Casting

## 1. Concepts

### What is Type Conversion?

**Type Conversion** is the automatic conversion of a smaller data type into a larger data type.

It is also called **Implicit Conversion** or **Widening**.

Example:

```java
byte b = 10;
int a = b;
```

Java performs the conversion automatically because `byte` can safely fit into an `int`.

---

### What is Type Casting?

**Type Casting** is the manual conversion of a larger data type into a smaller data type.

It is also called **Explicit Conversion** or **Narrowing**.

Example:

```java
int a = 257;
byte b = (byte) a;
```

The `(byte)` tells Java to convert the value manually.

---

## 2. Why?

Java automatically performs only **safe conversions**.

If there is a possibility of data loss, Java requires the programmer to explicitly perform the conversion using type casting.

---

## 3. Code Explained

### Type Conversion (Automatic)

```java
byte b = 127;
int a = b;
```

`byte → int`

✅ Automatic conversion.

---

### Type Casting (Manual)

```java
int a = 257;
byte b = (byte) a;
```

Output:

```text
1
```

Reason:

```text
257 % 256 = 1
```

---

### Integer to Float

```java
int a = 10;
float f = a;
```

Output:

```text
10.0
```

---

### Float to Integer

```java
float f = 5.6f;
int a = (int) f;
```

Output:

```text
5
```

The decimal part is discarded.

---

## 4. Interview Questions

### Q1. What is type conversion?

**Answer:**

Automatic conversion of a smaller data type into a larger data type.

---

### Q2. What is type casting?

**Answer:**

Manual conversion of a larger data type into a smaller data type.

---

### Q3. Why is casting required?

**Answer:**

Because converting from a larger data type to a smaller one may result in data loss.

---

### Q4. What is the output?

```java
int a = 257;
byte b = (byte) a;
System.out.println(b);
```

**Answer:**

```text
1
```

---

## 5. Practice

### Practice 1

Convert:

```java
byte b = 20;
```

to an `int`.

---

### Practice 2

Convert:

```java
float f = 9.8f;
```

to an `int`.

---

### Practice 3

Predict the output:

```java
int a = 300;
byte b = (byte) a;
System.out.println(b);
```

---

## 6. Key Takeaways

* Type Conversion = Automatic.
* Type Casting = Manual.
* Small → Large = Automatic.
* Large → Small = Casting.
* Casting may result in data loss.

---

## 7. Common Mistakes

❌

```java
float f = 5.6;
```

✔️

```java
float f = 5.6f;
```

---

❌

```java
int a = 5.6f;
```

✔️

```java
int a = (int) 5.6f;
```

---
## 8. Key Differences

| Type Conversion | Type Casting |
|-----------------|--------------|
| Automatic | Manual |
| Also called Implicit Conversion | Also called Explicit Conversion |
| Small → Large data type | Large → Small data type |
| No cast operator required | Requires `(datatype)` |
| No data loss | Data loss may occur |

### Example

```java
byte b = 10;
int a = b;        // Type Conversion
```

```java
int a = 257;
byte b = (byte) a; // Type Casting
```

## 📝 30-Second Revision

* Type Conversion = Automatic.
* Type Casting = Manual.
* Use `(datatype)` for casting.
* Casting can lose data.
* `257` cast to `byte` becomes `1`.
