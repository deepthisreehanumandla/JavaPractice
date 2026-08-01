## 68) What is Enum in Java

### What is an Enum?
- `enum` is a special data type used to represent a fixed set of constants.
- It improves code readability and avoids using random integer or string values.

### Syntax
```java
enum Status {
    Running, Failed, Pending, Success
}
```

### Creating an Enum Object
```java
Status s = Status.Running;
```

### Features
- Enum values are constants.
- Enum names are usually written in PascalCase (as shown by Telusko).
- Useful when the possible values are limited and predefined.

### Common Uses
- Days of the week
- Months
- Order status
- Traffic lights
- User roles

### Key Points
- Enum represents a fixed collection of constants.
- Values cannot be changed at runtime.
- Makes code safer and easier to understand.

---

## 69) Enum if and Switch in Java

### Enum with if
```java
if (s == Status.Running) {
    System.out.println("Running...");
}
```

### Enum with switch
```java
switch (s) {
    case Running:
        System.out.println("Running");
        break;

    case Failed:
        System.out.println("Failed");
        break;

    default:
        System.out.println("Done");
}
```

### Key Points
- Compare enums using `==`.
- Enums work directly with `switch`.
- No need to compare strings.

---

## 70) Enum Class in Java

### Enum is a Class
- Every enum is internally a class.
- Enum can have:
  - Variables
  - Constructors
  - Methods

### Example
```java
enum Laptop {
    Macbook(2000), XPS(1800), ThinkPad(1500);

    private int price;

    Laptop(int price) {
        this.price = price;
    }

    public int getPrice() {
        return price;
    }
}
```

### Important Points
- Enum constructors are called automatically.
- Enum constructors are private by default.
- Each enum constant is an object of the enum class.

### Key Points
- Enum is more than just constants.
- It can store data and methods.
- Useful for organizing related constant values with additional information.
