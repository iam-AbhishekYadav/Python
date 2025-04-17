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
> [!WARNING]
> ( ) के बिना tuple बन सकता है, लेकिन readability के लिए parentheses इस्तेमाल करना बेहतर होता है।
> Single-element tuple में , लगाना जरूरी है, वरना ये integer या string माना जाएगा।

## # Indexing & Slicing

``` py
my_tuple = (10, 20, 30, 40, 50)

print(my_tuple[1])                    # Output: 20  (0-based indexing)
print(my_tuple[-1])                   # Output: 50  (Last element)

# Slicing (start:end:step)

print(my_tuple[1:4])                  # Output: (20, 30, 40)
print(my_tuple[:3])                   # Output: (10, 20, 30)
print(my_tuple[::2])                  # Output: (10, 30, 50)  (हर दूसरा element)
print(my_tuple[::-1])                 # Output: (50, 40, 30, 20, 10)  (Reverse tuple)
```

## # Tuple Methods

```py
my_tuple = (1, 2, 3, 4, 2, 5, 2)

print(my_tuple.count(2))    # Output: 3 (2 कितनी बार आया)
print(my_tuple.index(3))    # Output: 2 (3 का index)
```
## # Tuple Packing and Unpacking

**`Packing`** - Putting multiple values ​​in a tuple.
**`Unpacking`** - Putting tuple values ​​into separate variables.

```py
# Packing

packed_tuple = ("sidd", 21, "India")

# Unpacking

name, age, country = packed_tuple

print(name)     # Output: sidd
print(age)      # Output: 21
print(country)  # Output: India
```` 
> [!WARNING]
>  Unpacking करते समय values और variables की count match होनी चाहिए, नहीं तो error आएगा।

## # Merging Of Tuples

```py
tuple1 = (1, 2, 3)
tuple2 = (4, 5, 6)

# Concatenation (जोड़ना)

merged_tuple = tuple1 + tuple2
print(merged_tuple)  # Output: (1, 2, 3, 4, 5, 6)

# Repetition (एक tuple को multiple बार repeat करना)

repeated_tuple = tuple1 * 3
print(repeated_tuple)  # Output: (1, 2, 3, 1, 2, 3, 1, 2, 3)
```

## # Conversion Between List & Tuple

```py
# Tuple to List (Modification के लिए)
tuple1 = (1, 2, 3)
list1 = list(tuple1)  # Convert to list
list1.append(4)       # List को modify किया
tuple1 = tuple(list1)  # फिर से tuple में बदला
print(tuple1)  # Output: (1, 2, 3, 4)

# List to Tuple
list2 = [10, 20, 30]
tuple2 = tuple(list2)
print(tuple2)  # Output: (10, 20, 30)
```
## # Checking If an Element Exists in a Tuple

```py
my_tuple = ("apple", "banana", "cherry")

print("banana" in my_tuple)           # Output: True
print("grape" in my_tuple)            # Output: False
```

## # Looping Over a Tuple

```py
fruits = ("apple", "banana", "cherry")

# For loop
for fruit in fruits:
    print(fruit)

output: apple
        banana
        cherry

# Using enumerate() (index + value)
for index, fruit in enumerate(fruits):
    print(f"Index {index}: {fruit}")

output: Index 0: apple
        Index 1: banana
        Index 2: cherry
```

## # Finding Maximum, Minimum, and Sum in a Tuple

```py
numbers = (5, 2, 9, 1, 7)

print(max(numbers))  # Output: 9
print(min(numbers))  # Output: 1
print(sum(numbers))  # Output: 24
```

## #  Tuple as Dictionary Key (Immutable होने की वजह से Possible)

```py
# Tuples can be dictionary keys, unlike lists
locations = {
    (28.6139, 77.2090): "Delhi",
    (19.0760, 72.8777): "Mumbai"
}

print(locations[(28.6139, 77.2090)])  # Output: Delhi
```

## # Checking if an Object is a Tuple

```py
my_tuple = (1, 2, 3)
print(isinstance(my_tuple, tuple))  # Output: True

my_list = [1, 2, 3]
print(isinstance(my_list, tuple))  # Output: False
```







