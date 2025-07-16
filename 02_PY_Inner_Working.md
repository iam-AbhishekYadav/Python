# # Python Inner Working 

- First we have to use Python interpreter/Software.
- Which Script/Program is running (Ex ---> Abhi.py).
  
<img src="https://github.com/user-attachments/assets/f26ad088-2ff4-4f3b-a657-c3aa95f0ea80" alt="Stack1" width="800" height="400">

- Compile to Byte Code (Low level & Platform Independent).
- Byte code run faster.
- - `.pyc` ---> Compiled Python (Frozin Binaries)
  - __ pycache __
  - `File_Name.cpython-3.12.pyc`  (Source Change & Python Version)
- Work only for imported files.
- Not for top level files.


## # Python Virtual Machine (PVM)

- Code loop to iterate byte code.
- Run time Engine
- Also Known as Python Interpreter
- Byte Code is not machin code
- Python specific Interpretation
- cPython (Standard implementation) , Iron Python , Stackless.pypy

# # Python Shell

- Through this we can import without file name.
``` py
PS D:\Desktop\File_Name> Python
>>> import os
>>> os.getcwd()       Output : 'D:\\Desktop\\File_Name'
```
