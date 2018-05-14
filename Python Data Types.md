# Python Data Types:

### How do we print in python?
- Use `print()`.

```python
print(3 + 5)
```

## Variables and Data types:

### Variable:
- Define using `=` sign. e.g. `x = 15`
- `=` sign is an anssignment operator. (Doesn't check equality.)
- **Multiple assignments:**
    - You can perform multiple assignments to multiple variables in single line.
    ```python
    x, y, z = 2, 3, 4
    ```
- **Naming the variables:**
    - Don't start with number. 
    - Don't use spaces in variable name.
    - Don't use camel case.
    - Don't use python keywords (e.g. break, def, if, return etc.).
    - Right way of varible name is `var_name`.
- **Other asignment operators:**
    - += (`x += 5`)
    - -= (`x -= 5`)   
    - *= (`x *= 5`)

### Integer and Float:
- **Integer** - Whole number
- **Float** - Real number
- You can check the data type of the variable using `type()`.
```python
x = 4.5
print(type(x))
```
- While converting **Float to Int** the digits after decimals get cut off. No runding occurs.
```python
x = 4.5     ## Float
y = int(x)  ## Int
print(y)    ## y = 4
```
- While converting **Int to Float** adds .0 at the end of the number
```python
x = 4           ## Int
y = float(x)    ## Int
print(y)        ## y = 4.0
```
### Booleans:
- Either `0`  or `1`.

### Strings:
- Imutable
- Ordered series of character.
- Defined by " or '.
```python
print("hello")
print('hello')
```
- Use `str()` to convert floats and int to string.

### What are arithmatic operators in python?
- List of arithmatic operations:
    - +  ---> Addition `print(7 + 2)` = 9
    - -  ---> Subrtaction `print(7 - 2)` = 5
    - *  ---> Multiplication `print(7 * 2)` = 14
    - /  ---> Division `print(7 / 2)` = 3.5
    - ** ---> Power `print(7 ** 2)` = 49
    - %  ---> Modulo `print(7 % 2)` = 1
    - // ---> Intger divider `print(7 // 2)` = 3 or `print(17 // 2)` = -4

### Comparison Operators:
- Compares two values and produces boolean results.
    - > 
    - <
    - <=
    - >=
    - ==
    - !=

### Logical Operators:
- Logical operators are use for bitwise manupulation.
    - and   -> Evaluates if both the values are true.
    - or    -> Evaluates if any one from the values are true. 
    - not   -> Inverses the boolean type.

### String operators:
- + -> To append the string.
```python
x = "I love " + "python."
print(x)    # x = "I love python."
```
- * -> To repeat strings.
```python
x = "I love python." * 2
print(x)    # x = "I love python.I love python."
```
- `len()` tells the length of the string.
```python
x = len("Python")
print(x)    # x = 6
```

## Type conversion:
- Convert string or float to int using `int()`.
- Convert string or int to float using `float()`.
- Convert float or int to string using `str()`.

## Exceptions in python:
- In general, there are two types of errors to look out for
    - Exceptions
    - Syntax
- An Exception is a problem that occurs when the code is running, but a 'Syntax Error' is a problem detected when Python checks the code before it runs it.

## Lists in python:
- List is collection of data. 
- It's a container.
- It's mutable.
- It's ordered. (Indexed)

### How do we write list?
```python
months = [1, 3.4, 'a string', True]
```

### How to read the values from list?
- Use position of the item in the list.
```python
months = [1, 3.4, 'a string', True]
print(mpnths[0])    # 1
print(months[-1])   # True
```

### Slicing:
- Slice the list by giving start and end position.
- Here list[3:6] will create new list starting from 3rd element of the list to 5th.
- It is [3,6).
```python
months = [1, 3.4, 'a string', True]
print(months[1:3])  # 3.4, 'a string'
```
- Other short hand notation:
```python
months = [1, 3.4, 'a string', True]
print(months[:2])  # 1, 3.4
print(months[2:])  # 'a string', True

### Membership operators:
- **in** checks weather the member on the left side is included in the list/string on the right side.
```python
months = [1, 3.4, 'a string', True]
print(1 in months)  # True
```
- **not in** checks weather the member on the left side is not included in the list/string on the right side.
```python
months = [1, 3.4, 'a string', True]
print(1 not in months)  # False
```