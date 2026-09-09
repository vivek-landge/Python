# Dictionaries

- Dictionaries are similar to the sql schemas
- Everything in dictionaries are stored in (key : value) pair
- Syntax:

```python
>>> chai = {"Masala" : "Spicy","Ginger" : "Zesty","Green":"Mild"}
```

- Accessing Elements

```python
>>> chai["Masala"]
'Spicy'
>>> chai.get("Ginger")
'Zesty'
```

- Changing Values

```python
>>> chai
{'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Mild'}
>>> chai["Green"] = "Fresh"
>>> chai
{'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Fresh'}
```

- In Loop we get access of Keys

```python
>>> chai = {'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Fresh'}
>>> chai
{'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Fresh'}
>>> for tea in chai :
...     print(tea)
...
Masala
Ginger
Green
>>> for tea in chai :
...     print(tea, chai.get(tea))
...
Masala Spicy
Ginger Zesty
Green Fresh
```

- Accesing Keys and Values simultaneously

```python
>>> for keys,values in chai.items():
...     print(keys,values)
...
Masala Spicy
Ginger Zesty
Green Fresh
```

- Adding Items

```python
>>> chai["Mint"] = "Minty"
>>> chai
{'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Fresh', 'Mint': 'Minty'}
```

- Removing Items

```python
>>> chai
{'Masala': 'Spicy', 'Ginger': 'Zesty', 'Green': 'Fresh', 'Mint': 'Minty'}
>>> chai.pop("Ginger")
'Zesty'
>>> chai
{'Masala': 'Spicy', 'Green': 'Fresh', 'Mint': 'Minty'}
>>> chai.popitem()
('Mint', 'Minty')
>>> chai
{'Masala': 'Spicy', 'Green': 'Fresh'}
>>> del chai["Green"]
>>> chai
{'Masala': 'Spicy'}
>>> chai.clear()
>>> chai
{}
```

- Making copies (Reference Game)

```python
>>> chai_copy = chai.copy()
```

- Special syntax of writing dictionary

```python
>>> squared_nums = {x:x**2 for x in range(6)
... }
>>> squared_nums
{0: 0, 1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

# Tuple

- It is Immutable just like strings
- Nearly all the operations we learnt previously works similarly on tuples
- Syntax
```python
chai = ("Masala","Ginger","Green","Mint")
```
