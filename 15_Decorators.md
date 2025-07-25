# # Decorators in Python

- A powerful and flexible way to modify or extend the behavior of functions or methods, without changing their actual code.
- A decorator is essentially a function that takes another function as an argument and returns a new function with enhanced functionality
- Decorators are often used in scenarios such as logging, authentication and memorization, allowing us to add additional functionality to existing functions or methods in a clean, reusable way.

### Syntax

``` py
def decorator_name(func):
    def wrapper(*args, **kwargs):

        # Add functionality before the original function call
        result = func(*args, **kwargs)

        # Add functionality after the original function call
        return result

    return wrapper

@decorator_name
def function_to_decorate():
    # Original function code
    pass
```

## Timing Function Execution

**`Problem`** ---> Write a decorator that measures the time of a function takes to execute

``` py
import time

def timer(func):
    def wrapper(*args, **kwargs):
        start = time.time()                                         # Calculate Sarting time 
        result = func(*args, **kwargs)
        end = time.time()                                           # Calculate Ending time
        print(f"{func.__name__} run in {end-start} time")
        return result
    return wrapper

@timer                                                              # Decorator
def example_function(n):
    time.sleep(n)                                                   # Delay execution for a given number of seconds.

example_function(2)                                                 # Output : example_function run in 2.0004477500915527 time
```

















