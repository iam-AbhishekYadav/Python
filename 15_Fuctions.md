# Functions In Python

- **`Functions`** is a block of statements that return the specific task.
- writing the same code again and again for different inputs, we can do the function calls to reuse code contained in it over and over again.
- It increase Code Readability and Reusability.

## # Syntax

<img src="https://github.com/user-attachments/assets/1a4b4270-4894-43da-b4f8-009c8d2e2353" alt="Stack1" width="550" height="300">

#### Example --->

``` py
def square(number):
     return number ** 2                                      
     
result = square(4)                                          
print(result)                   # Output : 16
```

## # Types of Functions in Python

- There are two types of functions in python.

**(i)** **`Built-in library function`** ---> These are Standard functions in Python that are available to use.

**(ii)** **`User-defined function`** ---> We can create our own functions based on our requirements.

## # Lambda Function 

- Lambda Functions are anonymous functions means that the function is without a name.

- **`Syntax`** ---> &nbsp; **lambda  &nbsp; arguments &nbsp; : &nbsp; expression**
  - **Lambda** = The keyword to define the function.
  - **Arguments** = A comma-separated list of input parameters (like in a regular function).
  - **Expression** = A single expression that is evaluated and returned.


 #### Example --->
 
``` py
cube = lambda x : x**3

print(cube(3))                  # Output : 27
```

## # Mutiple Arguments

--> There are two ways of arguments in python.

**(i)** **`*args`**

- If we want to make a multiply function that takes any number of arguments and is able to multiply them all together. It can be done using *args.

```py
def sum_all(*args):
     return sum(args)

print(sum_all(1,2,3))                      # Output : 6
print(sum_all(1,2,3,4,5))                  # Output : 15
print(sum_all(1,2,3,4,5,6,7,8,9))          # Output : 45
```




















