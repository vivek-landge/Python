# List

- We can say Lists are arrays in python.List shows similar properties and methods as that of arrays in other language
- Lists are Mutable.
- Python does not have arrays 
- We can use dicing,splicing and slicing operations on List
- We can also use above methods to replace , remove or add elments in the list
```python
>>> chai
['Masala', 'Lemon', 'Ginger', 'Mint']
>>> chai[1:2] = "Green"
>>> chai
['Masala', 'G', 'r', 'e', 'e', 'n', 'Ginger', 'Mint']
# To print the element properly we have to give list as an equivalent to add
>>> chai[1:6] =["Green"]
>>> chai
['Masala', 'Green', 'Ginger', 'Mint']
```

- Conditional Statement
```python
>>> chai = ["Masala","Lemon","Ginger","Mint"]
>>> if "Ginger" in chai:
...     print("I have Ginger Tea")
... else:
...     print("I do not have Ginger Tea")
... 
I have Ginger Tea
```

- Loops 
```python
>>> for chai in chai:
...     print(chai)
... 
Masala
Green
Ginger
Mint
```

- Adding and Removing the elments in the list
```python
>>> chai = ['Masala', 'Lemon', 'Ginger', 'Mint']
>>> chai
['Masala', 'Lemon', 'Ginger', 'Mint']
>>> chai.append("Oolong")
>>> chai
['Masala', 'Lemon', 'Ginger', 'Mint', 'Oolong']
>>> chai.pop()
'Oolong'
>>> chai.remove("Ginger")
>>> chai
['Masala', 'Lemon', 'Mint']
>>> chai.insert(1,"Ginger")
>>> chai
['Masala', 'Ginger', 'Lemon', 'Mint']
```

- Changing the reference keeping the data same
```python
>>> # Method - 1
>>> chai = ['Masala', 'Ginger', 'Lemon', 'Mint']
>>> chai_copy = ['Masala', 'Ginger', 'Lemon', 'Mint']

>>> # Method - 2 
>>> Chai_Copy = chai.copy()
```

- List Comprehension
```python
>>> squared_nums = [x**2 for x in range(10)]
>>> squared_nums                            
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
>>> squared_nums = [x**2 for x in range(10)]
>>> cube_nums = [x**3 for x in range(10)]   
>>> cube_nums    
[0, 1, 8, 27, 64, 125, 216, 343, 512, 729]
```
