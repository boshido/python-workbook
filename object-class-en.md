# Class / Object #

#### In terms of "Class" ####
Class is what you can call it as "Blueprint", prepared to be used to create objects with 2 things inside class itself  
1. Property - Describe what class can contain data inside itself that means class can have multiple variables and objects inside itself, which can be just integer and boolean or another class's object, it can be private or public variables
2. Method - Describe what class can do with/without the property inside itself, method can just return static result or calculate the values inside properties

Python itself is an object oriented programming language, so most of all variables you use in python, they are created by "Class" except primitive type variables such as integer, short, boolean, float, etc.

Python's class will have  methods that is designed for developer can write logic to act in each event

###### Example
```python
class Book:
  def __init__(self, title, price):
    self.__title = title
    self.__price = price

  def __lt__(self, other):
    return self.price < other.price

  def __str__(self):
    return 'price: ' + title + ', price: ' + price

  def get_book_title:
    return self.__title
```

* Method ```__init__``` is the first method to be executed when object is created, this method usually uses for initializing the properties inside object, as you can see in example the properties ```(title, price)```

* Method ```__lt__``` will be used automatically when objects in same class do comparing or sorting
  ```
  book1 = new Book('Python', 199)
  book2 = new Book('NodeJS', 50)
  if book1 < book2
  books = [book1, book2].sort()
  ```


* Method ```__str__``` will be used automatically when objects is an argument of function print ```print(book1)```
