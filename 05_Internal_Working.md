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

<img src="https://github.com/user-attachments/assets/ae42ce45-5b71-440c-9251-48e27dcb1dc5" alt="Stack1" width="750" height="500">


## In List

