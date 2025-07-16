# String In Python


# # String Declaration

``` py
>>> Juice = "Apple Juice"
>>>
>>> Juice                             # Output : Apple Juice 
>>> print(Juice)                      # Output : Apple Juice
```

# # Slicing and Dicing

- It Cut elements on the bases of index.
- slice[start,end]
- slice[start,end,hoping]

``` py
>>> name = "Abhishek Yadav"
>>> slice_name = name[0:6]
>>> print(slice_name)                          # Output : 'Abhishek'
>>>
>>> name = [-1]                                # Output : 'v'
```

``` py
>>> num_list = "0123456789"
>>>
>>> num_list[:]                              # Output : '0123456789'
>>> num_list[3:]                             # Output : '3456789'
>>> num_list[:7]                             # Output : '0123456'
>>>
>>> num_list[0:7:2]                          # Output : '026'   (3rd parameter is for hoping)
```

# # String Properties and Methods

``` py
str1 = "Hello World"

print(len(str1))                     # Output: 11
print(str1[1])                       # Output: 'e'
print(str1.index('l'))               # Output: 2
print(str1[1:4])                     # Output: 'ell' (Slicing)
print(str1.upper())                  # Output: 'HELLO WORLD'
print(str1.lower())                  # Output: 'hello world'
print(str1.replace('H', 'J'))        # Output: 'Jello World'
print(str1.split(' '))               # Output: ['Hello', 'World']
print(str1.strip())                  # Removes leading/trailing spaces
print(str1.find("World"))            # Output: 6
print(str1.count("World"))           # Output: 1
```


# # Order Formating 

















