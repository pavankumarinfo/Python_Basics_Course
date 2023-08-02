# Topic 3: Control Flow and Conditional Statements

In this topic, we'll explore control flow and conditional statements in Python. Control flow allows us to make decisions and control the flow of program execution based on certain conditions.

Items covered:

   ## If Statement:
        The "if" statement is used to execute a block of code only if a given condition is True.
        Syntax:

        python
    if condition:
        # Code block to execute if the condition is True

## Else Statement:

    The "else" statement is used along with "if" to execute an alternative block of code when the condition is False.
    Syntax:

    python

    if condition:
        # Code block to execute if the condition is True
    else:
        # Code block to execute if the condition is False

## Elif Statement:

    The "elif" (short for "else if") statement is used to check additional conditions after the "if" statement.
    It allows for multiple conditions to be evaluated sequentially.
    Syntax:

    python

    if condition1:
        # Code block to execute if condition1 is True
    elif condition2:
        # Code block to execute if condition2 is True
    else:
        # Code block to execute if all conditions are False

## Nested If-Else Statements:

    You can nest "if" statements inside other "if" or "else" blocks to create more complex decision-making structures.
    Be careful to maintain proper indentation for readability.
    Syntax:

    python

        if condition1:
            if condition2:
                # Code block to execute if both condition1 and condition2 are True
            else:
                # Code block to execute if condition1 is True but condition2 is False
        else:
            # Code block to execute if condition1 is False

Example:

python

## Example: Control Flow and Conditional Statements

### If statement
    x = 10
    if x > 5:
        print("x is greater than 5")

  ## If-else statement
      y = 3
      if y % 2 == 0:
          print("y is even")
      else:
          print("y is odd")

  ## Elif statement
      grade = 85
      if grade >= 90:
          print("A grade")
      elif grade >= 80:
          print("B grade")
      elif grade >= 70:
          print("C grade")
      else:
          print("Fail")

  ## Nested if-else statement
      num = 7
      if num > 0:
          if num % 2 == 0:
              print("Positive even number")
          else:
              print("Positive odd number")
      else:
          print("Non-positive number")

## Output:

      csharp
      
      x is greater than 5
      y is odd
      B grade
      Positive odd number
