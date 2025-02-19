# # Internal Working Of Python

## # Refrence Count

- Python and various other programming languages employ reference counting, a memory management approach, to automatically manage memory by tracking how many times an object is referenced.

``` py
PS D:\Desktop\File_Name> Python

>>> impot sys
>>> sys.getrefrencecount('Abhishek')        Output : 4294967295 (Internaly a complier optimization loop runs)
>>> sys.getrefrencecount('A')               Output : 4294967295
>>> sys.getrefrencecount(2)                 Output : 4294967295
```

<img src="https://github.com/user-attachments/assets/ae42ce45-5b71-440c-9251-48e27dcb1dc5" alt="Stack1" width="750" height="400">


- ### In List


<img src="https://github.com/user-attachments/assets/49ce0bc2-9c69-4134-943a-b71020bfb8ef" alt="Stack1" width="650" height="300">

``` py 
PS D:\Desktop\File_Name> Python

>>> myListOne = [1,2,3]
>>> myListTwo = myListOne
>>>
>>> myListOne                  Output : [1,2,3] 
>>>
>>> myListTwo                  Output : [1,2,3] 
>>>
>>> myListOne[0] = 55
>>> myListOne                  Output : [55,2,3] 
>>>
>>> myListTwo                  Output : [1,2,3]
```

> Examples - 01

``` py
PS D:\Desktop\File_Name> Python

>>> l1 = [1,2,3]
>>> l2 = l1
>>> 
>>> l1                     Output : [1,2,3]
>>> l2                     Output : [1,2,3]
>>>
>>> l1 [0] = 44
>>>
>>> l1                    Output : [44,2,3]
>>> l2                    Output : [44,2,3]
```
























