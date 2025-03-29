# Dictionary in Python

- **`Dictionary`** ---> A Python dictionary is a data structure that stores the value in key: value pairs.
- Values in a dictionary can be of any data type and can be duplicated, whereas keys can’t be repeated and must be immutable.

## # Decleration of Dictionary 

--> **2 Ways to declare Dictionary in Py.**

**(i)** `1st Way to declare Dictionary`

- Using **{}** (Dictionary Literal)

``` py
user = {
    "name": "Abhishek",
    "age": 21,
    "location": "Delhi",
    "email": "abhi@gmail.com",
    "is_logged_in": False,
    "last_login_days": ["Monday", "Saturday"],
    "full Name": "Abhishek Yadav"
}
```

**(ii)** `2nd Way to declare Dictionary`

- Using **dict ()** Constructor

```py
user = dict(name="Siddharth", age=19, location="Delhi")
```

## # Accessing Dictionary Items

--> **2 Ways to Access Dictionary items in Py.**

**(i)** Using the key within square.  
**(ii)** Using get() method.

``` py
print(user["email"])                          # Output : abhi@gmail.com
print(user.get("email"))                      # Output : abhi@gmail.com
print(user["full Name"])                      # Output : Abhishek Yadav
print(user.get("username", "Not Found"))      # Output : Default value if key is missing
```












