========================================
COMPILE TIME VS RUN TIME
========================================

------------------------------------------------------------

BASIC IDEA
----------

Program execution happens in two major phases:

    1) Compile Time
    2) Run Time


------------------------------------------------------------

COMPILE TIME
------------------------------------------------------------

Definition:

    Compile time is the phase when
    source code is converted into
    machine code by the compiler.


It happens:

    Before program execution


------------------------------------------------------------

COMPILE TIME ERRORS
------------------------------------------------------------

Errors detected during compilation.

Examples:

    • Syntax error
    • Missing semicolon
    • Undeclared variable
    • Type mismatch


Example:

    int x = "Hello"

This causes type mismatch error
at compile time.


------------------------------------------------------------

COMPILE TIME FEATURES
------------------------------------------------------------

• Static binding  
• Method overloading  
• Syntax checking  
• Type checking  


------------------------------------------------------------

RUN TIME
------------------------------------------------------------

Definition:

    Run time is the phase when
    the compiled program is
    actually executed.


It happens:

    After successful compilation


------------------------------------------------------------

RUN TIME ERRORS
------------------------------------------------------------

Errors that occur during execution.

Examples:

    • Division by zero
    • Array index out of bound
    • Null pointer exception
    • File not found


Example:

    int a = 10 / 0

This causes arithmetic exception
at run time.


------------------------------------------------------------

RUN TIME FEATURES
------------------------------------------------------------

• Dynamic binding  
• Method overriding  
• Exception handling  
• User input handling  


------------------------------------------------------------

KEY DIFFERENCES
------------------------------------------------------------

Compile Time

    • Happens before execution
    • Checked by compiler
    • Syntax & type errors detected
    • Faster error detection


Run Time

    • Happens during execution
    • Checked by JVM / OS
    • Logical & execution errors detected
    • May crash program


------------------------------------------------------------

IMPORTANT SHORT NOTES
------------------------------------------------------------

Compile Time

    = Code checking phase


Run Time

    = Code execution phase


Compile Time errors

    → Must be fixed before running


Run Time errors

    → Occur while program is running


