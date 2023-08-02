# Topic 8: Object-Oriented Programming (OOP)

In this topic, we'll explore the principles of Object-Oriented Programming (OOP) in Python. OOP is a programming paradigm that uses objects and classes to structure and model real-world entities.

Items covered:

   ## Classes and Objects:
            Classes are blueprint or templates that define the structure and behavior of objects.
            Objects are instances of classes, representing specific entities with unique characteristics.
            Syntax to define a class:
    
            python
    
        class MyClass:
            def __init__(self, parameter1, parameter2):
                self.attribute1 = parameter1
                self.attribute2 = parameter2

## Constructors and Initialization:

        The __init__() method is a special method used to initialize the object's attributes when the object is created.
        It is also known as the constructor of the class.
        Example:
    
        python
    
        class Person:
            def __init__(self, name, age):
                self.name = name
                self.age = age
    
        person1 = Person("John", 25)
        person2 = Person("Alice", 30)

## Class Methods and Instance Methods:

        Class methods are methods that act on the class itself and are defined using the @classmethod decorator.
        Instance methods are methods that operate on individual instances of the class and take self as the first parameter.
        Example:
    
        python
    
        class MyClass:
            class_attribute = 10
    
            @classmethod
            def class_method(cls):
                print("This is a class method.")
    
            def instance_method(self):
                print("This is an instance method.")

## Inheritance:

        Inheritance allows a class (subclass) to inherit attributes and methods from another class (superclass).
        It helps to create a hierarchy of classes with specialized behavior.
        Syntax to create a subclass:
    
        python
    
            class SubClass(SuperClass):
                def __init__(self, parameter1, parameter2):
                    super().__init__(parameter1, parameter2)
                    # Additional subclass-specific attributes and methods

## Example:

  python

  ## Example: Object-Oriented Programming
    
        class Car:
            def __init__(self, make, model, year):
                self.make = make
                self.model = model
                self.year = year
        
            def display_info(self):
                print(f"Car: {self.year} {self.make} {self.model}")
        

      class ElectricCar(Car):
          def __init__(self, make, model, year, battery_capacity):
              super().__init__(make, model, year)
              self.battery_capacity = battery_capacity
      
          def display_info(self):
              super().display_info()
              print(f"Battery Capacity: {self.battery_capacity} kWh")


      my_car = Car("Toyota", "Camry", 2022)
      my_car.display_info()
      
      my_electric_car = ElectricCar("Tesla", "Model S", 2023, 100)
      my_electric_car.display_info()

## Output:

    yaml
    
    Car: 2022 Toyota Camry
    Car: 2023 Tesla Model S
    Battery Capacity: 100 kWh

## Summary:
    In this example, we define a Car class with attributes make, model, and year, along with an instance method display_info() to display car details. 
    We then create an ElectricCar subclass that inherits from the Car class and has an additional attribute battery_capacity.
    The display_info() method is overridden in the subclass to include the battery capacity along with the car details.
