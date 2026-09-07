# Internals

- Garbage collection does not happen immediately
- We can't the correct reference count(not of variables created/memory references)
- When reference is changed
```python

>>> myListOne = [1,2,3]
>>> myListTwo = myListOne          
>>> myListTwo = "Bankai" 
>>> myListTwo
'Bankai'
>>> myListOne
[1, 2, 3]
>>> myListTwo = [1,2,3]
>>> myListTwo[0] = 44
>>> myListTwo
[44, 2, 3]
>>> myListOne
[1, 2, 3]
```

- When the reference is not changed
``` python
>>> l1 = [1,2,3]
>>> l2 = l1
>>> l1
[1, 2, 3]
>>> l2
[1, 2, 3]
>>> l1[0] = 44
>>> l1
[44, 2, 3]
>>> l2
[44, 2, 3]
```
- Lists are mutable
```python
>>> p1 = [1,2,3]
>>> p2 = p1
>>> p1
[1, 2, 3]
>>> p2
[1, 2, 3]
>>> p2 = [1,2,3]   
>>> p1
[1, 2, 3]
>>> p2
[1, 2, 3]
>>> p1[0] = 66
>>> p1
[66, 2, 3]
>>> p2
[1, 2, 3]
```

- Making copy
```python

>>> h1 = [1,2,3] 
>>> h2 = h1[:]
>>> h1
[1, 2, 3]
>>> h2
[1, 2, 3]
>>> h1[0] = 33
>>> h1
[33, 2, 3]
>>> h2
[1, 2, 3]
```

- == operator checks the value 

``` python
>>> m = [1,2,3]
>>> n = m
>>> m
[1, 2, 3]
>>> n
[1, 2, 3]
>>> m == n
True
>>> m is n
True
```
- but is checks the reference
``` python
>>> m = [1,2,3]
>>> n = m
>>> m
[1, 2, 3]
>>> n
[1, 2, 3]
>>> m == n
True
>>> m is n
True
>>> m = [1,2,3]
>>> m == n
True
>>> m is n
False
```
