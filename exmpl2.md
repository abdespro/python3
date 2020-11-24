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
