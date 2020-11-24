# examples
## hello python


```python
# hello python
print("Hello Python!")
```

    Hello Python!


## if statement


```python
# conditional 
# if statement

x = 100
y = 55
if x > y:
    print("X is greater than Y.")
```

    X is greater than Y.


## if-else 


```python
# if-else
num = int(input("Enter 1:"))
if num == 1:
    print("The number is 1")
else:
    print("You entered something else!")
```

    Enter 1: 1


    The number is 1


## more if-else


```python
# if-else

number = int(input("Enter any number: "))
if number <= 50:
    print("Number is less than or equal to 50!")
else:
    print("Number is greater than 50!")
```

    Enter any number:  100


    Number is greater than 50!


## again if-else


```python
# if-else

check_human = input("Are you a human? (y/n): ")
if check_human == 'y' or check_human == 'Y':
    print("Welcome to earth, human!")
else:
    print("Alien detected!")
```

    Are you a human? (y/n):  y


    Welcome to earth, human!


## much more if-else


```python
# if-else

age = int(input("Enter your age: "))
if age >= 18 and age <= 120:
    print("You are eligible for voting!")
else:
    print("You are not eligible for voting!")
```

    Enter your age:  22


    You are eligible for voting!


## if-elif-else


```python
# if-elif-else

marks = int(input("Enter your marks: "))
if marks < 35:
    print("Grade 'F': Fail")
elif marks >= 35 and marks <= 40:
    print("Grade 'D'")
elif marks >= 41 and marks < 50:
    print("Grade 'C'")
elif marks >= 50 and marks < 60:
    print("Grade 'B'")
elif marks >= 60 and marks < 70:
    print("Grade 'B+'")
elif marks >= 70 and marks < 80:
    print("Grade 'A'")
else:
    print("Grade 'A+'")
```

    Enter your marks:  75


    Grade 'A'


## nested if


```python
# nested if

numb = int(input("Enter a number: "))
if numb > 20:
    print("The number is greater than 20!")
    if numb % 2 == 0:
        print("The number is also even!")
    else:
        print("The number is also odd!")
else:
    print("The number is less than 20!")
```

    Enter a number:  21


    The number is greater than 20!
    The number is also odd!


## switch-case 


```python
# switch-case using dictionary 

num2wordbeng = {
    1:'Ek',
    2:'Dui',
    3:'Tin',
    4:'Char',
    5:'Panch',
    6:'Chhoy',
    7:'Saat',
    8:'Aatt',
    9:'Noy',
    10:'Dash',
}

usrinp = int(input("Enter a case number: "))
print('Tomar prodotto input: ',num2wordbeng.get(usrinp, 'Invalid Input'))
```

    Enter a case number:  5


    Tomar prodotto input:  Panch


## using for loop to access elements


```python
# for loop-accessing elements

lang =[
    'python',
    'c++',
    'c',
    'java',
    'c#',
    'assembly',
    'vb.net',
    'php',
    'javascript',
]

for prog in lang:
    print(prog, end="| ")
```

    python| c++| c| java| c#| assembly| vb.net| php| javascript| 

## using for loop to access characters in a string


```python
# for loop-accessing chars in string

for char in 'python-programming':
    print(char,end="| ")
```

    p| y| t| h| o| n| -| p| r| o| g| r| a| m| m| i| n| g| 

## using for loop to print square of numbers


```python
# for loop-print square of numbers

for number in range(1, 11):
    print("Square of: ", number, " is ", number*number)
```

    Square of:  1  is  1
    Square of:  2  is  4
    Square of:  3  is  9
    Square of:  4  is  16
    Square of:  5  is  25
    Square of:  6  is  36
    Square of:  7  is  49
    Square of:  8  is  64
    Square of:  9  is  81
    Square of:  10  is  100


## using for loop to print even numbers


```python
# for loop-print even numbers

print("Even numbers between 1 to 25!")
for num in range(1, 26):
    if num % 2 == 0:
        print(num, end="| ")
```

    Even numbers between 1 to 25!
    2| 4| 6| 8| 10| 12| 14| 16| 18| 20| 22| 24| 

## using for loop to print multiplication table


```python
# for loop-print multiplication table

thenum = int(input("Enter a number: "))
for x in range(1, 11):
    print(thenum*x)
```

    Enter a number:  19


    19
    38
    57
    76
    95
    114
    133
    152
    171
    190


## use else with for


```python
# for-else 

for x in range(5):
    print(x)
else:
    print("End of loop!")
```

    0
    1
    2
    3
    4
    End of loop!


## using range function 1


```python
# range function 1

for y in range(5):
    print(y)
```

    0
    1
    2
    3
    4


## using range function 2


```python
# range function 2

for z in range(2, 10):
    print(z)
```

    2
    3
    4
    5
    6
    7
    8
    9


## using range function 3


```python
# range function 3

for odd in range(1, 10, 2):
    print(odd)
```

    1
    3
    5
    7
    9


## using range function 4


```python
# range function 4

for even in range(10, 1, -2):
    print(even)
```

    10
    8
    6
    4
    2


## while loop begins


```python
# while loop

b = 0
while b != 1:
    print("You are inside the while loop.")
    print("Enter 1 to exit from the loop.")
    b = int(input())
print("You are out of the loop.")
```

    You are inside the while loop.
    Enter 1 to exit from the loop.


     2


    You are inside the while loop.
    Enter 1 to exit from the loop.


     1


    You are out of the loop.


## more while loop


```python
# while loop

c = 1
while c <= 5:
    print(c)
    c += 1
```

    1
    2
    3
    4
    5


## much more while loop


```python
# while loop (square of numbers)

d = 1
while d != 0:
    d = int(input("Enter a number: "))
    print("Square of ", d, " is ", d*d)
    
print("End of program")
```

    Enter a number:  2


    Square of  2  is  4


    Enter a number:  5


    Square of  5  is  25


    Enter a number:  0


    Square of  0  is  0
    End of program


## use else with while


```python
# while-else 

e = 1
while e < 5:
    print(e, "is less than 5.")
    e += 1
else:
    print("End of program.")
```

    1 is less than 5.
    2 is less than 5.
    3 is less than 5.
    4 is less than 5.
    End of program.


## nested loop


```python
# nested loop

for x in range(1, 11):
    for y in range(1, 11):
        print("{:03d}".format(x*y), end=" ")
    print()
```

    001 002 003 004 005 006 007 008 009 010 
    002 004 006 008 010 012 014 016 018 020 
    003 006 009 012 015 018 021 024 027 030 
    004 008 012 016 020 024 028 032 036 040 
    005 010 015 020 025 030 035 040 045 050 
    006 012 018 024 030 036 042 048 054 060 
    007 014 021 028 035 042 049 056 063 070 
    008 016 024 032 040 048 056 064 072 080 
    009 018 027 036 045 054 063 072 081 090 
    010 020 030 040 050 060 070 080 090 100 


## break the loop


```python
# break

for digit in range(10):
    if digit >= 5:
        break
    print(digit, end="| ")
```

    0| 1| 2| 3| 4| 

## continue the loop


```python
# continue

for digit in range(6):
    if digit == 3:
        # skip 3
        continue
    print(digit)
```

    0
    1
    2
    4
    5


## break & continue 


```python
# break - continue 

while True:
    print("Enter a number between (1 to 100)")
    print("Press 0 to exit")
    num = int(input())
    if num == 0:
        print("End of program. Thank you!")
        break
    elif num > 100:
        print("Number is greater than 100")
        continue
    print("Square of ", num, " is ", num*num)

```

    Enter a number between (1 to 100)
    Press 0 to exit


     2


    Square of  2  is  4
    Enter a number between (1 to 100)
    Press 0 to exit


     3


    Square of  3  is  9
    Enter a number between (1 to 100)
    Press 0 to exit


     0


    End of program. Thank you!


## pass it


```python
# Empty loop
for x in range(5):
    pass

# Empty function
def func():
    pass

# Empty class
class NewClass:
    pass
```

# more examples

## even/odd? 


```python
# number is even or odd

number = int(input("Enter a number: "))
if number % 2 == 0:
    print(f"{number} is even")
else:
    print(f"{number} is odd")
```

    Enter a number:  5


    5 is odd


## n!=? (factorial)


```python
# factorial using recursion

def factorial(num):
    if num < 0:
        return "Invalid input!"
    elif num == 0:
        return 1
    # base_case
    elif num == 1:
        return num
    else:
        return num * factorial(num - 1)
    
number = int(input("Enter a number: "))
print(f"Factorial of {number}: ", factorial(number))
```

    Enter a number:  5


    Factorial of 5:  120


## is prime number? 


```python
# prime numbers 
# naive algorithm 

number = int(input("Enter any number: "))
if number > 1:
    for x in range(2, number):
        if number % x == 0:
            print(number, " is not a prime number!")
            break
    else:
        print(number, " is a prime number!")
else:
    print(number, " is not a prime number!")
```

    Enter any number:  3


    3  is a prime number!


## find the largest among n digits!


```python
# Largest among n digits

ncollection = list()
num = int(input("Enter number of elements: "))
for i in range(1, num+1):
    usrinp = int(input(f"Enter element {i}: "))
    ncollection.append(usrinp)
ncollection.sort()
print("Largest number: ", ncollection[-1])
```

    Enter number of elements:  5
    Enter element 1:  23
    Enter element 2:  45
    Enter element 3:  65
    Enter element 4:  100
    Enter element 5:  2


    Largest number:  100


## swap 'em


```python
# swap two numbers without using third variable

num1 = 25
num2 = 52

print("num1: ", num1)
print("num2: ", num2)
print()
(num1, num2) = (num2, num1)

print("num1: ", num1)
print("num2: ", num2)
```

    num1:  25
    num2:  52
    
    num1:  52
    num2:  25


## swap 'em again


```python
# swap two numbers 
# another method
# without using third variable 

num1 = 25
num2 = 52

print("num1: ", num1)
print("num2: ", num2)
print()

num1 = num1 + num2 # 77
num2 = num1 - num2 # 77 - 52 = 25
num1 = num1 - num2 # 77 - 25 = 52

print("num1: ", num1)
print("num2: ", num2)
```

    num1:  25
    num2:  52
    
    num1:  52
    num2:  25


## swap 'em with third variable


```python
# swap two numbers 
# using a third temporary variable

num1 = 25
num2 = 52

print("num1: ", num1)
print("num2: ", num2)
print()

temp = num1
num1 = num2
num2 = temp

print("num1: ", num1)
print("num2: ", num2)
```

    num1:  25
    num2:  52
    
    num1:  52
    num2:  25


## fibonacci sequence!


```python
# Fibonacci sequence 
# using recursion
# limited - without memoization

def fibonacci(num):
    # base_case
    if num <= 1:
        return num
    else:
        return fibonacci(num-1) + fibonacci(num-2)
    
# 0, 1, 1, 2, 3, 5, 8
number_of_terms = 10
print("Fibonacci Sequence")
for x in range(number_of_terms):
    print(fibonacci(x))
```

    Fibonacci Sequence
    0
    1
    1
    2
    3
    5
    8
    13
    21
    34


## palindrome?


```python
# check palindrome - string

string = input("Enter a word: ")
string = string.casefold()
reverse_string = reversed(string)

if list(string) == list(reverse_string):
    print("the word is a palindrome")
else:
    print("the word is not a palindrome")
```

    Enter a word:  abir


    the word is not a palindrome


## palindrome number? 


```python
# check palindrome - number

number = int(input("Enter a number: "))
temporary = number
reverse = 0

while temporary > 0:
    remainder = temporary % 10
    reverse = reverse*10 + remainder
    temporary = temporary // 10
    
if reverse == number:
    print("The number is a palindrome!")
else:
    print("The number is not a palindrome!")

```

    Enter a number:  155


    The number is not a palindrome!
