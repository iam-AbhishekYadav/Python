# Tuples in Python

- **`Tuple`** - An immutable ordered collection of elements.
- Tuples are similar to lists, but unlike lists, they cannot be changed after their creation (i.e., they are immutable).
- Tuples can hold elements of different data types.
- The main characteristics of tuples are being ordered , heterogeneous and immutable.

## # Decleration of Dictionary

--> Tuple is create by using **() parentheses**.

``` py
# Empty tuple

empty_tuple = ()
print(empty_tuple)                                                 # Output : ()                            

# Tuple with values

my_tuple = (1, 2, 3, "sidd", True, None)
print(my_tuple)                                                     # Output : (1, 2, 3, 'sidd', True, None)

# Tuple without parentheses (valid but not recommended)

my_tuple2 = 1, 2, 3
print(my_tuple2)                                                   # Output : (1, 2, 3)

# Single element tuple (comma जरूरी है)

single_element_tuple = (5,)  
print(type(single_element_tuple))                                  # Output : <class 'tuple'>

# Using tuple() constructor

my_tuple3 = tuple([1, 2, 3, 4])  
print(my_tuple3)                                                    # Output: (1, 2, 3, 4)                         
```



