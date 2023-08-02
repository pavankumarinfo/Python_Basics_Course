# Topic 7: Exception Handling

In this topic, we'll explore how to handle exceptions in Python. Exceptions are errors that occur during program execution, and exception handling allows us to handle these errors gracefully, preventing the program from crashing.

Items covered:

   ##  What are Exceptions?
            Exceptions are errors that occur during program execution due to unexpected situations, like dividing by zero or accessing an invalid index in a list.
            When an exception occurs, Python raises an error and stops executing the program unless the exception is handled.

   ## try-except Block:
            The try-except block is used to catch and handle exceptions.
            It allows the program to continue executing even if an exception occurs, preventing the program from crashing.
            Syntax:
    
            python
    
        try:
            # Code that may raise an exception
        except ExceptionType:
            # Code to handle the exception

## Handling Specific Exceptions:

        You can handle specific types of exceptions individually using multiple except blocks.
        This allows for different handling based on the type of exception raised.
        Syntax:
    
        python
    
        try:
            # Code that may raise an exception
        except ValueError:
            # Code to handle ValueError
        except ZeroDivisionError:
            # Code to handle ZeroDivisionError
        except:
            # Code to handle any other exception

## else and finally Clauses:

        The "else" clause is used in the try-except block to specify code that should run if no exception occurs.
        The "finally" clause is used to specify code that should always run, regardless of whether an exception is raised or not.
        Syntax:
    
        python
    
            try:
                # Code that may raise an exception
            except ExceptionType:
                # Code to handle the exception
            else:
                # Code that runs if no exception occurs
            finally:
                # Code that always runs

# Example:

    python

  ## Example: Exception Handling
    
        try:
            num1 = int(input("Enter a number: "))
            num2 = int(input("Enter another number: "))
            result = num1 / num2
            print("Result:", result)
        except ValueError:
            print("Invalid input. Please enter valid integers.")
        except ZeroDivisionError:
            print("Division by zero is not allowed.")
        except Exception as e:
            print("An error occurred:", e)
        else:
            print("No exceptions occurred.")
        finally:
            print("Exception handling complete.")
    
  ## Output:
    
    csharp
    
    Enter a number: 10
    Enter another number: 0
    Division by zero is not allowed.
    Exception handling complete.

## Summary:
   In this example, the program takes two numbers as input from the user and performs division. 
   It uses a try-except block to handle possible exceptions such as ValueError (if the input is not an integer) and ZeroDivisionError (if the user enters 0 as the second number).
   The "else" clause is executed if no exceptions occur, and the "finally" clause runs regardless of whether an exception is raised or not.
