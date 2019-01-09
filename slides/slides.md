![](assets/reveal.js/img/python.png)
<!-- .element: style="margin-top: -5%;" -->
## Python 101

#### [Mario Garcia](https://mattdark.github.io) · [@mariogmd](https://twitter.com/mariogmd)

---

## What is Python?

---

## Download Python

----

### Download from python.org

```
python.org/downloads

```

----

- Available for Windows, GNU/Linux, Mac
- Support for x86, x86-64 & ARM<!-- .element: class="fragment" -->
- Python 2.7.15 & Python 3.6.5<!-- .element: class="fragment" -->

----

### Install from repositories on GNU/Linux

----

### Ubuntu

```
sudo apt install python3

```

<!-- .element: class="fragment" -->

----

### Manjaro

```
sudo pacman -S python

```

<!-- .element: class="fragment" -->

---

## Python 2.7.x vs Python 3.6.x

- Syntax slightly different<!-- .element: class="fragment" -->
- Compatibility with libraries<!-- .element: class="fragment" -->

----

### Python 2.7.13

```
  print "Hello world!"
```

----

### Python 3.6.5

```
  print("Hello world!")
```

---

### Python 2.7.x countdown

- Support until January 1st, 2020

---

## Python 3.6

---

## Interactive Shell

```
[mattdark@manjaro ~]$ python
Python 3.6.1 (default, Mar 27 2017, 00:27:06)
[GCC 6.3.1 20170306] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>

```

<!-- .element: class="fragment" -->

----

```
>>> print("Hello world!")
Hello world!

```

---

## Text editors

- Atom<!-- .element: class="fragment" --> [atom.io](https://atom.io/)<!-- .element: class="fragment" -->
- Notepad++<!-- .element: class="fragment" --> [notepad-plus-plus.org](https://notepad-plus-plus.org/)<!-- .element: class="fragment" -->
- Sublime Text<!-- .element: class="fragment" --> [sublimetext.com](https://www.sublimetext.com/)<!-- .element: class="fragment" -->

---

## IDEs

- Ninja IDE<!-- .element: class="fragment" --> [ninja-ide.org](https://ninja-ide.org/)<!-- .element: class="fragment" -->
- Thonny<!-- .element: class="fragment" --> [thonny.org](https://thonny.org/)<!-- .element: class="fragment" -->

---

## Basic Syntax

---

## Printing text

```
  # hello.py
  print("Hello world!")

```

----

```
  mattdark@ubuntu:~$ python hello.py
  Hello world!

```

---

## variables

```
  variable_name = value

```

---

## data types

```
  str = "This is a string" # string
  age = 28 # integer
  price = 7435.28 # float
  bool = True # boolean
  bool = False
```

---

## operators

```
  a = 10 + 5 # Addition
  a = 12 - 7 # Subtraction
  a = 7 * 5 # Multiplication
  a = 2 ** 3 # Exponent

```

----

```
  a = 12.5 / 2 # Division
  a = 12.5 // 2 # Floor division
  a = 27 % 4 # Modulus

```

---

## comments

```
  # This is a comment

```

----

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

----

```
  # if ... else statement
  a = 5
  if a > 10:
      print("a is greater than 10")
  else:
      print("a is less than 10")
```

----

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

----

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

----

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

----

## print list content

```
  a = [1, 2, 3, 4, 5, 6, 7, 8, 9]
  print(a)

```

----

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

----

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

----

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

----

### Order numbers

```
list = list()
for i in range(3):
    list.append(int(input("Introduce a number: ")))
list.sort(reverse = True)
print(list)

```

----

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
[iscmariog](https://facebook.com/iscmariog)

mattdark@mozilla-mexico.org
