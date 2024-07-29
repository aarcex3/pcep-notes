# Key Take Aways

1. A **function** is a block of code that performs a specific task when the function is called (invoked). You can use functions to make your code reusable, better organized, and more readable. Functions can have parameters and return values.
    1. Types:
        - **built-in**: The come with python
        - **pre-installed modules**
        - **user-defined functions**
        - **lambda**

    2. Defintion:

        ```python
        def your_function(optional parameters):
        # the body of the function
        ```

2. You can pass arguments to a function using the following techniques:
    - **positional** argument passing in which the order of arguments passed matters,
    - **keyword** (named) argument passing in which the order of arguments passed doesn't matter,
    - a mix of positional and keyword argument passing.

    **It's important to remember that positional arguments mustn't follow keyword arguments**

3. You can use the `return` keyword to tell a function to return some value. The return statement exits the function.

4. A variable that exists outside a function has a scope inside the function body (Example 1) unless the function defines a variable of the same name (Example 2, and Example 3), e.g:

    Example 1:

    ```python
    var = 2

    def mult_by_var(x):
        return x * var


    print(mult_by_var(7))    # outputs: 14
    ```

    Example 2:

    ```python
    def mult(x):
        var = 5
        return x * var


    print(mult(7))    # outputs: 35
    ```

    Example 3:

    ```python
    def mult(x):
        var = 7
        return x * var


    var = 3
    print(mult(7))    # outputs: 49

    ```

5. A variable that exists inside a function has a scope inside the function body (Example 4), e.g.:

    Example 4:

    ```python
    def adding(x):
        var = 7
        return x + var


    print(adding(4))    # outputs: 11
    print(var)    # NameError

    ```

6. You can use the `global` keyword followed by a variable name to make the variable's scope global, e.g.

    ```python
    var = 2
    print(var)    # outputs: 2


    def return_var():
        global var
        var = 5
        return var


    print(return_var())    # outputs: 5
    print(var)    # outputs: 5

    ```

7. Tuples are ordered and unchangeable (immutable) collections of data. They can be thought of as immutable lists. They are written in round brackets.

8. Dictionaries are ordered, changeable (mutable), and indexed collections of data. Each dictionary is a set of *key: value* pairs. You can create it by using the following syntax:

    ```python
    my_dictionary = {
        key1: value1,
        key2: value2,
        key3: value3,
        }
    ```

9. Exceptions:

    1. **TypeError**: Raised when an operation or function is applied to an object of inappropriate type.

    ```python
    # Example of TypeError
    try:
        result = len(5)
    except TypeError as e:
        print(f"TypeError: {e}")

    ```

    2. **ValueError**: Raised when a function receives an argument of the correct type but an inappropriate value.

    ```python
    # Example of ValueError
    try:
        result = int('abc')
    except ValueError as e:
        print(f"ValueError: {e}")
    ```
  
10. You can "catch" and handle exceptions in Python by using the `try-except` block

    ```python
    while True:
    try:
        number = int(input("Enter an integer number: "))
        print(number/2)
        break
    except:
        print("Warning: the value entered is not a valid number. Try again...")
    ```

11. You can handle multiple exceptions in your code block.

    ```python
    while True:
    try:
        number = int(input("Enter an int number: "))
        print(5/number)
        break
    except ValueError:
        print("Wrong value.")
    except ZeroDivisionError:
        print("Sorry. I cannot divide by zero.")
    except:
        print("I don't know what to do...")
    ```

    You can also specify and handle multiple built-in exceptions within a single *except* clause:

    ```python
    while True:
    try:
        number = int(input("Enter an int number: "))
        print(5/number)
        break
    except (ValueError, ZeroDivisionError):
        print("Wrong value or No division by zero rule broken.")
    except:
        print("Sorry, something went wrong...")

    ```
