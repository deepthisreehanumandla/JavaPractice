## 77-81) Exception Handling, Multiple Catch, Exception Hierarchy, `throw` & Custom Exception 

### Purpose
- Handle runtime errors without terminating the program.
- Create meaningful and controlled error handling.

### Exception Handling (`try-catch`)
- `try` contains code that may cause an exception.
- `catch` handles the exception.
- Program continues execution after handling the exception.

```java
try {
    int result = 10 / 0;
} catch (Exception e) {
    System.out.println("Something went wrong");
}
```

### Multiple Catch
- A single `try` block can have multiple `catch` blocks.
- Specific exceptions should be placed before general exceptions.

### Exception Hierarchy
- `Throwable` is the parent class.
- `Error` → System-level errors.
- `Exception` → Application-level exceptions that can be handled.

### `throw` Keyword
- Used to throw an exception manually.
- Helps validate conditions.

```java
if(age < 18)
    throw new ArithmeticException("Not Eligible");
```

### Custom Exception
- Create your own exception by extending `Exception`.

```java
class MyException extends Exception {
    public MyException(String msg) {
        super(msg);
    }
}
```

### Key Points
- Exceptions occur during runtime.
- `try-catch` prevents abnormal termination.
- Multiple `catch` blocks handle different exceptions.
- `throw` manually generates an exception.
- Custom exceptions make error handling more meaningful.
