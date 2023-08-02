# Topic 9: Debugging and Troubleshooting

In this topic, we'll explore debugging and troubleshooting techniques in Python. Debugging is the process of identifying and fixing errors (bugs) in your code to ensure it runs smoothly and as expected.

Items covered:

  ## Common Types of Errors:
            Syntax Errors: Errors that occur due to incorrect syntax in the code, preventing the program from running.
            Runtime Errors (Exceptions): Errors that occur during program execution due to unexpected conditions, such as division by zero or accessing an invalid index in a list.
            Logic Errors: Errors that do not cause the program to crash but result in incorrect output or behavior due to flawed logic.

  ## Reading Error Messages:
        Python provides error messages that help identify the cause of an error.
        Understanding error messages is crucial for debugging.
        The error message includes the type of error and the line number where the error occurred.

  ## Using print() Statements:
        Placing print statements at various points in your code can help you understand the flow and values of variables during execution.
        This technique allows you to trace the program's behavior and identify potential issues.

  ## Debugging Tools:
        Python comes with built-in debugging tools, such as pdb (Python Debugger) and traceback.
        These tools enable you to step through your code and inspect variables, helping you find and fix errors.

  ## Commenting Out Code:
        Temporarily commenting out sections of code can help identify if a specific piece of code is causing an error.
        This technique helps narrow down the problematic area.

  ## Isolating the Problem:
        If you encounter an error in a large program, try isolating the problem by creating a minimal example (a small piece of code that reproduces the error).
        This approach simplifies debugging and prevents distractions caused by unrelated code.

## Example:

  python

## Example: Debugging and Troubleshooting

    def calculate_average(numbers):
        total = sum(numbers)
        average = total / len(numbers)
        return average
    
    try:
        scores = [90, 85, 95, 80]
        avg = calculate_average(scores)
        print("Average Score:", avg)
        print("Max Score:", max(scores))
        print("Min Score:", min(scores))
        print("Total Scores:", sum(scores))
        print("Last Score:", scores[len(scores)])  # Error: Index out of range
    except Exception as e:
        print("An error occurred:", e)
    
## Output:

    go
    
    An error occurred: list index out of range

## Summary:
    In this example, we have a function calculate_average() that calculates the average of a list of numbers.
    However, there is a bug in the code; we are trying to access an element at an invalid index in the list scores. 
    The program raises an IndexError, and the error message points to the line with the issue.
    By reading the error message, we can quickly identify the problem and fix it by using scores[len(scores) - 1] to access the last element of the list.
