# Numbers

- In python Number is a group of different objects in python
- Number gives similar accuracy as that of doible in the cpp
- We can use all the different types of arithmetic operators
- repr

- str

- print

- We can use all the comparison operators in python and their results are always in boolean form (True/False)
- We use different libraries in python
  ex : math,random

```python
>>> import random
>>> random.random()
0.9750978682379833
>>> random.random()
0.07172882549290582
```

```python
>>> random.randint(1,100)
35
>>> random.randint(1,100)
29
```

```python
>>> Bankai = ["Tensa","Zangetsu","Digoren","Hiorimaru"]
>>> random.choice(Bankai)
'Hiorimaru'
>>> random.choice(Bankai)
'Zangetsu'
```

```python
>>> Bankai
['Tensa', 'Zangetsu', 'Digoren', 'Hiorimaru']
>>> random.shuffle(Bankai)
>>> Bankai
['Tensa', 'Zangetsu', 'Hiorimaru', 'Digoren']
>>> random.shuffle(Bankai)
>>> Bankai
['Hiorimaru', 'Digoren', 'Zangetsu', 'Tensa']
```

```python
>>> import math
>>> math.floor(3.5)
3
>>> math.floor(-3.2)
-4
```

- trunc() ==> give nearest whole no towards 0

```python
>>> math.trunc(3.4)
3
>>> math.trunc(-3.4)
-3
```

- Number precision is very high in python
- We can also work on Complex No using python
- Python shows errors when we use decimals

```python
>>> 0.1 + 0.1 + 0.1
0.30000000000000004
>>> (0.1 + 0.1 + 0.1) - 0.3
5.551115123125783e-17
```

To resolve this we use

```python
>>> from decimal import Decimal

>>> Decimal('0.1') + Decimal('0.1') + Decimal('0.1')
Decimal('0.3')
```

- We can also import Fractions
```python
>>> from fractions import Fraction
>>> Frac = Fraction(2,4)
>>> Frac
Fraction(1, 2)
```

- In Python, Set is also a part of Number
- We can also perform the basic set operation in python
- Empty set is denoted as set() and not as { }. {} ==>it is a dictionary
