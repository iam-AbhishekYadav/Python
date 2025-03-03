# String In Python

## # String Declaration

``` py
>>> Juice = "Apple Juice"
>>>
>>> Juice                             # Output : Apple Juice 
>>> print(Juice)                      # Output : Apple Juice
```

## # Slicing and Dicing

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





















