# Key Take Aways

1. The **print()** function is a built in function.
2. Built-in functions, contrary to user-defined functions, are always available and don't have to be imported. Python 3.8 comes with 69 built-in functions.
3. To call a function (this process is known as **function invocation** or **function call**), you need to use the function name followed by parentheses. You can pass arguments into a function by placing them inside the parentheses. You must separate arguments with a comma, e.g., **print("Hello,", "world!")**
4. Computer programs are collections of instructions. An instruction is a command to perform a specific task when executed, e.g., to print a certain message to the screen.
5. **Positional arguments** are the ones whose meaning is dictated by their position, e.g., the second argument is outputted after the first, the third is outputted after the second, etc.
6. **Keyword arguments** are the ones whose meaning is not dictated by their location, but by a special word (keyword) used to identify them. E.g., **func(var1=a,var2=b)**
7. Literals are notations for representing some fixed values in code. Python has various types of literals - for example, a literal can be a number (numeric literals, e.g., 123), or a string (string literals, e.g., "I am a literal.").
8. **Integers** (or simply ints) are one of the numerical types supported by Python. They are numbers written without a fractional component, e.g., 256, or -1 (negative integers).
9. **Floating-point** numbers (or simply floats) are another one of the numerical types supported by Python. They are numbers that contain (or are able to contain) a fractional component, e.g., 1.27.
10. **Boolean** values are the two constant objects True and False used to represent truth values (in numeric contexts 1 is True, while 0 is False).
11. An **expression** is a combination of values (or variables, operators, calls to functions)
12. **Operators** are special symbols or keywords which are able to operate on the values and perform (mathematical) operations, e.g., the \* operator multiplies two values: x \* y.
    1. Types:
        1. **unary**: operator that requires only one operand, e.g., -1, or +3.
        2. **binary**: operator that requires two operand, 4 + 5, or 12 % 5.
    2. Hierarchy:
        Operators have a hierachy, which one comes first and which one comes last?

        |Priotiry|Operator|Type|
        | ------------- | ------------- |---|
        |1| **||
        |2|+, -|unary|
        |3|*, /, //, %||
        |4|+, -|binary|

13. Subexpressions in parentheses are always calculated first, e.g., 15 - 1 \* ( 5\* (1 + 2)) = 0.

14. The exponentiation operator uses right-sided binding, e.g., 2 \*\* 2 \*\* 3 = 256.

15. A variable is a named location reserved to store values in the memory. A variable is created or initialized automatically when you assign a value to it for the first time.

16. Each variable must have a unique name - an **identifier**. A legal identifier name must be a non-empty sequence of characters, must begin with the underscore(_), or a letter, and it cannot be a Python keyword. The first character may be followed by underscores, letters, and digits. Identifiers in Python are case-sensitive, e.g., var != Var

17. Python is a dynamically-typed language, which means you don't need to declare variables in it. To assign values to variables, you can use a simple assignment operator in the form of the equal (=) sign, i.e., var = 1.

18. You can also use compound assignment operators (shortcut operators) to modify values assigned to variables, e.g., var += 1, or var /= 5 * 2.

19. Comments can be used to leave additional information in code. They are omitted at runtime. The information left in source code is addressed to human readers. In Python, a comment is a piece of text that begins with #. The comment extends to the end of line.

20. If you want to place a comment that spans several lines, you need to place # in front of them all.

21. Comments can be important when *you* are reading your own code after some time, and when *others* are reading your code.
