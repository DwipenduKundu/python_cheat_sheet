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