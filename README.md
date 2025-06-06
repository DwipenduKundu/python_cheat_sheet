# Strings
- Python string is a sequence of characters, and each character can be individually accessed using its index.

- You can create strings by enclosing text in both forms of quotes - single quotes or double quotes:
```python
variable_name = "String Data"
```
Example:
```python
str = "Dwip"
print("string is ", str)
```
### Indexing
- The position of every character placed in the string starts from the 0th position and step by step it ends at length-1 position.

```python
txt = "Hello, welcome to my world."
x = txt.index("welcome")
print(x)
```
Output:
```
7
```

### Slicing
- Slicing refers to obtaining a sub-string from the given string. The following code will include index 1, 2, 3, and 4 for the variable named var_name.

- Slicing of the string can be obtained by the following syntax:
```python
string_var[int_start_value:int_stop_value:int_step_value]
```
```python
var_name = "Dwipendu"
print(var_name[1:5])
```
Output:
```
wipe
```
- Here start and step value are considered 0 and 1 respectively if not mentioned by the programmer.

### isalnum() Method
- Returns True if all the characters in the string are alphanumeric, else False:
```python
string_variable = "Company12"
print(string_variable.isalnum())
```
Output:
```
True
```
### isalpha() Method
- Returns True if all the characters in the string are alphabets:
```python
string_variable = "Dwip"
print(string_variable.isalpha())
```
Output:
```
True
```
### isdecimal() Method
- Returns True if all the characters in the string are decimals:
```python
string_variable = "1234"
print(string_variable.isdecimal())
```
Output:
```
True
```
### isdigit() Method
- Returns True if all the characters in the string are digits:
```python
string_variable = "1234"
print(string_variable.isdigit())
```
Output:
```
True
```
### islower() Method
- Returns True if all characters in the string are lower case:
```python
string_variable = "dwip"
print(string_variable.islower())
```
Output:
```
True
```
### isspace() Method
- Returns True if all characters in the string are whitespaces:
```python
string_variable = " "
print(string_variable.isspace())
```
Output:
```
True
```
### isupper() Method
- Returns True if all characters in the string are upper case:
```python
string_variable = "DWIP"
print(string_variable.isupper())
```
Output:
```
True
```
### lower() Method
- Converts a string into lower case equivalent:
```python
string_variable = "DWIP"
print(string_variable.lower())
```
Output:
```
dwip
```
### upper() Method
- Converts a string into upper case equivalent:
```python
string_variable = "dwip"'
string_variable.upper()
```
output
```
DWIP
```
### strip() Method
- It removes leading and trailing spaces in the string:

```python
string_variable.strip()
```

```python
txt = "     Dwip     "
x = txt.strip()
print(x)
```
Output:
```
Dwip
```
```python
txt = "!!!Dwip!!!"
x = txt.strip()
print(x)
```
Output:
```
Dwip
```
## Python String Methods table Sheet

### String Basics

```python
s = "Hello World"
```

| Operation      | Example   | Result          |
| -------------- | --------- | --------------- |
| Length         | `len(s)`  | `11`            |
| Indexing       | `s[0]`    | `'H'`           |
| Slicing        | `s[0:5]`  | `'Hello'`       |
| Step slicing   | `s[::2]`  | `'HloWrd'`      |
| Reverse string | `s[::-1]` | `'dlroW olleH'` |


### Changing Case

| Method     | Example          | Result          |
| ---------- | ---------------- | --------------- |
| Lowercase  | `s.lower()`      | `'hello world'` |
| Uppercase  | `s.upper()`      | `'HELLO WORLD'` |
| Capitalize | `s.capitalize()` | `'Hello world'` |
| Title Case | `s.title()`      | `'Hello World'` |
| Swap Case  | `s.swapcase()`   | `'hELLO wORLD'` |


### Whitespace and Stripping

| Method         | Example            | Result |
| -------------- | ------------------ | ------ |
| Strip (ends)   | `'  hi  '.strip()` | `'hi'` |
| LStrip (left)  | `'  hi'.lstrip()`  | `'hi'` |
| RStrip (right) | `'hi  '.rstrip()`  | `'hi'` |


### Searching & Replacing

| Method     | Example               | Result          |
| ---------- | --------------------- | --------------- |
| Find       | `s.find("o")`         | `4`             |
| Index      | `s.index("o")`        | `4`             |
| Replace    | `s.replace("o", "0")` | `'Hell0 W0rld'` |
| Count      | `s.count("l")`        | `3`             |
| Startswith | `s.startswith("He")`  | `True`          |
| Endswith   | `s.endswith("ld")`    | `True`          |


### Splitting and Joining

| Method | Example                | Result               |
| ------ | ---------------------- | -------------------- |
| Split  | `s.split(" ")`         | `['Hello', 'World']` |
| Join   | `' '.join(['a', 'b'])` | `'a b'`              |


### Testing Strings

| Method          | Example              | Result |
| --------------- | -------------------- | ------ |
| Is alpha        | `'abc'.isalpha()`    | `True` |
| Is digit        | `'123'.isdigit()`    | `True` |
| Is alphanumeric | `'abc123'.isalnum()` | `True` |
| Is lowercase    | `'abc'.islower()`    | `True` |
| Is uppercase    | `'ABC'.isupper()`    | `True` |
| Is space        | `'   '.isspace()`    | `True` |


### Formatting Strings

| Method   | Example                | Result       |
| -------- | ---------------------- | ------------ |
| f-string | `f"Hi {name}"`         | `'Hi Alice'` |
| format() | `'Hi {}'.format(name)` | `'Hi Alice'` |

---
# Array
### List
- A list in Python represents a list of comma-separated values of any data type between square brackets:
```python
var_name = [element1, element2, ...]
```
- These elements can be of different data types.

#### Indexing
- The position of every element placed in the list starts from the 0th position and step by step it ends at length-1 position. List is ordered, indexed, mutable, and the most flexible and dynamic collection of elements in Python.
```python
fruits = ['apple', 'banana', 'cherry']
print(fruits.index("cherry"))
```
Output:
```
2
```
#### Empty List
- This method allows you to create an empty list:
```python
my_list = []
```

#### index() Method
- Returns the index of the first element with the specified value:
```python
list.index(element)
```
Example:
```python
fruits = ['apple', 'banana', 'cherry']
print(fruits.index("cherry"))
```
Output:
```
2
```
#### append() Method
- Adds an element at the end of the list:
```python
list.append(element)
```
Example:
```python
list = [1,2]
list.append(3)
print(list)
```
Output:
```
[1,2,3]
```
#### extend() Method
- Add the elements of a given list (or any iterable) to the end of the current list:
```python
list.extend(iterable)
```
#### insert() Method
- Adds an element at the specified position:
```python
list.insert(position, element)
```
Example:
```python
a = [1, 2]
b = [3, 4]
a.extend(b)
print(a)
```
Output:
```
[1, 2, 3, 4]
```
#### pop() Method
- Removes the element at the specified position and returns it:
```python
list.pop(position)
```
Example:
```python
fruits = ['apple', 'banana', 'cherry', 'date']
fruits.pop(1)
print(fruits)
```
Output:
```
['apple', 'cherry', 'date']
```
#### remove() Method
- The remove() method removes the first occurrence of a given item from the list:
```python
list.remove(element)
```
Example:
```python
colors = ['red', 'green', 'blue', 'green']
colors.remove('green')
print(colors)
```
Output:
```
['red', 'blue', 'green']
```
#### clear() Method
- Removes all the elements from the list:
```python
list.clear()
```
Example:
```python
items = [10, 20, 30]
items.clear()
print(items)
```
Output:
```
[]
```
#### count() Method
- Returns the number of elements with the specified value:
```python
list.count(value)
```
Eaxample:
```python
nums = [1, 2, 2, 3, 2, 4]
print(nums.count(2))
```
Output:
```
3
```
#### reverse() Method
- Reverses the order of the list:
```python
list.reverse()
```
Eaxample:
```python
num = [1, 2, 3]
num.reverse()
print(num)
```
Output:
```
[3,2,1]
```

#### sort() Method
- Sorts the list:
```python
list.sort(reverse=True|False)
```
Eaxample:
```python
num = [9, 1, 2, 6, 3]
num.sort(reverse=True)
#sorted(list)
print(num)
num.sort(reverse=False)
print(num)
```
Output:
```
[9, 6, 3, 2, 1]
[1, 2, 3, 6, 9]
```
## Python List Methods table Sheet

| **Operation**           | **Code Example**                    | **Description**                   |
|------------------------|-----------------------------------|---------------------------------|
| **Create List**         | `my_list = [1, 2, 3]`             | Create a list                   |
| **Empty List**          | `empty = []`                      | Create an empty list            |
| **Access Element**      | `my_list[0]`                     | Get first element               |
| **Access Last Element** | `my_list[-1]`                    | Get last element                |
| **Slice List**          | `my_list[1:3]`                   | Get elements from index 1 to 2 |
| **Check Membership**    | `3 in my_list`                   | Check if 3 is in list           |
| **Append**              | `my_list.append(4)`              | Add element at end              |
| **Insert**              | `my_list.insert(1, 10)`          | Insert 10 at index 1            |
| **Extend**              | `my_list.extend([5,6])`          | Add multiple elements           |
| **Update Element**      | `my_list[0] = 100`               | Change element at index 0       |
| **Remove by Value**     | `my_list.remove(2)`              | Remove first occurrence of 2    |
| **Pop Last**            | `my_list.pop()`                  | Remove and return last element  |
| **Pop at Index**        | `my_list.pop(1)`                 | Remove and return element at 1  |
| **Delete Element**      | `del my_list[0]`                 | Delete element at index 0       |
| **Length**              | `len(my_list)`                   | Get number of elements          |
| **Sum**                 | `sum(my_list)`                   | Sum of elements (numbers only)  |
| **Loop Over Elements**  | `for item in my_list:`           | Loop through list items         |
|                        | `  print(item)`                  |                                 |
| **Loop with Index**     | `for i, val in enumerate(my_list):` | Loop with index and value  |
|                        | `  print(i, val)`                |                                 |
| **Sort List**           | `my_list.sort()`                 | Sort list in-place              |
| **Reverse List**        | `my_list.reverse()`              | Reverse list in-place           |
| **Copy List**           | `new_list = my_list.copy()`      | Create a shallow copy           |
| **Clear List**          | `my_list.clear()`                | Remove all elements             |


---
## Tuples
- Tuples are represented as comma-separated values of any data type within parentheses.

#### Tuple Creation
```python
variable_name = (element1, element2, ...)
```

- These elements can be of different data types.

#### Indexing
- The position of every element placed in the tuple starts from the 0th position and step by step it ends at length-1 position. Tuples are ordered, indexed, immutable, and the most secure collection of elements.
```python
thistuple = (1, 3, 7, 8, 7, 5, 4, 6, 8, 5)
print(thistuple.index(8))
```
Output:
```
3
```

- Methods:

#### count() Method
- It returns the number of times a specified value occurs in a tuple:
```python
tuple.count(value)
```
Example:
```python
thistuple = (1, 3, 7, 8, 7, 5, 4, 6, 8, 5)
print(thistuple.count(5))
```
Output:
```
2
```
#### index() Method
- It searches the tuple for a specified value and returns the position:
```python
tuple.index(value)
```
Example:
```python
thistuple = (1, 3, 7, 8, 7, 5, 4, 6, 8, 5)
print(thistuple.index(8))
```
Output:
```
3
```
## Python Touple Methods table Sheet
| **Topic**            | **Description**                               | **Example**                       |
|----------------------|-----------------------------------------------|---------------------------------|
| **Definition**       | Immutable ordered collection                   | `t = (1, 2, 3)`                 |
| **Creating**         | Parentheses or without parentheses             | `t1 = (1, 2, 3)` <br> `t2 = 1, 2, 3` |
| **Single element**   | Comma required to define a single-element tuple| `t = (5,)`                      |
| **Access elements**  | Indexing, slicing                              | `t[0]` → `1` <br> `t[1:3]` → `(2, 3)` |
| **Concatenation**    | Combine two tuples                             | `(1, 2) + (3, 4)` → `(1, 2, 3, 4)` |
| **Repetition**       | Repeat elements                                | `(1, 2) * 3` → `(1, 2, 1, 2, 1, 2)` |
| **Length**           | Number of elements                             | `len(t)`                        |
| **Membership check** | Check if element exists                         | `3 in t` → `True`               |
| **Unpacking**        | Assign tuple elements to variables             | `a, b, c = (1, 2, 3)`           |
| **Immutability**     | Elements cannot be changed after creation      | `t[0] = 5` → Error              |
| **Methods**          | Limited methods: `count()`, `index()`          | `t.count(2)` <br> `t.index(3)`  |
| **Nested tuples**    | Tuples inside tuples                           | `t = (1, (2, 3), 4)`            |

-------
## Sets
- A set is a collection of multiple values which is both unordered and unindexed. It is written in curly brackets.

#### Set Creation: Way 1
```python
var_name = {element1, element2, ...}
```
#### Set Creation: Way 2
```python
var_name = set([element1, element2, ...])
```
- Set is an unordered, immutable, non-indexed type of collection. Duplicate elements are not allowed in sets.

#### Set Methods
Let's talk about some of the methods of sets:

##### add() Method
- Adds an element to a set:
```python
set.add(element)
```
#### clear() Method
- Remove all elements from a set:
```python
set.clear()
```
#### discard() Method
- Removes the specified item from the set:
```python
set.discard(value)
```
#### intersection() Method
- Returns the intersection of two or more sets:
```python
set.intersection(set1, set2 ... etc)
```
#### issubset() Method
- Checks if a set is a subset of another set:
```python
set.issubset(set)
```
#### pop() Method
- Removes an element from the set:
```python
set.pop()
```
#### remove() Method
- Removes the specified element from the set:
```
set.remove(item)
```
#### union() Method
- Returns the union of two or more sets:
```python
set.union(set1, set2...)
```
## Python Set Methods table Sheet

## Creating Sets
```python
s = {1, 2, 3}          # set literal
s = set([1, 2, 3])     # from list
s = set()              # empty set
```

## Basic Properties
- Sets are **unordered** collections of **unique** elements.
- Elements must be **hashable** (immutable types like int, string, tuple).

---

## Adding and Removing Elements

| Operation        | Syntax                 | Description                              |
|------------------|------------------------|----------------------------------------|
| Add element      | `s.add(elem)`          | Adds `elem` to set `s`                  |
| Remove element   | `s.remove(elem)`       | Removes `elem`; raises KeyError if not found |
| Remove element   | `s.discard(elem)`      | Removes `elem` if present; no error if absent |
| Remove and return| `s.pop()`              | Removes and returns an arbitrary element |
| Clear set        | `s.clear()`            | Removes all elements                    |


## Set Operations

| Operation                 | Syntax                     | Description                           |
|---------------------------|----------------------------|-------------------------------------|
| Union                    | `s1 | s2` or `s1.union(s2)` | Elements in `s1` or `s2` or both    |
| Intersection             | `s1 & s2` or `s1.intersection(s2)` | Elements in both `s1` and `s2`       |
| Difference               | `s1 - s2` or `s1.difference(s2)` | Elements in `s1` but not in `s2`     |
| Symmetric Difference    | `s1 ^ s2` or `s1.symmetric_difference(s2)` | Elements in either `s1` or `s2` but not both |
| Subset check            | `s1 <= s2` or `s1.issubset(s2)` | True if all elements of `s1` in `s2`  |
| Superset check          | `s1 >= s2` or `s1.issuperset(s2)` | True if all elements of `s2` in `s1`  |
| Disjoint check          | `s1.isdisjoint(s2)`       | True if `s1` and `s2` have no common elements |

## Iteration
```python
for elem in s:
    print(elem)
```
## Set Comprehension
```python
s = {x for x in range(10) if x % 2 == 0}  # even numbers 0-9
```
## Example
```python
a = {1, 2, 3}
b = {3, 4, 5}

print(a | b)  # {1, 2, 3, 4, 5} - union
print(a & b)  # {3} - intersection
print(a - b)  # {1, 2} - difference
print(a ^ b)  # {1, 2, 4, 5} - symmetric difference
```
------
## Dictionaries
- The dictionary is an unordered set of comma-separated key:value pairs, within {}, with the requirement that within a dictionary, no two keys can be the same.

#### Dictionary
```python
<dictionary-name> = {<key>: value, <key>: value ...}
```
- Dictionary is an ordered and mutable collection of elements. Dictionary allows duplicate values but not duplicate keys.

#### Empty Dictionary
By putting two curly braces, you can create a blank dictionary:

```python
mydict = {}
```
#### Adding Element to a Dictionary
- By this method, one can add new elements to the dictionary:
```python
<dictionary>[<key>] = <value>
```
#### Updating Element in a Dictionary
- If a specified key already exists, then its value will get updated:
```python
<dictionary>[<key>] = <value>
```
#### Deleting an Element from a Dictionary
- del keyword is used to delete a specified key:value pair from the dictionary as follows:
```python
del <dictionary>[<key>]
```
#### Dictionary Functions & Methods
- Below are some of the methods of dictionaries:

#### len() Method
- It returns the length of the dictionary, i.e., the count of elements (key: value pairs) in the dictionary:
```python
len(dictionary)
```
#### clear() Method
- Removes all the elements from the dictionary:
```python
dictionary.clear()
```
#### get() Method
- Returns the value of the specified key:
```python
dictionary.get(keyname)
```
#### items() Method
- Returns a list containing a tuple for each key-value pair:
```python
dictionary.items()
```
#### keys() Method
- Returns a list containing the dictionary's keys:
```python
dictionary.keys()
```
#### values() Method
- Returns a list of all the values in the dictionary:
```python
dictionary.values()
```
#### update() Method
- Updates the dictionary with the specified key-value pairs:
```python
dictionary.update(iterable)
```


## Python Dictionary Methods table Sheet

| **Operation**               | **Code Example**                              | **Description**                              |
|-----------------------------|----------------------------------------------|----------------------------------------------|
| **Create dictionary**        | `d = {}` <br> `d = {"key": "value"}`         | Create empty or initialized dictionary       |
| **Access value by key**      | `d["key"]`                                    | Get value by key (raises `KeyError` if missing) |
| **Access with default**      | `d.get("key")` <br> `d.get("key", default)`  | Get value or default if key missing           |
| **Add or update key**        | `d["key"] = value`                            | Add new key or update existing key            |
| **Remove key**               | `del d["key"]`                                | Remove key (raises `KeyError` if missing)     |
| **Pop key**                  | `d.pop("key")` <br> `d.pop("key", default)`  | Remove and return value, or default if missing |
| **Check if key exists**      | `"key" in d`                                  | Returns `True` if key exists                    |
| **Get keys**                 | `d.keys()`                                    | Returns dict_keys view of all keys             |
| **Get values**               | `d.values()`                                  | Returns dict_values view of all values         |
| **Get items**                | `d.items()`                                   | Returns dict_items view of (key, value) pairs |
| **Iterate keys**             | `for key in d:` <br> `  print(key)`           | Loop through keys                              |
| **Iterate keys and values** | `for key, val in d.items():` <br> `  print(key, val)` | Loop through keys and values                   |
| **Copy dictionary**          | `new_d = d.copy()`                            | Creates shallow copy                           |
| **Clear dictionary**         | `d.clear()`                                   | Removes all items                              |
| **Dictionary comprehension**| `{x: x*x for x in range(5)}`                   | Create dict with comprehension                  |
| **Merge dicts (3.9+)**       | `d3 = d1 | d2`                                | Merge two dicts (d2 overrides d1)             |
| **Set default value**        | `d.setdefault("key", default)`                | Return existing value or set and return default|
| **Update dictionary**        | `d.update({"key": "value"})`                   | Update dict with another dict or iterable      |

---
# Object Oriented Programming (OOPS)
- It is a programming approach that primarily focuses on using objects and classes. The objects can be any real-world entities.

## class
- The syntax for writing a class in Python:
```python
class class_name:
    pass  # statements
```
## Creating an Object
Instantiating an object can be done as follows:
```python
<object-name> =
```

## 1. Class & Object

```python
class ClassName:
    # class body
    pass

obj = ClassName()  # Creating an object (instance)
```

---

## 2. Constructor 
```__init__```

```python
class Person:
    def __init__(self, name, age):
        self.name = name    # instance variable
        self.age = age

p1 = Person("Alice", 30)
```

---

## 3. Instance Variables & Methods

```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, my name is {self.name}")

p = Person("Bob")
p.greet()  # Output: Hello, my name is Bob
```


## 4. Class Variables

```python
class Person:
    species = "Homo sapiens"  # Class variable

    def __init__(self, name):
        self.name = name

print(Person.species)
```


## 5. Inheritance

```python
class Animal:
    def speak(self):
        print("Animal speaks")

class Dog(Animal):
    def speak(self):
        print("Woof!")

d = Dog()
d.speak()  # Output: Woof!
```


## 6. Encapsulation (Private/Protected)

```python
class Person:
    def __init__(self, name):
        self._protected = name        # Protected (convention)
        self.__private = "secret"     # Private (name mangling)

p = Person("Alice")
print(p._protected)      # Accessible but discouraged
# print(p.__private)     # Error

print(p._Person__private)  # Access private variable (not recommended)
```

## 7. Polymorphism

```python
class Cat:
    def speak(self):
        print("Meow")

class Dog:
    def speak(self):
        print("Woof")

def animal_sound(animal):
    animal.speak()

c = Cat()
d = Dog()

animal_sound(c)  # Meow
animal_sound(d)  # Woof
```


## 8. Method Overriding

```python
class Parent:
    def greet(self):
        print("Hello from Parent")

class Child(Parent):
    def greet(self):
        print("Hello from Child")

c = Child()
c.greet()  # Output: Hello from Child
```

## 9. `super()` Function

```python
class Parent:
    def __init__(self):
        print("Parent init")

class Child(Parent):
    def __init__(self):
        super().__init__()
        print("Child init")

c = Child()
# Output:
# Parent init
# Child init
```


## 10. Special Methods (Magic / Dunder Methods)

- `__str__` – String representation  
- `__repr__` – Official string representation  
- `__eq__` – Equality check  

```python
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __str__(self):
        return f"Point({self.x}, {self.y})"

    def __eq__(self, other):
        return self.x == other.x and self.y == other.y

p1 = Point(1, 2)
p2 = Point(1, 2)
print(p1)          # Point(1, 2)
print(p1 == p2)    # True
```

## 11. Class Methods & Static Methods

```python
class MyClass:
    count = 0

    @classmethod
    def increment(cls):
        cls.count += 1

    @staticmethod
    def greet():
        print("Hello!")

MyClass.increment()
print(MyClass.count)  # 1
MyClass.greet()      # Hello!
```

## Summary Table:

| Concept              | Syntax / Example                       | Notes                          |
|----------------------|--------------------------------------|--------------------------------|
| Class                | `class ClassName:`                    | Defines a class                 |
| Object               | `obj = ClassName()`                   | Creates an object              |
| Constructor          | `def __init__(self, ...):`            | Initialize instance variables  |
| Instance Variable    | `self.var`                           | Unique to each object          |
| Class Variable       | `ClassName.var`                      | Shared across all instances    |
| Inheritance          | `class Child(Parent):`               | Subclass inherits from parent  |
| Encapsulation        | `_var` (protected), `__var` (private)| Name mangling for private vars |
| Polymorphism         | Same method name in different classes| Allows for flexible code       |
| Method Overriding    | Define method with same name in subclass | Overrides parent method        |
| `super()`            | `super().method()`                   | Calls parent class method      |
| Magic Methods        | `__str__`, `__eq__`, etc.            | Customize class behavior       |
| Class Method         | `@classmethod`                       | Method receives class as first param |
| Static Method        | `@staticmethod`                      | Method does not receive class/instance |
