# Getting Started With Python


## Python
- Python is a high-level, interpreted, object-oriented, and general-purpose programming language. It has a simple and easy-to-read syntax, making it easy to learn, write, and debug programs. Python is widely used for web development, data analysis, artificial intelligence, automation, and software development.


## Features of Python
1. Simple and Easy to Learn – Python has a clear and readable syntax, making it easy for beginners to learn and write programs.
2. Interpreted Language – Python executes code line by line, which makes debugging and error detection easier.
3. High-Level Language – It allows programmers to write code without worrying about the complex details of computer hardware.
4. Object-Oriented – Python supports Object-Oriented Programming (OOP), which helps in organizing and reusing code efficiently.
5. Platform Independent – Python programs can run on different operating systems such as Windows, Linux, and macOS without major changes.
6. Case-sensitive - NUMBER and number are not same in Python.

<br>

## Execution Mode
- Python programs can be executed in two modes:
1. Interactive Mode
2. Script Mode
### 1. Interactive Mode
- Interactive Mode is the mode in which Python executes one statement at a time and displays the result immediately. It is mainly used for testing small pieces of code, performing calculations, and learning Python.

### 2. Script Mode
- Script Mode is the mode in which Python programs are written in a file with the .py extension, saved, and then executed. It is suitable for writing, editing, and running large programs.

<br><br>

## Keywords
- Keywords are reserved words in Python that have a predefined meaning and perform specific functions. They cannot be used as variable names, function names, or identifiers because they are part of Python's syntax.

<br>

| | | Python Keywords | | |
|-----------------|-----------------|-----------------|-----------------|-----------------|
| False | class | finally | is | return |
| None | continue | for | lambda | try |
| True | def | from | nonlocal | while |
| and | del | global | not | with |
| as | elif | if | or | yield |
| assert | else | import | pass | async |
| await | break | except | in | raise |


<br><br>

## Identifiers
- Identifiers are the names given to variables, functions, classes, objects, and other user-defined elements in a Python program. They are used to identify these elements uniquely.

### The Rules for naming an identifier in Python are as follows:- 
1. The name should begin with an uppercase or lowercase alphabet or an underscore sign (\_). This may be followed by any combination of characters a-z, A-Z, 0-9 or underscore (\_). Thus, an identifier can't be start with a digit.
2. It can be of any length . (However, it is preferred to keep it short and meaningful).
3. It should not be a keyword or reserved word .
4. We can't use special symbols like !,@,#,$,%,etc , in identifiers.

<br><br>

## Variables
- A variable is a named memory location used to store data or values in a Python program. It acts as a container that holds information, and its value can be changed during the execution of the program. Variable declaration is implicit in Python, means variables are automatically declared and defined when they are assigned a value the first time. Ex :- age = 19

<br><br>

## Comments
- Comments are used to add a remark or a note in the source code. Comments are not executed by interpreter. They are added with the purpose of making the source code easier for humans to understand. A comment starts with # (hash sign). Everything following the # till end of that line is treated as a comment and the interpreter simply ignores it while executing the statement.
- Example:

    ```python
    # totalMarks is sum of all subject marks
    totalMarks = sub1 + sub2 + sub3 
    ```

<br><br><br>

## Everything is an Object
- In Python, everything is an object. This means that every value, such as numbers, strings, lists, functions, and even variables, is treated as an object. Every object has an identity (ID), a data type, and a value, and it can perform operations associated with its type.
- Example:

    ```python
    num = 19
    print( id(num) )
    ```

<br><br><br>

## Data Types
- A data type is the classification or category of data that determines the kind of value a variable can store, the amount of memory required, and the operations that can be performed on it. In Python, every value has a specific data type, which helps the interpreter understand how to store and process that data.


### Common Data Types in Python

| Data Type | Description                             | Example                     |
| --------- | --------------------------------------- | --------------------------- |
| **int**   | Stores whole numbers                    | `10`, `-5`, `100`           |
| **float** | Stores decimal numbers                  | `3.14`, `5.0`               |
| **str**   | Stores text or characters               | `"Hello"`, `'Python'`       |
| **bool**  | Stores logical values                   | `True`, `False`             |
| **list**  | Ordered, mutable collection             | `[10, 20, 30]`              |
| **tuple** | Ordered, immutable collection           | `(10, 20, 30)`              |
| **set**   | Unordered collection of unique elements | `{1, 2, 3}`                 |
| **dict**  | Stores data in key-value pairs          | `{"Name":"Rahul","Age":16}` |

#### 1. Integer (int)
- Integer (int) is a data type used to store whole numbers without any decimal point. It can store positive numbers, negative numbers, and zero. Ex: 64, -6, 0, etc.

#### 2. Float (float)
- Float (float) is a data type used to store decimal (floating-point) numbers. It represents numbers that have a fractional part. Ex: 6.4, -19, 0.4, etc.

#### 3. String (str)
- String (str) is a data type used to store text or a sequence of characters. A string is enclosed within single quotes (' ') or double quotes (" "). Ex: "Hello", 'Python', "Class 11", etc.

#### 4. Boolean (bool)
- Boolean (bool) is a data type that stores only two logical values: True and False. It is mainly used in decision-making and conditional statements. Ex: True, False.

#### 5. List (list)
- A list is an ordered and mutable (changeable) collection of elements. It can store different types of data, and its elements are enclosed in square brackets ([ ]) and separated by commas. Ex: [10, 20, 30] , ["Aman", 16, True] , etc.

#### 6. Tuple (tuple)
- A tuple is an ordered and immutable (unchangeable) collection of elements. Its elements are enclosed in parentheses (( )) and separated by commas. Ex: (10, 20, 30) , ("Red", "Blue") , etc.

#### 7. Set (set)
- A set is an unordered collection of unique elements. It is enclosed in curly braces ({ }) and does not allow duplicate values. Ex: {10, 20, 30} , {"Apple", "Mango", "Orange"} , etc.

#### 8. Dictionary (dict)
- A dictionary is a mutable collection of data stored as key–value pairs. It is enclosed in curly braces ({ }), where each key is associated with a value. Ex: {"Name": "Rahul", "Age": 16} , {"Roll No": 101, "Marks": 95} , etc.

<br><br><br>

## Mutable and Immutable Data Types
### Mutable Data Types
- Mutable data types are those whose values or contents can be changed after they are created, without creating a new object. It only includes List and Dictionary .

### Immutable Data Types
- Immutable data types are those whose values or contents cannot be changed after they are created. If any modification is required, Python creates a new object instead of changing the existing one. It includes Integers, Float, Boolean, Complex, Strings, Tuples, Sets.

<br><br><br>

## Operators
- Operators are special symbols or keywords in Python that are used to perform operations on operands (variables or values) and produce a result. They are used to perform mathematical calculations, comparisons, logical operations, assignment of values, and other tasks in a program.

## Types of Operators in Python
### 1. Arithmetic Operators
- Used to perform mathematical calculations.

| Operator | Meaning             | Example        |
| -------- | ------------------- | -------------- |
| `+`      | Addition            | `10 + 5 = 15`  |
| `-`      | Subtraction         | `10 - 5 = 5`   |
| `*`      | Multiplication      | `10 * 5 = 50`  |
| `/`      | Division            | `10 / 5 = 2.0` |
| `%`      | Modulus (Remainder) | `10 % 3 = 1`   |
| `//`     | Floor Division      | `10 // 3 = 3`  |
| `**`     | Exponent (Power)    | `2 ** 3 = 8`   |

<br>

### 2. Relational (Comparison) Operators
- Used to compare two values. The result is always True or False.

| Operator | Meaning                  | Example           |
| -------- | ------------------------ | ----------------- |
| `==`     | Equal to                 | `5 == 5` → `True` |
| `!=`     | Not equal to             | `5 != 3` → `True` |
| `>`      | Greater than             | `7 > 4` → `True`  |
| `<`      | Less than                | `2 < 8` → `True`  |
| `>=`     | Greater than or equal to | `5 >= 5` → `True` |
| `<=`     | Less than or equal to    | `3 <= 6` → `True` |

<br>

### 3. Logical Operators
- Used to combine or modify conditions.

| Operator | Meaning                                |
| -------- | -------------------------------------- |
| `and`    | True if both conditions are True       |
| `or`     | True if at least one condition is True |
| `not`    | Reverses the result                    |

<br>

### 4. Assignment Operators
- Used to assign values to variables.

| Operator | Meaning                 | Example   |
| -------- | ----------------------- | --------- |
| `=`      | Assign value            | `x = 10`  |
| `+=`     | Add and assign          | `x += 5`  |
| `-=`     | Subtract and assign     | `x -= 5`  |
| `*=`     | Multiply and assign     | `x *= 2`  |
| `/=`     | Divide and assign       | `x /= 2`  |
| `//=`    | Floor divide and assign | `x //= 2` |
| `%=`     | Modulus and assign      | `x %= 2`  |
| `**=`    | Exponentiate and assign | `x **= 2` |


<br>

### 5. Identity Operators
- Used to check whether two variables refer to the same object.

| Operator | Meaning             |
| -------- | ------------------- |
| `is`     | Same object         |
| `is not` | Not the same object |

<br>

### 6. Membership Operators
- Used to check whether a value exists in a sequence.

| Operator | Meaning          |
| -------- | ---------------- |
| `in`     | Value is present |
| `not in` | Value is absent  |

<br><br><br>

## Expressions
- An expression is a combination of operands (variables, constants, or values) and operators that is evaluated by Python to produce a single value or result. Expressions are used to perform calculations, comparisons, and logical operations in a program.
- Example: 
    ```python
    a = 10
    b = 5
    c = a + b
    # 'a + b' is an expression , 'a' and 'b' are operands , '+' is operator and The result of the expression is '15'.
    ```

### Precedence of Operator

