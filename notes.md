**Matrix**<br>
A matrix is a 2 dimensional array, can be represented as a list of lists in python 3.<br>
this list of lists follows several rules so it can represent a matrix:<br>
all rows have the same amount of values, all columns have the same amount of values, all items are in the same data type, indexing starts at zero.<br>

Example:
```python:
my_matrix = [[0,1,2,3],[4,5,6,7]] #this is a matrix
```
**List Comprehension**<br>
List Comprehension is the method to concisely create lists.<br>
The syntax of list comprehension is:<br>
1.A Square Bracket containing an expression that describes the list.<br>
2.One or more For clause to explain its members.<br>
3.Then a zero or more if clauses depending on the complexity of the list.<br>

Example:
```python:
#Generate a list of even numbers from 0 to 100
my_list = [x for x in range(101) if x % 2 == 0]
#or
my_other_list = [x for x in range(0,101,2)]
```
**Tuples**<br>
A tuple is an immutable data type, that:<br>
- is immutable<br>
- allow different datatypes as items<br>
- is iterable<br>
- is nestable<br>

Tuples are declared with parenthesis, ()<br>
items are seperated with commas<br>
Tuples are indexable and slicable similar to lists, using square brackets. <br>
Tuples are also responsible for packing and unpacking variables for python 3<br>
Example:
```python:
my_tuple = (1, "apple", 2, "banana", 3.5)
a, b, c, d = my_tuple[0], my_tuple[1], my_tuple[2], my_tuple[3:] #unpacking using indexing and slicing  
for item in d: #since d was my_tuple sliced, it is still a tuple, therefore iterable
    print(item)
another tuple = a, b, c #packing
```

**Map & Filters** <br>
The map function applies a function to every item in an iterable data type.
the format is map(function_name, sequence)
The filter function filters out items from a data set that meets a certain condition.
the format is filter(bool_returning_function, sequence)
Example:
def add_1(n): #function
    return n + 1
def greater_than_10(n): #bool_returning_function
    return n > 10

a = range(1,100) #iterable sequence
b = list(map(add_1, a)) #create new sequence using map function
c = list(filter(greater_than_10, b)) #create new sequence using filter function

**Sets**<br>
A set is an unordered collection with no duplicate elements <br>
To define a non empty set use {}, and seperate items using commas<br>
To define an empty set, use set()<br>
Another alternative is to define a set using set comprehension, similar to list comprehension<br>
to check if an item is inside a set, use the in operator<br>
To add/remove items from a set, use the add() method and remove() method<br>
In addition one can use set operators for complex calculations.<br>
Example:
```python:
set_a = set() # empty set using set()
set_a.add(16) # add elements to set
set_a.add(17)
set_a.add(18)
set_a.add(19)
set_a.add(20)
set_b = {1, 2, 3, 5, 7, 11, 13, 17, 19} # non empty set using {}
set_c = {x for x in range(1, 11) if x % 2 == 1} #set comprehension
set_d = (set_a | set_c) & set_b # set operators
print(7 in set_d) #use membership operators to check if 7 is in the set, this prints True
```

**Disctionaries**<br>
Dictionary (Associative Array, map, symbol table) is a data type that stores a collection of (key, value) pairs, such that each possible key appears at most once in the collection.<br>
To create a dictionary, use {}, and use : to seperate key-value pairs, with the key on the left side of the :, and the value on the right side. to seperate different pairs, use commas.<br>
To index dictionaries, use the key as the index for the value.<br>
To add a newe pair to the disctionary, use the same format as indexing a pair<br>
To remove a pair from a disctionary, use the del keyword<br>
Example:
```python:
```
