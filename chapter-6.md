# Flow  of Control
- Flow of Control is the order in which the statements of a program are executed. It determines how the program moves from one statement to another. In Python, the flow of control can be changed using selection and iteration statements.

## 1. Selection (Decision Making)
- Selection (Decision Making) is a flow of control mechanism in which the program chooses and executes one block of statements from two or more alternatives based on a given condition. The condition is evaluated as either True or False. If the condition is True, the corresponding block of code is executed; otherwise, another block of code is executed or skipped.

### Selection Statements in Python
- Python provides three main decision-making statements:

#### 1. if Statement
- The if statement executes a block of code only when the condition is True.
- Syntax:
    ```python
    if condition:
        statement(s)
    ```
- Example:
    ```python
    marks = 85

    if marks >= 33:
        print("Pass")
    ```

#### 2. if-else Statement
- The if-else statement is used when there are two possible choices.

- Syntax:
    ```python
    if condition:
        statements
    else:
        statements
    ```
- Example:
    ```python
    age = 16

    if age >= 18:
        print("Eligible to vote")
    else:
        print("Not Eligible")
    ```

#### 3. if-elif-else Statement
- This statement is used when there are multiple conditions.
- Python checks conditions one by one.
- As soon as one condition becomes True, Python executes that block and ignores the remaining conditions.
- Syntax:
    ```python
    if condition1:
        statements
    elif condition2:
        statements
    elif condition3:
        statements
    else:
        statements
    ```
- Example:
    ```python
    marks = 72

    if marks >= 90:
        print("Grade A+")
    elif marks >= 75:
        print("Grade A")
    elif marks >= 60:
        print("Grade B")
    else:
        print("Grade C")
    ```

<br><br>

## 2. Repetition
- Repetition, also called Iteration or Looping, is a flow of control in which a block of statements is executed repeatedly until a specified condition is met or for a fixed number of times. Python performs repetition using for and while loops.

### There are two main types of loops in Python:
#### 1. for Loop
- A for loop is one of the most important looping statements in Python. It executes a block of code repeatedly by taking values one by one from a sequence. It is simple, efficient, and ideal for situations where the number of repetitions is known or when working with collections such as strings, lists, tuples, and ranges. Because it reduces repetitive code and improves readability, the for loop is widely used in Python programming.
- Syntax:
    ```python
    for variable in sequence:
        statement(s)
    ```
- Example:
    ```python
    for i in range(5):
        print(i)
    ```

#### 2. while Loop
- A while loop is a powerful looping statement in Python that repeats a block of code as long as a specified condition is True. It is especially useful when the number of repetitions is not known beforehand. Proper initialization, condition checking, and variable updation are essential to avoid infinite loops. Because of its flexibility, the while loop is widely used in user-interactive programs, games, login systems, and many real-world applications.
- Syntax:
    ```python
    while condition:
        statement(s)
    ```
- Example:
    ```python
    i = 1

    while i <= 5:
        print(i)
        i = i + 1
    ```
    

#### Difference Between for Loop and while Loop

| **for Loop**                                 | **while Loop**                                     |
| -------------------------------------------- | -------------------------------------------------- |
| Used when the number of iterations is known. | Used when the number of iterations is not known.   |
| Iterates over a sequence.                    | Runs while a condition is true.                    |
| Easier to write for fixed repetitions.       | Better for condition-based repetition.             |
| Automatically moves to the next value.       | The programmer must update the condition manually. |

<br><br>

## The range() Function
- The range() function is one of the most useful built-in functions in Python. It generates a sequence of integers and is mainly used with for loops to repeat a block of code a fixed number of times. It supports three forms—range(stop), range(start, stop), and range(start, stop, step)—making it flexible for generating ascending or descending sequences. Understanding the start, stop, and step parameters is essential for writing efficient Python programs.
- Syntax:
    ```python
    range(start, stop, step)
    ```
- Example:
    ```python
    l = list(range(10))
    print(l)
    ```

<br><br>

## Indentation 
- Indentation is the space (or tab) provided at the beginning of a line of code to define a block of statements in Python. >It tells Python which statements belong to the same block.
- Unlike many other programming languages that use { } (curly braces), Python uses indentation to define code blocks.
- Indentation is one of the most important features of Python. It is used after statements like if, else, for, while, def, etc., to indicate which statements are part of that block.
- All statements inside the same block must have the same indentation. If the indentation is incorrect or inconsistent, Python generates an IndentationError.
- The standard practice is to use 4 spaces for each level of indentation.
- Syntax:
    ```python
    if condition:
        statement1
        statement2
    ```
- Example:
    ```python
    # Program to find Greater of the numbers
    num1 = 6
    num2 = 4
    if num1 > num2:     # Block 1
        print("First Number is Greater.")
        print("Over")
    else:               # Block 2
        print("Second Number is Greater.")
        print("Over and Out")
    print("Out of all Blocks")
    ```

<br><br>

## The Break and Continue Statement 

### 1. The break Statement
- The break statement is a loop control statement that immediately terminates a loop when a specified condition is met. After the break statement is executed, control moves to the first statement after the loop.
- Syntax:
    ```python
    break
    ```
- Example:
    ```python
    for i in range(1, 6):
        if i == 4:
            break
        print(i)
    ```

### 2. The continue Statement
- The continue statement is a loop control statement in Python that skips the remaining statements of the current iteration and immediately transfers control to the next iteration of the loop. It can be used with both for and while loops.
- Syntax:
    ```python
    continue
    ```
- Example:
    ```python
    for i in range(1, 6):
        if i == 3:
            continue
        print(i)
    ```

<br><br>

## Nested Loops
- A nested loop is a loop inside another loop. In a nested loop, the inner loop executes completely for each iteration of the outer loop. Nested loops can be created using for loops, while loops, or a combination of both.
- Syntax(for loop):
    ```python
    for outer_variable in sequence:
        for inner_variable in sequence:
            statement(s)
    ```
- Syntax(while loop):
    ```python
    while condition1:
        while condition2:
            statement(s)
    ```
- Example(for loop):
    ```python
    for i in range(3):
        for j in range(5):
            print("*", end=" ")
        print()
    ```
- Example:
    ```python
    i = 1

    while i <= 3:
        j = 1
        while j <= 4:
            print(j, end=" ")
            j += 1
        print()
        i += 1
    ```