# Questions On Conditions

## # Question - 1

> **`Age Group Categorization`** --> Classify A person's age group : Child(<13) , Teenager(13-19) , Adult(20-59) , Senior(60+).

## Solution :-

```py
age = int(input("Enter Your age :"))

if age < 13 :
    print("Child")

elif age < 20 :
    print("Teenager")

elif age < 60 :
    print("Adult")

else : print("Senior")
```

## # Question - 2

> **`Movie Ticket Pricing`** --> Movie Ticket are price based on age : $12 for Adult (18 and over) , $18 for children. Everyone gets a $12 discount on Wednesday.

## Solution :-
```py
age = int(input("Enter Your age :"))
day = input("Enter the day :")

price = 12 if age >= 18 else 8

if day == "wed" :
    price = price - 2

print("Movie Ticket Price or you is $",price)
```

## # Question - 3

> **`Grade Calulator`** --> Assign a letter grade based on a student's score : A(90-100) , B(80-89) , C(70-79), D(60-69) , F(below 60).

## Solution :-
``` py
grdae = int(input("Enter Your grade :"))

if grdae >= 101 : 
    print("Please Verify your grade.")

exit()

if grdae >= 90 :
    grdae = "A"

elif grdae >= 80 :
    grdae = "B"

elif grdae >= 70 :
    grdae = "C"

elif grdae >= 60 :
    grdae = "D"

else : grdae = "F"

print("Your Grade is", grdae)
```





























































