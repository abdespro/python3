### python abs() function

* returns the absolute value of a number


```python
x = abs(-2.31)
y = abs(6.2+3.1j)

print("x={} and y={:.2f}".format(x,y))
```

    x=2.31 and y=6.93


### python all() function

* returns True if all elements of the iterable are true (or if the iterable is empty)


```python
collection_of_bools_one = [True, True, True]
print(all(collection_of_bools_one))
```

    True



```python
collection_of_bools_two = [True, True, False]
print(all(collection_of_bools_two))
```

    False



```python
list_of_numbers_one = [2,3,4,5,-7,-6]
print(all(list_of_numbers_one))
```

    True



```python
list_of_numbers_two = [2,3,4,5,-7,-6,0]
print(all(list_of_numbers_two))
```

    False



```python
# check whether all the numbers in a list are even

numbers_list_one = [2,4,6,8,10]
numbers_list_two = [2,3,4,6,8,10]

print("every number in list_one is even: ", all(map(lambda x:True if x%2 == 0 else False, numbers_list_one)))
print("every number in list_two is even: ", all(map(lambda x:True if x%2 == 0 else False, numbers_list_two)))
```

    every number in list_one is even:  True
    every number in list_two is even:  False


### python any() function

* returns True if any element of the iterable is true. If the iterable is empty, returns False.


```python
zero_zero_one = [0,0,1]
print(any(zero_zero_one))
```

    True



```python
zero_zero_zero = [0] * 3
print(any(zero_zero_zero))
```

    False



```python
# check whether any one number in a list is odd

numbers_list_one = [2,4,6,8,10]
numbers_list_two = [2,3,4,6,8,10]

print("at least one number in list_one is odd: ", any(map(lambda x:True if x%2 != 0 else False, numbers_list_one)))
print("at least one number in list_two is odd: ", any(map(lambda x:True if x%2 != 0 else False, numbers_list_two)))
```

    at least one number in list_one is odd:  False
    at least one number in list_two is odd:  True


### python ascii() function

* the ascii() function returns a readable version of any object (Strings, Tuples, Lists, etc).

* the ascii() function will replace any non-ascii characters with escape characters.


```python
string = ascii("My name is åbir")
print(string)
```

    'My name is \xe5bir'


### python bin() function

* convert an integer number to a binary string prefixed with “0b”


```python
for decimal in range(2, 6):
    print(bin(decimal))
```

    0b10
    0b11
    0b100
    0b101



```python
# evil-odious number
# 3 - evil number
# binary(3) = 11
# two 1s => even
# 16 - odious number
# binary(16) = 10000
# one 1 => odd

def is_evil(decimal):
    count_one = 0
    for element in list(bin(decimal))[2:]:
        if element == '1':
            count_one = count_one + 1
    
    return count_one % 2 == 0

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
