# Topic 6: Input and Output

In this topic, we'll learn how to interact with users through input and display output in Python. We'll use input functions to receive user input and output functions to display information on the screen.

Items covered:

## Input Function:
        The "input()" function allows us to receive input from the user through the console.
        It takes a prompt (optional) as an argument, which is displayed to the user before waiting for input.
        The input is always received as a string, so typecasting might be necessary for numeric operations.
        Syntax:

        python

    user_input = input("Enter your name: ")

## Output Function:

        The "print()" function is used to display output on the console.
        It can take multiple arguments separated by commas and print them with spaces by default.
        The "end" parameter can be used to change the ending character (default is a newline).
        Syntax:
    
        python
    
        name = "John"
        print("Hello,", name)  # Output: Hello, John
        print("Hello,", name, end="!")  # Output: Hello, John!

## Formatted Output:

        We can use string formatting to include variables and formatted text in print statements.
        The "%" operator and format() method are commonly used for string formatting.
        Example:
    
        python
    
        name = "John"
        age = 25
        print("Name: %s, Age: %d" % (name, age))  # Output: Name: John, Age: 25
        print("Name: {}, Age: {}".format(name, age))  # Output: Name: John, Age: 25

## Reading and Writing Files:

        Python allows us to read data from files and write data to files using file objects.
    
        We use the "open()" function to create a file object and specify the file mode (read, write, append, etc.).
    
        Example of reading from a file:
    
        python
    
    with open("data.txt", "r") as file:
        content = file.read()
        print(content)
    
    Example of writing to a file:
    
    python
    
            with open("output.txt", "w") as file:
                file.write("Hello, this is a new file.")

## Summary :
    The input and output functions are fundamental for creating interactive programs.0 
    They allow users to provide input and receive meaningful information from the program. 
    File input/output is crucial for reading and writing data to external files, which is essential for handling data in real-world applications. 
    Practice using input, output, and file handling to enhance your programming skills.
