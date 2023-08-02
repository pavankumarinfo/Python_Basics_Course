# Topic 5: Lists and Dictionaries

In this topic, we'll explore two important data structures in Python: lists and dictionaries. Lists allow us to store collections of items, while dictionaries provide a way to store data as key-value pairs.

Items covered:

   ## Lists:
            Lists are ordered collections of elements, enclosed in square brackets [].
            They can contain elements of different data types (e.g., numbers, strings, other lists).
            Syntax:
    
            python
    
        my_list = [1, 2, 3, "apple", "banana"]

## Accessing List Elements:

      You can access elements in a list using their index (starting from 0).
      Negative indices count from the end of the list.
      Example:
  
      python
  
      fruits = ["apple", "banana", "orange"]
      print(fruits[0])  # Output: apple
      print(fruits[-1])  # Output: orange

## List Operations:

        Lists support various operations, such as slicing, appending, removing, and concatenating.
        Example:
    
        python
    
        numbers = [1, 2, 3, 4, 5]
        numbers[2] = 10  # Modify an element: [1, 2, 10, 4, 5]
        numbers.append(6)  # Add an element to the end: [1, 2, 10, 4, 5, 6]
        numbers.remove(2)  # Remove an element by value: [1, 10, 4, 5, 6]

## Dictionaries:

        Dictionaries are unordered collections of key-value pairs, enclosed in curly braces {}.
        Each key in the dictionary must be unique, and keys are used to access corresponding values.
        Syntax:
    
        python
    
        my_dict = {"name": "John", "age": 25, "city": "New York"}

## Accessing Dictionary Values:

        You can access values in a dictionary using their keys.
        Example:
    
        python
    
        person = {"name": "John", "age": 25, "city": "New York"}
        print(person["name"])  # Output: John

## Modifying and Adding Dictionary Items:

        You can modify or add new items to a dictionary by assigning values to keys.
        Example:
    
        python
    
        person["age"] = 26  # Modify an existing item
        person["job"] = "Engineer"  # Add a new item

## Dictionary Operations:

        Dictionaries support various operations, such as removing items and checking key existence.
        Example:
    
        python
    
            car = {"brand": "Toyota", "model": "Camry"}
            del car["model"]  # Remove an item by key: {"brand": "Toyota"}
            print("brand" in car)  # Check key existence: True
    
## Summary:
      Lists and dictionaries are powerful data structures that allow you to organize and manipulate data efficiently in Python. 
      They are widely used in various programming tasks, from data processing to handling complex datasets. 
      Practice using lists and dictionaries to become more comfortable with their functionalities.
