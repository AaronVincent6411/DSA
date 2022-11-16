# Datatypes

### Built-in types

###### Booleans

- bool
A boolean value returns either ```True``` or ```False```. Logic operations like ```and``` or ```not``` can be performed on booleans.


```
x or y  # if x is False then y otherwise x

x and y # if x is False then x otherwise y

not x # if x is True then False otherwise True
```

If boolean values are used in arithmetic operations, the integer values will be used to return an integer result.

```
True + False == 1 # 1 + 0 == 1
True * True == 1 # 1 + 1 == 2
```

###### Numbers

- int

int means integer number. Integers in python are arbitrary sizes

```
a = 1
b = 200
```
- float

float refers to floating point numbers. Precision depends on the implementation and system architecture, for CPython the float datatype corresponds to a C double.

```
a = 1.0
b = 200.e0 # e refers to exponents
```
- complex

complex refers to Complex numbers

```
a = 1 + 2j
b = 200 + 1j
```

+ NB: The ```<, <=, >``` and ```=>``` operators will raise a ```TypeError``` excepetion when any operand is a complex number.

###### Strings

Strings in python varies depending python versions. 

- str 

In Python 3.x version str is a unicode string
In Python 2.x version str is a byte string

- bytes

In Python 3.x version bytes is a byte string
In Python 2.x version bytes is a synonym for str

- unicode

In Python 2.x version unicode is a unicode string

### Collection types

###### List

List type is most probably the most commonly used collection type in Python. Despite its name, a list is more like an array in other languages, mostly Javascript. In python a list is an ordered collection of valid python values. A list can be created by enclosing values, separated by commas, in square brackets.

```
list1 = [1,2,3]
list2 = ['I', 'am', 'Aaron']
```

A list can be also given empty and it can accept values of multiple datatypes. A list can also contain value of another list.

```
list3 = []
list4 = ['I', 'am', 24]
list5 = [['a', 'b', 'c'],[1, 2, 3]]
```
Elements in a list can be accessed via index

```
>>> list6 = [1, 2, 3]
>>> print(list6[1])
2
>>> print(list6[0])
1
```
Indices can also be negative which means counting from the end of the list.

```
>>> list7 = [10, 20, 30]
>>> print(list7[-1])
30
>>> print(list7[-2])
20
```

Lists are mutable. So values can be changed

```
>>> list8 = [2,2,3,4,5]
>>> list8[0] = 1
>>> print(list8)
[1, 2, 3, 4, 5]
```
###### Tuples

A tuple is a similar to a list except that it fixed-length and immutable. So the values in the tuple cannot be changed nor the values be added to or removed from the tuple.

```
tuple1 = (1,2,3)
tuple2 = ('hello', 'I', 'am', 'Aaron')
```

###### Dictionaries

a dictionary in a python is a collection of key-value pair. The dictionary is surrounded by curly braces. Each pair is separated by comma and the key and value are separated by a colon.

```
dict1 = {
    'SIno' : 1,
    'Name' : 'Aaron',
    'githubname' : 'Aaron Vincent 6411',
}
```
To get key

```
>>> print(dict1)
{'SIno': 1, 'Name': 'Aaron', 'githubname': 'Aaron Vincent 6411'}
>>> for key in dict1:
...     print(key)
... 
SIno
Name
githubname
```

```
>>> for key in dict1:
...     print(dict1[key])
... 
1
Aaron
Aaron Vincent 6411
```

```
>>> for key,values in dict1.items():
...     print(key, values)
... 
SIno 1
Name Aaron
githubname Aaron Vincent 6411
```

###### Set

A set is a collection of elements with no repeat and without insertion order but sorted order. They are used in situations where it is only important that some things are grouped together and not what order they were included.

```
set1 = {1,2,3}
set2 = set([1,2,3])
```
###### Next
[Modules and Functions](./6Modules%20and%20Functions.md)

###### Previous
[Block Indentation](./4Block%20Indentation.md)