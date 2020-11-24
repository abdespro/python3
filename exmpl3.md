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
