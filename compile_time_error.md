# Compile-Time Error

## Definition
A compile-time error is an error that occurs during the compilation of a program.

The compiler detects these errors before the program runs.

If compile-time errors exist, the program **cannot execute**.

---

# Causes of Compile-Time Errors

Syntax errors  
Missing symbols  
Incorrect variable declarations  
Wrong method signatures  
Type mismatch

---

# Example (Java)

```java
public class Test {
    public static void main(String[] args) {
        int x = "Hello";   // compile-time error
        System.out.println(x);
    }
}