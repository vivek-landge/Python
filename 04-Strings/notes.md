# Strings 

- Strings can be in '',"",""" """
- Strings are immutable
- It supports slicing and splicing of the string 
- There are different methods for strings
- Ex :

``` python
>>> chai = "Masala Chai"
>>> chai
'Masala Chai'
>>> chai.lower()
'masala chai'
>>> chai.upper()
'MASALA CHAI'
```

- There is also a method to replace something in the string
```python
>>> chai.replace("Masala" , "Lemon")
'Lemon Chai'
```

- Converting strings into list
``` python
>>> chai = "Lemon, Ginger, Masala, Mint"
>>> chai
'Lemon, Ginger, Masala, Mint'
>>> chai.split()
['Lemon,', 'Ginger,', 'Masala,', 'Mint']
>>> chai.split(", ") # passed the parameter on the basis of which the string is is seperated
['Lemon', 'Ginger', 'Masala', 'Mint']
```

- Converting list into strings
```python
>>> chai_variety = ["Masala","Lemon","Ginger","Oolong"]
>>> chai_variety
['Masala', 'Lemon', 'Ginger', 'Oolong']
>>> "".join(chai_variety)
'MasalaLemonGingerOolong'
>>> " ,".join(chai_variety)
'Masala ,Lemon ,Ginger ,Oolong'
```

- Searching for the starting index a string inside a given string
```python
>>> chai = "Masala Chai"
>>> chai.find("Chai")
7
>>> chai.find("chai")
-1
```

- Count of a string inside a string

``` python
>>> chai  = "Masala Chai Chai Chai Chai Chai"
>>> chai.count("Chai")
5
```

- Order Formatting in Strings
```python
>>> chai_type = "Masala"
>>> quantity = 4
>>> order = "I ordered {} cups of {} chai"
>>> order
'I ordered {} cups of {} chai'
>>> order.format(quantity ,chai_type)
'I ordered 4 cups of Masala chai'
```
