#  runtime_error.md

```md
# Runtime Error

## Definition
A runtime error occurs during the execution of a program after it has successfully compiled.

The program starts running but crashes due to an unexpected problem.

---

# Causes of Runtime Errors

Division by zero  
Invalid memory access  
Null pointer access  
Array index out of bounds  
Invalid user input

---

# Example (Java)

```java
public class Test {
    public static void main(String[] args) {
        int a = 10;
        int b = 0;

        int result = a / b;  // runtime error
        System.out.println(result);
    }
}