![](img/python.png)
<!-- .element: style="margin-top: -5%;" -->
## Python 101

#### [Mario Garcia](http://mariog.xyz) · [@mariogmd](https://twitter.com/mariogmd)

---

## What is Python?

---

## Installing Python

```
python.org/downloads

```

***

### Ubuntu

```
sudo apt install python3

```

<!-- .element: class="fragment" -->

***

### Manjaro

```
sudo pacman -S python

```

<!-- .element: class="fragment" -->

---

## Interactive Shell

```
mattdark@ubuntu:~$ python3
Python 3.5.2+ (default, Sep 22 2016, 12:18:14)
[GCC 6.2.0 20160927] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>

```

<!-- .element: class="fragment" -->

***

```
>>> print("Hello world!")
Hello world!

```

---

![](img/ninja-ide.png)
<!-- .element: style="margin-top: -5%;" -->
## Ninja-IDE

***

### Download

```
ninja-ide.org/downloads

```

***

### Ubuntu

```
sudo apt install ninja-ide

```

<!-- .element: class="fragment" -->

***

### Manjaro

```
sudo pacman -S ninja-ide

```

<!-- .element: class="fragment" -->

---

## Basic Syntax

---

## Hello world!

```
# hello.py
print("Hello world!")

```

***

```
mattdark@ubuntu:~$ python hello.py
Hello world!

```

---

## variables

```
variable_name = value

```

***

## constants

```
my_constant = 12

```

---

## data types

***

### string

```
string = "Hello world!"

```

***

### integer

```
age = 28

```

***

### float

```
price = 7435.28

```

***

### boolean

```
bool = true
bool = false

```

---

## operators

```
a = 10 + 5 # Addition
a = 12 - 7 # Subtraction
a = 7 * 5 # Multiplication
a = 2 ** 3 # Exponent

```

***

```
a = 12.5 / 2 # Division
a = 12.5 / 2 # Floor division
a = 27 % 4 # Modulus

```

---

## comments

```
# This is a comment

```

***

```
""" This is a comment
    of two lines """

```

---

## decision making

```
# if statement
a = 5
if a == 10:
    print("Value of a is ", a)

```

***

```
# if ... else statement
a = 5
if a > 10:
    print("a is greater than 10")
else:
    print("a is less than 10")
```

***

```
# if ... elif statement
a = 5
if a > 10:
    print("a is greater than 10")
elif a == 10:
    print("a is equal to 10")

```

---

## comparison operators

```
if a == 12 # equal to
if a != 20 # not equal to
if a < 100 # less than

```

***

```
if a > 50 # greater than
if a >= 10 # greater than or equal to
if a <= 30 # less than or equal to

```

---

## logical operators

```
if a > 10 and a < 50 # and
if a > 10 or a > 15 # or

```

---

## loops

```
# while loop
n = 0
while n < 10:
    print(n)
    n = n + 1

```

***

```
# for loop
for i in range(10):
    print(n)

```

---

## lists

```
a = [1, 2, 3, 4, 5, 6, 7, 8, 9] # List
b = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] # 2D List

```

***

## print list content

```
a = [1, 2, 3, 4, 5, 6, 7, 8, 9]
print(a)

```

***

```
a = [1, 2, 3, 4, 5, 6, 7, 8, 9]
for i in range(9):
    print(a)

```

---

## functions

```
def function_name(parameters):
    # Statements

```

***

```
def sum(a, b):
    c = a + b
    print("The result of a + b is ", c)

a = 10
b = 5
sum(a, b)
```

---

## Examples

***

### Create a password

```
import random
c = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!-#$%&/()=?¿[]{}"
p = random.sample(c, 16)
pw = ""
for i in range(len(p)):
    pw += p[i]
print("Password:", pw)

```

***

### Order numbers

```
list = list()
for i in range(3):
    list.append(int(input("Introduce a number: ")))
list.sort(reverse = True)
print(list)

```

***

### Days between two dates

```
import datetime
h = datetime.date.today()
y = int(input("Introduce year (AAAA): "))
m = int(input("Introduce month (MM): "))
d = int(input("Introduce day (DD): "))
date = datetime.date(y, m, d)
days = h - date
print("Days passed: ", days.days)

```

---

## Learn More

_[python.org](https//python.org)_

___

[@mariogmd](https://twitter.com/mariogmd)

mattdark@mozilla-mexico.org
