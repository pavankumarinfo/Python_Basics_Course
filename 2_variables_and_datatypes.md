  In this topic, we'll explore the concept of variables and data types in Python. Variables allow us to store and manipulate data, while data types define the type of data that can be stored in variables.

  ## Items covered:
  
  ### Variables:
      Variables are containers used to store data in Python.
      You can assign values to variables using the "=" operator.
      For example: age = 25 assigns the value 25 to the variable "age."

  ### Data Types:
        Python supports several built-in data types, including:
            Integer: Whole numbers, e.g., 10, -5, 0.
            Float: Decimal numbers, e.g., 3.14, -0.5.
            String: Sequence of characters, e.g., "Hello", 'Python'.
            Boolean: Represents True or False values.

 ### Dynamic Typing:
        Python is dynamically typed, meaning you don't need to specify the data type of a variable explicitly.
        The data type is determined automatically based on the assigned value.
        For example: message = "Hello" automatically assigns the string data type to the variable "message."

 ### Type Conversion (Typecasting):
            You can convert data from one type to another using typecasting.
            For example, str(42) converts the integer 42 to a string "42."

 ### Variable Naming Rules:
         Variable names can contain letters (a-z, A-Z), numbers (0-9), and underscores (_).
         They cannot start with a number or contain special characters.
         Python is case-sensitive, so "age" and "Age" are different variables.

 ### Printing Variables:
       You can use the print() function to display the values of variables.
       For example: print(age) will display the value of the variable "age."

  ### Arithmetic Operations:
         You can perform basic arithmetic operations on numeric variables:
              Addition: a + b
              Subtraction: a - b
              Multiplication: a * b
              Division: a / b
              Modulo (Remainder): a % b
              Exponentiation: a ** b

  ### String Operations:
          Strings support various operations, such as concatenation and slicing:
              Concatenation: "Hello" + " " + "Python"
              Slicing: "Python"[0:3] returns "Py".
  ### Boolean Operations:
          Boolean variables can be combined using logical operators:
            AND: True and False evaluates to False.
            OR: True or False evaluates to True.
            NOT: not True evaluates to False.

   ### Practice Exercises:
          To reinforce your understanding, we'll provide practice exercises involving variables and different data types.

   ### Example:
    
     Understanding variables and data types is fundamental to programming in Python. With this knowledge, you can store and manipulate data effectively in your programs. Keep practicing and exploring more Python concepts to build a solid foundation. Happy coding!

  ### Example:

  ### Example: Variables and Data Types
        
        # Variables
        name = "John"
        age = 25
        height = 1.75
        is_student = True
        
        # Printing variables
        print("Name:", name)
        print("Age:", age)
        print("Height:", height)
        print("Is Student:", is_student)
        
        # Basic arithmetic operations
        a = 10
        b = 5
        sum_result = a + b
        diff_result = a - b
        mul_result = a * b
        div_result = a / b
        mod_result = a % b
        exp_result = a ** b
        
        print("Sum:", sum_result)
        print("Difference:", diff_result)
        print("Multiplication:", mul_result)
        print("Division:", div_result)
        print("Modulo:", mod_result)
        print("Exponentiation:", exp_result)
        
        # String operations
        message = "Hello" + " " + "Python"
        print("Message:", message)
        
        # Boolean operations
        is_adult = age >= 18
        is_tall = height > 1.80
        can_vote = is_adult and not is_student
        print("Is Adult:", is_adult)
        print("Is Tall:", is_tall)
        print("Can Vote:", can_vote)

### Output
      Name: John
      Age: 25
      Height: 1.75
      Is Student: True
      Sum: 15
      Difference: 5
      Multiplication: 50
      Division: 2.0
      Modulo: 0
      Exponentiation: 100000
      Message: Hello Python
      Is Adult: True
      Is Tall: False
      Can Vote: True
