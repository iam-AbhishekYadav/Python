# # Scope and Closure in Python

# # Scope in Python

- **`Scope`** --> A variable is only available from inside the **`{---}`** region it is created.

## Local Scope

- A variable created inside a function belongs to the local scope of that function, and can only be used inside that function.

### Example --->
``` py
UserName = "Abhishek Yadav"

def func():
    UserName = "Sachin Yadav"
    print(UserName)

print(UserName)                     # Output : Abhishek Yadav
func()                              # Output : Sachin Yadav
```

## Global Scope

- A variable created in the main body of the Python code is a global variable and belongs to the global scope.
- A variable created outside of a function is global and can be used by anyone:


### Example --->
- Here, We comment out the UserName in Function.
- When python UserName not found in function it goes go up above to find the UserName

``` py
UserName = "Abhishek Yadav"

def func():
  # UserName = "Sachin Yadav"            # Comment out this UserName
    print(UserName)

print(UserName)                     # Output : Abhishek Yadav
func()                              # Output : Abhishek Yadav
```

## Global Keyword

- If you need to create a global variable, but are stuck in the local scope, you can use the global keyword.
- Also, use the global keyword if you want to make a change to a global variable inside a function.
- Avoid this Global Keywoard to use.

``` py
x = 300

def myfunc():
  global x
  x = 200

myfunc()
print(x)               # Output : 200
```

## Function Inside Function Scope

- The variable is available for any function inside the function.
- The local variable can be accessed from a function within the function:

``` py
x = 99

def myfunc():
    x = 300
    def myinnerfunc():
        print(x)                   # Output : 300
        myinnerfunc()

myfunc()
```

# # Closure in Python

- A nested function that allows us to access variables of the outer function even after the outer function is closed.

``` py
def fun1():
    x = 300
    def fun2():
        print(x)                   # Output : 300
    return fun2


result = fun1()
result()
```

























