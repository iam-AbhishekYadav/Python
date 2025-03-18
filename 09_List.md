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

## # Slicing and Dicing  

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












