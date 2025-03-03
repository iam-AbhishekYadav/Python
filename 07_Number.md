# # Numbers in Python

## # Basics

``` py
>>> x = 2
>>> y = 3
>>> z = 4
>>> 
>>> x + y                      Output : 5
>>>
>>> 40 + 2.23                  Output : 42.23
>>>
>>> 'Abhishek' + 2             Output : TypeError: can only concatenate str (not "int") to str
>>>
>>> int(2.53)                  Output : 2
>>>
>>> float(55)                  Output : 55.0
>>>
>>> 'Abhishek' + ' Yadav'       Output : Abhishek Yadav
>>>
>>> x = 1
>>> y = 2
>>> z = 3
>>>
>>> x,y,z                        Output : (1, 2, 3)
>>>
>>> 1 < 2                         Output : True
>>>
>>> 5.0 == 5.0                    Output : True
>>>
>>> 4.0 != 5.0                    Output : True
>>>
>>> (2 +1 j) * 3                     Output : (6 + 3j
```

``` py
>>> x = 1
>>> y = 2
>>> z = 3
>>>
>>> x,y,z                           Output : (1,2,3)
>>>
>>> x<y<z                           Output : True
>>>
>>> x < y and y < z                 Output : True
>>> 
>>> 1 == 2 < 3                      Output : False
>>>
>>> 1 == 2 and 2 < 3                 Output : False
```


## # Exponents in Python

- **`**`** :  x ** y computes x raised to the power of y.
- **`pow()`** : This built-in function takes two arguments: the base and the exponent. pow(x,y)
- **`math.pow()`** : It always returns a floating-point result.

``` py
>>> 2 ** 3                        Output : 8
>>>
>>> pow(2,4)                      Output : 16
>>>
>>> import math
>>> math.pow(2,3)                 Output : 8.0
```


## # Library Import


``` py
>>> import math
>>> 
>>> math.floor(3.7)                  Output : 3          # Closest bottom value
>>> math.floor(-3.5)                 Output : -4
>>>
>>> math.trunc(2.8)                   Output : 2        # Towards zero
>>> math.trunc(-2.8)                  Output : -2
```


## # Random Library

- **`random()`** : It returns a random floating number between 0 and 1.

``` py
>>> import random
>>> random.random()                       Output : 0.6036513999382547
>>>
>>> random.randint(1,100)                 Output : 6   ( Give random number between 1 and 100 )
>>>
```

- **`Random choice()`** : It returns a randomly selected element from the specified sequence.

``` py
>>> import random
>>> mylist = ["apple", "banana", "cherry"]
>>>
>>> print(random.choice(mylist))                    Output : banana
```

- **`Random shuffle()`** : The shuffle() method takes a sequence, like a list, and reorganize the order of the items.

``` py
>>> import random
>>> mylist = ["apple", "banana", "cherry"]
>>>
>>> print(random.shuffle(mylist))                    Output : ['cherry', 'banana', 'apple']
```

## # Another types of Number

``` py 
>>> 0o20                       Output : 16        # Octal   oct(16)
>>>
>>> 0xFF                       Output : 255       # Hexal   hex(255)
>>>
>>> 0b1000                     Output : 8         # Binary  bin(8)
>>>
>>> int("64",8)                 Output : 52       # convert in Octal
>>> int("64",16)                Output : 100      # convert in Hexal
>>> int("10000",2)              Output : 16       # convert in Binary
```

## # Interesting Problem

```py
>>> 0.1 + 0.1 + 0.1                    Output : 0.30000000000000004
>>>
>>>  0.1 + 0.1 + 0.1 - 0.3             Output :  5.551115123125783e-17
>>>
>>> from decimal import Decimal        # decimal context manager
>>>
>>>  Decimal('0.1') + Decimal('0.1') + Decimal('0.1') - Decimal('0.3')           Output : Decimal('0.0')
>>>
>>> fram fraction import Fraction
>>> myFrac = Fraction(2,7)
>>> myFrac                                Output : Fraction(2,7)
```


## # Sets 

``` py
>>> setOne = {1,2,3,4,5}
>>>
>>> setOne & {4,5,6,7,8}                  Output : {4,5}
>>> setOne | {1,8,5,9}                    Output : {1,2,3,4,5,8,9}
>>>
>>> setOne - {1,2,3,4,5}                  Output : set()     (Empty set is not given becasue It is Dictonary)
>>>
>>> type ({})                             Output : <class 'dict'>
```






































