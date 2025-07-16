# # Object Oriented Programming in python

Python is an object-oriented language, allowing you to structure your code using classes and objects for better organization and reusability.

## Advantages of OOP

- Provides a clear structure to programs
- Makes code easier to maintain, reuse, and debug
- Helps keep your code DRY (Don't Repeat Yourself)
- Allows you to build reusable applications with less code

# # Class in Python

- A class in Python is a user-defined template for creating objects.
- A class defines a set of attributes and methods that the created objects (instances) can have.

## Some points on Python class 

- Classes are created by keyword class.
- Attributes are the variables that belong to a class.
- Attributes are always public and can be accessed using the dot (.) operator.
  - Example ---> Myclass.Myattribute

``` py
class Dog:
    species = "Canine"                  # Class attribute

    def __init__(self, name, age):
        self.name = name                # Instance attribute
        self.age = age                  # Instance attribute
```

# # Object in Python

- An object is refered to as an instance of a given Python class.
- Each object has its own attributes and methods, which are defined by its class.

``` py
class Dog:
    def __init__(self, name, age):
        self.name = name                        # Instance attribute
        self.age = age                          # Instance attribute

# Creating an object of the Dog class
dog1 = Dog("Buddy", 3)

print(dog1.name)                                # Output : Buddy
print(dog1.age)                                 # Output : 3
```
# # Class Method and Self

**`Problem`** ---> Add a method to Car Class that displays the full name of the car (Brand and Model)

``` py
class Car:
    def __init__(self, brand ,model):
        self.brand = brand
        self.model = model

    def fullName(self):
        return f"{self.brand} {self.model}"
    

my_car = Car("Tata", "Safari")

print(my_car.brand)                                 # Output : Tata
print(my_car.model)                                 # Output : Safari

print(my_car.fullName())                            # Output : Tata Safari
```
































