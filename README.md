visit <a href="https://abdespro.github.io/python3/built_in_functions_one.html" target="_blank">built_in_functions</a>
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


# much more examples
## construct pascal triangle


```python
# pascal triangle 
# using factorial & combination 

def factorial(number):
    if number == 0:
        return 1
    # base_case
    elif number == 1:
        return number
    else:
        return number * factorial(number - 1)
    
def combination(n, r):
    return ((factorial(n)) // (factorial(r) * factorial(n - r)))

def pascal(rows):
    for numrow in range(0, rows+1):
        for r in range(0, numrow+1):
           print(combination(numrow, r), end=" ")
        print()

NumRows = int(input("Enter the number of rows: "))


pascal(NumRows)
```

    Enter the number of rows:  6


    1 
    1 1 
    1 2 1 
    1 3 3 1 
    1 4 6 4 1 
    1 5 10 10 5 1 
    1 6 15 20 15 6 1 


## leap year?


```python
# Leap year

def is_leap_year(year):
    if year % 4 == 0 and year % 100 != 0:
        return True
    elif year % 100 == 0 and year % 400 == 0:
        return True
    else:
        return False
    
print(is_leap_year(int(input("Enter a year: "))))
```

    Enter a year:  1600


    True


## perfect number?


```python
# perfect number
# sum of factors (except the number itself) = number

def is_perfect(number):
    sum_of_divisors = 0
    for divisor in range(1, number):
        if number % divisor == 0:
            sum_of_divisors += divisor
    if sum_of_divisors == number:
        return True
    return False

for number in range(1, 10000):
    if is_perfect(number):
        print(number, " is perfect")
```

    6  is perfect
    28  is perfect
    496  is perfect
    8128  is perfect


## what about armstrong number? 


```python
# armstrong number
# cube of digits = number

def is_armstrong(number):
    num_list = list(number)
    sum_of_digits = 0
    for element in num_list:
        sum_of_digits += int(element) * int(element) * int(element)
    
    if int(number) == sum_of_digits:
        return True
    return False

for number in range(1, 1000000):
    if is_armstrong(str(number)):
        print(number, " is an armstrong!")
```

    1  is an armstrong!
    153  is an armstrong!
    370  is an armstrong!
    371  is an armstrong!
    407  is an armstrong!


## bam! strong number


```python
# strong number
# 145 = 1! + 4! + 5!

def factorial(number):
    if number == 0:
        return 1
    # base_case
    elif number == 1:
        return number
    else:
        return number * factorial(number - 1)
    
def is_strong(number):
    num_list = list(number)
    sum_of_factorial_of_digits = 0
    for element in num_list:
        sum_of_factorial_of_digits += factorial(int(element))
    if sum_of_factorial_of_digits == int(number):
        return True
    return False

for number in range(1, 1000000):
    if is_strong(str(number)):
        print(number, " is strong!")
```

    1  is strong!
    2  is strong!
    145  is strong!
    40585  is strong!


## automorphic number!


```python
# automorphic number
# 25*25 = 6(25)

def is_automorphic(number):
    square = number * number
    temporary = number
    while temporary > 0:
        if temporary % 10 == square % 10:
            temporary = temporary// 10
            square = square//10
        else:
            return False
    return True

for number in range(1, 1000):
    if is_automorphic(number):
        print(number, " is automorphic!")
```

    1  is automorphic!
    5  is automorphic!
    6  is automorphic!
    25  is automorphic!
    76  is automorphic!
    376  is automorphic!
    625  is automorphic!


## spy number! (sum == mul)


```python
# spy number
# 1412
# sum = 1 + 4 + 1 + 2 = 8
# mul = 1 * 4 * 1 * 2 = 8

def is_spy_number(number):
    sum_of_digits = 0
    mul_of_digits = 1
    temporary = number
    while temporary > 0:
        sum_of_digits += temporary % 10
        mul_of_digits *= temporary % 10
        temporary = temporary // 10
        
    if sum_of_digits == mul_of_digits:
        return True
    return False

for number in range(2000, 10000):
    if is_spy_number(number):
        print(number, " is spy number!")
```

    2114  is spy number!
    2141  is spy number!
    2411  is spy number!
    4112  is spy number!
    4121  is spy number!
    4211  is spy number!


## happy numbers :D


```python
# happy numbers
# 19
# 1^2 + 9^2 = 82
# 8^2 + 2^2 = 68
# 6^2 + 8^2 = 100
# 1^2 + 0^2 + 0^2 = 1

def is_happy_number(number):
    # base_case for unhappy numbers
    if number==4:
        return False
    # base_case for happy numbers
    if number <= 1:
        return True
    sum_of_sq_of_digits = 0
    while number > 0:
        sum_of_sq_of_digits += (number % 10)**2
        number = number // 10
    return is_happy_number(sum_of_sq_of_digits)

for number in range(1, 10):
    if is_happy_number(number):
        print(number, " is happy!")
    else:
        print(number, " is unhappy!")
```

    1  is happy!
    2  is unhappy!
    3  is unhappy!
    4  is unhappy!
    5  is unhappy!
    6  is unhappy!
    7  is happy!
    8  is unhappy!
    9  is unhappy!

## sunny numbers


```python
# sunny numbers
# N = 8
# N + 1 = 9 (perfect square)

from math import sqrt

def is_sunny(number):
    sqrt_of_num_plus_one = sqrt(number + 1)
    if int(sqrt_of_num_plus_one) == sqrt_of_num_plus_one:
        return True
    return False

for number in range(1, 101):
    if is_sunny(number):
        print(number, " is a sunny number")
```

    3  is a sunny number
    8  is a sunny number
    15  is a sunny number
    24  is a sunny number
    35  is a sunny number
    48  is a sunny number
    63  is a sunny number
    80  is a sunny number
    99  is a sunny number


## fascinating number


```python
# fascinating number 
# 192
# 192 * 2 = 384
# 192 * 3 = 576
# 192 384 576
# 123456789
# fascinating, isn't it?

def is_fascinating(number):
    if number < 100:
        return False
    one_to_nine = '123456789'
    number_mul_two = number * 2
    number_mul_three = number * 3
    concat_num_num2_num3 = "".join(sorted(list(str(number) + str(number_mul_two) +  str(number_mul_three))))
    if concat_num_num2_num3 == one_to_nine:
        return True
    return False
    

for number in range(100, 1001):
    if is_fascinating(number):
        print(number, " is fascinating!")
```

    192  is fascinating!
    219  is fascinating!
    273  is fascinating!
    327  is fascinating!


## disarium number


```python
# disarium number

def is_disarium(number):
    temporary = number
    sum_of_powered_digits = 0
    power = len(str(number))
    while temporary > 0:
        sum_of_powered_digits += (temporary % 10) ** power
        temporary = temporary // 10
        power = power - 1
        
    if sum_of_powered_digits == number:
        return True
    return False

for number in range(80,1001):
    if is_disarium(number):
        print(number, " is disarium!")
```

    89  is disarium!
    135  is disarium!
    175  is disarium!
    518  is disarium!
    598  is disarium!


## pronic number


```python
# pronic number
# 42
# 6 * 7 => n(n+1) => 42

def is_pronic(number):
    for n in range(number + 1):
        if n * (n + 1) == number:
            return True
    return False

for number in range(0, 101):
    if is_pronic(number):
        print(number, " is pronic!")
```

    0  is pronic!
    2  is pronic!
    6  is pronic!
    12  is pronic!
    20  is pronic!
    30  is pronic!
    42  is pronic!
    56  is pronic!
    72  is pronic!
    90  is pronic!


## trimorphic number


```python
# trimorphic number
# 5
# 5 * 5 * 5 = 12(5)

def is_trimorphic(number):
    cube_of_number = number ** 3
    temporary = number
    while temporary > 0:
        if cube_of_number % 10 == temporary % 10:
            cube_of_number = cube_of_number // 10
            temporary = temporary // 10
            continue
        else:
            return False
    return True

for number in range(1, 50):
    if is_trimorphic(number):
        print(number, " is trimorphic!")
```

    1  is trimorphic!
    4  is trimorphic!
    5  is trimorphic!
    6  is trimorphic!
    9  is trimorphic!
    24  is trimorphic!
    25  is trimorphic!
    49  is trimorphic!


## evil-odious number


```python
# evil number
# odious number
# 3 - evil number
# binary(3) = 11
# two 1s => even
# 16 - odious number
# binary(16) = 10000
# one 1 => odd

def binary(decimal):
    bin_out = list()
    while decimal > 0:
        bin_out.append(decimal%2)
        decimal = decimal // 2
    return bin_out

def is_evil(number):
    count_one = 0
    for element in binary(number):
        if element == 1:
            count_one += 1
    if count_one % 2 == 0:
        return True
    return False

for number in range(1, 11):
    if is_evil(number):
        print(number, " is evil!")
    else:
        print(number, " is odious!")
```

    1  is odious!
    2  is odious!
    3  is evil!
    4  is odious!
    5  is evil!
    6  is evil!
    7  is odious!
    8  is odious!
    9  is evil!
    10  is evil!

## floyd triangle


```python
# floyd triangle
#  1
#  2  3
#  4  5  6
#  7  8  9  10
#  11 12 13 14 15

def floyd(number_of_lines):
    element = 1
    for line in range(0, number_of_lines+1):
        for num_of_element in range(0, line):
            print(element,end=" ")
            element = element + 1
        print()
        
floyd(5)    
```

    
    1 
    2 3 
    4 5 6 
    7 8 9 10 
    11 12 13 14 15 


## reverse the number


```python
# reverse the number

def reverse(number):
    reversed_number = 0
    while number > 0:
        remainder = number % 10
        reversed_number = reversed_number * 10 + remainder
        number = number // 10
    return reversed_number

number = int(input("Enter a number: "))
print("reverse of ", number, ": ", reverse(number))
```

    Enter a number:  1458


    reverse of  1458 :  8541



```python
# previous one will not work 
# for some number like 1240
# reverse(1240) => 421

def true_reverse(number):
    list_reversed = list()
    while number > 0:
        list_reversed.append(str(number % 10))
        number = number // 10
    return "".join(list_reversed)

for number in range(100, 111):
    print(f"reverse of {number}: {true_reverse(number)}")
```

    reverse of 100: 001
    reverse of 101: 101
    reverse of 102: 201
    reverse of 103: 301
    reverse of 104: 401
    reverse of 105: 501
    reverse of 106: 601
    reverse of 107: 701
    reverse of 108: 801
    reverse of 109: 901
    reverse of 110: 011


## sum of digits


```python
# sum of digits

def sum_of_digits(number):
    sumofd = 0
    while number > 0:
        sumofd = sumofd + (number % 10)
        number = number // 10
    return sumofd

for number in range(123, 130):
    print(f"sum of digits of {number}: {sum_of_digits(number)}")
```

    sum of digits of 123: 6
    sum of digits of 124: 7
    sum of digits of 125: 8
    sum of digits of 126: 9
    sum of digits of 127: 10
    sum of digits of 128: 11
    sum of digits of 129: 12


## manual exponent


```python
# manual to the power operation

def powerof(number, exponent):
    result = 1
    for e in range(exponent):
        result = result*number
    return result

for number in range(2, 4):
    for power in range(1, 4):
        print(f"pow({number},{power}) = {powerof(number, power)}")
    print()
```

    pow(2,1) = 2
    pow(2,2) = 4
    pow(2,3) = 8
    
    pow(3,1) = 3
    pow(3,2) = 9
    pow(3,3) = 27
    


## count the number of digits


```python
# number of digits

def count_digits(number):
    count = 0
    while number > 0:
        count = count + 1
        number = number // 10
    return count

for number in range(95, 106, 3):
    print(f"number of digits in {number}: {count_digits(number)}")
```

    number of digits in 95: 2
    number of digits in 98: 2
    number of digits in 101: 3
    number of digits in 104: 3


## check anagram


```python
# check anagram
# listen <> silent
def CheckAnagram(string1, string2):
    for letter in string1:
        if not letter in string2:
            return False
    return True

print("'listen' is anagram of 'silent': ", CheckAnagram('listen', 'silent'))
```

    'listen' is anagram of 'silent':  True


## super digit


```python
# super digit
# super_digit(1234) => (1+2+3+4) = 10 => (1+0) = 1

def superdigitof(number):
    # base_case
    if number % 10 == number:
        return number
    sum_of_digits = 0
    while number > 0:
        sum_of_digits = sum_of_digits + (number % 10)
        number = number // 10
    return superdigitof(sum_of_digits)

print("super digit of 124587: ", superdigitof(124587))
print("super digit of 9875: ",superdigitof(9875))
```

    super digit of 124587:  9
    super digit of 9875:  2
