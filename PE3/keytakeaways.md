# Key Take Aways

1. The **comparison** (otherwise known as relational) operators are used to compare values. The table below illustrates how the comparison operators work, assuming that x = 0, y = 1, and z = 0:

    | Operator | Description | Example |
    |----------|-------------|---------|
    | ==       | Returns `True` if operands' values are equal, and `False` otherwise | `x == x -> True` <br> `x == y -> False` |
    | !=       | Returns `True` if operands' values are not equal, and `False` otherwise | `x != y -> True` <br> `x != z -> False` |
    | >        | `True` if the left operand's value is greater than the right operand's value, and `False` otherwise | `x > y -> False` <br> `y > z -> True` |
    | <        | `True` if the left operand's value is less than the right operand's value, and `False` otherwise | `x < y -> True` <br> `y < z -> False` |
    | ≥        | `True` if the left operand's value is greater than or equal to the right operand's value, and `False` otherwise | `x ≥ y -> False` <br> `x ≥ z -> True` <br> `y ≥ z -> True` |
    | ≤        | `True` if the left operand's value is less than or equal to the right operand's value, and `False` otherwise | `x ≤ y -> True` <br> `x ≤ z -> True` <br> `y ≤ z -> False` |

2. When you want to execute some code only if a certain condition is met, you can use a **conditional statement**. `if-else`, `if-elif-else`
3. There are two types of loops, `while` and `for` loop:
    1. **while**: It executes *while* a condition is met
    2. **for**: It executes a set of statements many times; it's used to iterate over a sequence (e.g., a list, a dictionary, a tuple, or a set) or other objects that are iterable (e.g., strings). You can use the for loop to iterate over a sequence of numbers using the built-in range function.

    Both types can have an `else` statement at the end. It executes when the loop finishes.

4. You can use the `break` and `continue` statements to change the flow of a loop:
    1. **break**: To exit a loop
    2. **continue**: To skip to the next iteration

5. The `range()` function generates a sequence of numbers. It accepts integers and returns range objects. The syntax of `range()` looks as follows: `range(start, stop, step)`, where:
    - start is an optional parameter specifying the starting number of the sequence (0 by default)
    - stop is an optional parameter specifying the end of the sequence generated (it is not included)
    - step is an optional parameter specifying the difference between the numbers in the sequence (1 by default.)

6. Python supports logical operators: `and`,`or`,`not`
    | Operator | Description | Example |
    |----------|-------------|---------|
    | `and`      | Returns `True` if both statements are true | `x and y -> True` if both x and y are True |
    | `or`       | Returns `True` if one of the statements is true | `x or y -> True` if either x or y is True |
    | `not`     | Reverses the result, returns `False` if the result is true | `not x -> True` if x is False |

7. Python also supports bitwise operators: `&`,`|`,`^`,`~`,`<<`,`>>`
    | Operator | Description                                                                 | Example                 |
    |----------|-----------------------------------------------------------------------------|-------------------------|
    | &        | AND: Sets each bit to 1 if both bits are 1                                  | `0b0101 & 0b0011 = 0b0001` (1 in decimal) |
    | \|       | OR: Sets each bit to 1 if one of the two bits is 1                         | `0b0101 \| 0b0011 = 0b0111` (7 in decimal) |
    | ^        | XOR: Sets each bit to 1 if only one of the two bits is 1                    | `0b0101 ^ 0b0011 = 0b0110` (6 in decimal) |
    | ~        | NOT: Inverts all the bits                                                     | `~0b0101 = 0b1010` (Assuming 4-bit representation, -6 in decimal) |
    | <<       | Zero fill left shift: Shift left by pushing zeros in from the right           | `0b0101 << 2 = 0b10100` (20 in decimal) |
    | >>       | Signed right shift: Shift right by pushing copies of the leftmost bit in from the left | `0b0101 >> 2 = 0b0001` (1 in decimal) |

8. The **list is a type of data** in Python used to store multiple objects. It is an ordered and mutable collection of comma-separated items between square brackets, e.g., `my_list = [1, None, True, "I am a string", 256, 0]`. Lists can be indexed, updated and nested. List elements and lists can be deleted. Lists can be iterated through. A typical *function invocation* looks as follows: `result = function(arg)`, while a typical *method invocation* looks like this: `result = data.method(arg)`

9. You can use `.sort()` to sort a list or `.reverse()` to reverse a list.
10. Having a list name list1 and then assigning it to another variable **does not make a copy** of the list, it just takes the address of the list in memory. E.g.

    ```python
    vehicles_one = ['car', 'bicycle', 'motor']
    print(vehicles_one) # outputs: ['car', 'bicycle', 'motor']

    vehicles_two = vehicles_one
    del vehicles_one[0] # deletes 'car'
    print(vehicles_two) # outputs: ['bicycle', 'motor']

    ```

11. To copy a list or part of it you use **slicing**
    ```python
    vehicles_one = ['car', 'bicycle', 'motor']
    print(vehicles_one) # outputs: ['car', 'bicycle', 'motor']

    vehicles_two = vehicles_one[:]
    del vehicles_one[0] # deletes 'car'
    print(vehicles_one) # outputs: ['bicycle', 'motor']
    print(vehicles_two) # outputs: ['car', 'bicycle', 'motor']
    ```
12. You can test if some items exist in a list or not using the keywords `in` and `not in`, e.g.:

    ```python
    my_list = ["A", "B", 1, 2]

    print("A" in my_list)  # outputs: True
    print("C" not in my_list)  # outputs: True
    print(2 not in my_list)  # outputs: False
    ```

13. List comprehension allows you to create new lists from existing ones in a concise and elegant way. The syntax of a list comprehension looks as follows:
        ```python
        [expression for element in list if conditional]
        ```
14. You can use **nested lists** in Python to create matrices (i.e., two-dimensional lists, n-dimensional lists)
