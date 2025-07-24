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

### __ init __ Function/Constructor

- All classes have a function called __init()
- Which is always execute when the class is being initiated.
- It always takes a parameter Self

### Self
The self parameter is a reference to the current instance of the class and is used to access variables that belongs to the class.


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

# # Inheritance

- Inheritance allows a class (called a child or derived class) to inherit attributes and methods from another class (called a parent or base class).
- It promotes code reusability by sharing attributes and methods across classes.

**`Super Method`** ---> It is used to access methods of the parent class.
```py
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def fullName(self):
        return f"{self.brand} {self.model}"
    
class ElectricCar(Car):
    def __init__(self, brand, model, battery_size):
        super().__init__(brand, model)
        self.battery_size = battery_size

my_car = ElectricCar("Tesla", "Model - S", "85kwh")

print(my_car.brand)                                 # Output : Tesla
print(my_car.model)                                 # Output : Model - S
print(my_car.battery_size)                          # Output : 85kwh

print(my_car.fullName())                            # Output : Tesla Model - S
```

# # Abstraction

- Hidding the implementation details of a class and only showing the essential features to the user.
- This approach helps in reducing the complexity and increasing the efficiency of application development.

``` py
class Car:
    def __init__(self):
        self.acc = False
        self.brk = False
        self.clucth = False

    def start(self):
        self.clucth = True
        self.acc = True
        print("Cra satrted ...")                                   # Output : Car started ...
    

my_car = Car()
my_car.start()
```

# # Encapsulation

- Encapsulation is the process of wrapping data and function into a single unit (object).
- It protects data from unauthorized access and accidental modification.
- Enhances modularity by hiding internal implementation details.

## Access Specifiers

<img src="https://github.com/user-attachments/assets/2fa89236-af43-4785-98b2-b33a7a39167b"  width="500" height="350">

 **(i)** **`Public Members`** ---> 

 - Public members are accessible from anywhere, both inside and outside the class.
 - These are the default members in Python.

``` py
class Public:
    def __init__(self):
        self.name = "John"

    def display_name(self):
        print(self.name)                     # Output : Jhon

obj = Public()
obj.display_name()
print(obj.name)                             # Output : Jhon
```

**(ii)** **`Protected Members`** ---> 

- Protected members are identified with a single underscore (_).
- They are meant to be accessed only within the class or its subclasses.

``` py
class Protected:
    def __init__(self):
        self._age = 30          # Protected attribute

class Subclass(Protected):
    def display_age(self):
        print(self._age)        # Accessible in subclass

obj = Subclass()
obj.display_age()               # Output : 30
```
**(iii)** **`Private Members`** ---> 

- Private members are identified with a double underscore (__).
- It cannot be accessed directly from outside the class.

``` py
class Private:
    def __init__(self):
        self.__salary = 50000   # Private attribute

    def salary(self):
        return self.__salary   # Access through public method

obj = Private()
print(obj.salary())           # Works
# print(obj.__salary)         # Raises AttributeError
```

# # Polymorphism 

- The word "polymorphism" means "many forms"
- In programming it refers to methods/functions/operators with the same name that can be executed on many objects or classes.

``` py
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def move(self):
        print("Drive!")

class Boat:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def move(self):
        print("Sail!")

class Plane:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def move(self):
        print("Fly!")

car1 = Car("Ford", "Mustang")       #Create a Car object
boat1 = Boat("Ibiza", "Touring 20") #Create a Boat object
plane1 = Plane("Boeing", "747")     #Create a Plane object

for x in (car1, boat1, plane1):
    x.move()
```

# # Class Variable

- A class variable is a variable that is declared inside of a Class but outside of any instance method or __init__() method.
- Class Variable (also known as class attributes) are shared across all instances (objects) of a class.
- They belong to the class itself, not to any specific instance.


<img src="https://github.com/user-attachments/assets/909286dd-a6b3-4061-8837-8f6397cfe2f7"  width="450" height="450">

``` py
class Student:
    # Class variable
    school_name = 'ABC School '
    
    def __init__(self, name, roll_no):
        self.name = name
        self.roll_no = roll_no

# create first object
s1 = Student('Emma', 10)

# access class variable
print(s1.name, s1.roll_no, Student.school_name)                 # Output : Emma 10 ABC School

# create second object
s2 = Student('Jessa', 20)

# access class variable
print(s2.name, s2.roll_no, Student.school_name)                 # Output : Jessa 20 ABC School
```

# # Static Method

- Static method is a type of method that does not require any instance to be called.
- Static method that don't use the self parameter (Work at class level).
- It is very similar to the class method but the difference is that the static method doesn't have a mandatory argument like reference to the object − self or reference to the class.
- Static method can't access or modify class state and generally for utility.

## How to Create Static Method in Python?

There are two ways to create Python static methods −

- Using **`staticmethod()`** Function
- Using **`@staticmethod`** Decorator

``` py
class Employee:
    empCount = 0
    def __init__(self, name, age):
        self.__name = name
        self.__age = age
        Employee.empCount += 1

    # creating staticmethod
    @staticmethod
    def showcount():
        print (Employee.empCount)

e1 = Employee("Bhavana", 24)
e2 = Employee("Rajesh", 26)
e3 = Employee("John", 27)

e1.showcount()                            # Output : 3
Employee.showcount()                      # Output : 3
```

# # Class Method 

- A class method is bound to the class and receives the class as an implicit first argument.
- Class method works with the class since its parameter is always the class itself.

``` py
class Person :
    name = "anonynomus"

    @classmethod
    def changeName(cls, name):
        cls.name = name


P1 = Person()
P1.changeName("Abhishek Yadav")

print(P1.name)                         # Output : Abhishek Yadav
print(Person.name)                     # Output : Abhishek Yadav
```

# # Property Method 

- We use @property decorator on any method in the class to use the method as a property.
- t allows developers to create properties within a class, providing a way to control access to an attribute.

``` py
class Student:
    def __init__(self, phy, chem, math):
        self.phy = phy
        self.chem = chem
        self.math = math


    @property
    def percentage(self):
        return str((self.phy + self.chem + self.math) / 3) + "%"
    
student1 = Student(98, 97, 99)
print(student1.percentage)                            # Output : 98.0 %

student1.phy = 86                                     # Change Student1 Phy marks by 86
print(student1.percentage)                            # Output : 94.0 %
```




























