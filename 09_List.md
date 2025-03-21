# List in Python

## # Declaring of List

``` py
my_list1 = [0, 1, 23, True, "sidd", None]  
my_list2 = list((0, 1, 2, 3, 4, 5))

print(my_list1)                              # Output: [0, 1, 23, True, "sidd", None] 
print(my_list2)                              # Output: [0, 1, 2, 3, 4, 5]
```

## # Accessing List Elements

- Elements in a list can be accessed using indexing.

```py
my_list = [10, 20, 30, 40, 50]

print(my_list[0])                   # Output: 10
print(my_list[-1])                  # Output: 50

print(my_list.count("30"))          # Output: 2
print("20" in my_list)              # Output: True        
```

## # Slicing in List

- It Cut elements on the bases of index.
- **Syntax** : list_name[stat : end : step]
- - Parameters:
  - start : Index to begin the slice (inclusive). Defaults to 0 if omitted.
  - end : Index to end the slice (exclusive). Defaults to the length of list if omitted.
  - step : Step size, specifying the interval between elements. Defaults to 1 if omitted

``` py
my_list = [1, 2, 3, 4, 5, 6, 7, 8, 9]

print(a[:})

## # Properties and Methods in List

**(i) `Sort()`**

- The list in ascending order (by default).

``` py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.sort()
print(my_list)                     # Output : [1, 2, 3, 4, 5, 6]
```

**(ii) `reverse()`**

- Reverses the order of the elements in the list.

``` py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.reverse()
print(my_list)                     # Output : [4, 6, 5, 2, 1, 3]
```

**(iii) `append()`**

- Adds an element to the end of the list.

```py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.append(22)
print(my_list)                     # Output : [3, 1, 2, 5 , 6, 4, 22]
```

**(iv) `insert()`**

- It will insert an element at a specific position in the list.
- **Syntax** : list_name.insert(index, element)

``` py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.append(2,55)
print(my_list)                     # Output : [3, 1, 2, 55, 5 , 6, 4]
```

**(v) `pop()`**

- Removes and returns the element at the specified position (or the last element if no index is specified).
- It gives eco back.
- **Syntax** : list_name.pop(index)

``` py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.pop()
print(my_list)                     # Output : [3, 1, 2, 5 , 6]

my_list.pop(3)
print(my_list)                    # Output :  [3, 1, 2, 6, 4]
```

**(vi) `remove()`**

- Removes the first occurrence of a specified element.
- **Syntax** : list_name.remove(element)

``` py
my_list = [3, 1, 2, 5 , 6, 4]

my_list.remove(6)
print(my_list)                     # Output : [3, 1, 2, 5 , 4]
```

## # Merge Two List in Python

- There are different methods to merge list in Python.

**(i) `Using + operator`**

```py
marvel_heros = ["Thor", "Ironman", "Spiderman"]
dc_heros = ["Superman", "Flash", "Tatman"]

all_heros = marvel_heros + dc_heros
print(all_heros)                            # Output: ['thor', 'ironman', 'spider', 'super', 'flash', 'batman']
```

**(ii) `Using extend()`**

- It modifies the original list by adding elements from another list.

```
marvel_heros = ["Thor", "Ironman", "Spiderman"]
dc_heros = ["Superman", "Flash", "Tatman"]

marvel_heros.extend(dc_heros)
print(marvel_heros)                         # Output: ['thor', 'ironman', 'spider', 'super', 'flash', 'batman']
```

**(iii) `Using unpacking or * operator`**

- Recommended for better readability.

``` py
marvel_heros = ["Thor", "Ironman", "Spiderman"]
dc_heros = ["Superman", "Flash", "Tatman"]

all_new_heros = [*marvel_heros, *dc_heros]
print(all_new_heros)                            # Output: ['thor', 'ironman', 'spider', 'super', 'flash', 'batman']
```


## # Iteration in List

```py
my_list2 = [0, 1, 2, 3, 4, 5]
print(my_list2)                                                 # [0, 1, 2, 3, 4, 5]

for element in my_list2:
    print(element)                                              # Output: 0 1 2 3 4 5

print([element * 2 for element in my_list2])                    # Output: [0, 2, 4, 6, 8, 10]
print([element for element in my_list2 if element > 1])         # Output: [2, 3, 4, 5]
```


## # List Comprehension

``` py
squares = [x**2 for x in range(1, 6)]
print(squares)                                               # Output: [1, 4, 9, 16, 25]

even_numbers = [x for x in range(10) if x % 2 == 0]
print(even_numbers)                                           # Output: [0, 2, 4, 6, 8]
```





