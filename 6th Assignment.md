## Question-1

### Object-oriented programming

OP is a programming paradigm based on the concept of "objects", which can contain data, in the form of fields 
(often known as attributes or properties), and code, in the form of procedures (often known as methods).

A feature of objects is an object's procedures that can access and often modify the data fields of the object with which 
they are associated (objects have a notion of "this" or "self"). 

In OOP, computer programs are designed by making them out of objects that interact with one another.
OOP languages are diverse, but the most popular ones are class-based.

## Question-2

### Benefits of OOPs

1. The primary purpose of OOP is to increase the flexibility and maintainability of programs. 
2. OOP brings together data and its behaviour(methods) in a single location(object) makes it easier to understand how a 
   program works.
3. OOP provides a clear modular structure for programs.
4. It is good for defining abstract data types.
5. Implementation details are hidden from other modules and other modules has a clearly defined interface.
6. It is easy to maintain and modify existing code as new objects can be created with small differences to existing ones.
7. Objects can also be reused within an across applications. 
8. The reuse of software also lowers the cost of development. 
9. OOP languages allows you to break down your software into bite-sized problems that you then can solve — one object at a time. 

 ## Question-3

There’s a thin line between method and function:

The major difference is that we call method on an object, but it’s not the same with functions. 
Methods may modify an object; functions don’t.

### Mehtods
1. Method is called by its name, but it is associated to an object (dependent).
2. A method is implicitly passed the object on which it is invoked.
3. It may or may not return any data.
4. A method can operate on the data (instance variables) that is contained by the corresponding class
5. An object has attributes and behaviours. These behaviours are called methods.

### Functions
1. Function is block of code that is also called by its name. (independent)
2. The function can have different parameters or may not have any at all. If any data (parameters) are passed, 
they are passed explicitly.
3. It may or may not return any data.
4. Function does not deal with Class and its instance concept.

## Question-4

### Class
A class is a blueprint for the objects. For example, Asad, Rashid, Ali  are all objects so we can 
define a template (blueprint) class Male for these objects. The class can define the common attributes and behaviours of all 
the objects.

### Object
An object is an entity that has attributes and behaviour. For example, HumanBeing is an object who has attributes 
such as height, weight, color etc. and has certain behaviours such as walking, talking, eating etc.

### Attributes
There are two types of attribute in Python:
1. Instance Attribute
An instance attribute is a Python variable belonging to one, and only one, object. This variable is only 
accessible in the scope of this object and it is defined inside the constructor function, __init__(self,..) of the class.

2. Class Attribute
A class attribute is a Python variable that belongs to a class rather than a particular object. It is shared between all the objects of this class and it is defined outside the constructor function, __init__(self,...), 
of the class.

### Behavior
Behaviors are actions that can occur on an object.
For instance, an object could represent a person with a name property, age, address, etc., 
with behaviors like walking, talking, breathing, and running.

## Question-5
~~~
class Car:
  def __init__(self,name,model,color,brand,price):
    self.name = name
    self.model = model
    self.color = color
    self.brand = brand
    self.price = price
    if color == 'White':
       self.price = price+(price * 0.05)
def names_of_cars():
    print('1 - {}\n2 - {}\n3 - {}\n4 - {}\n5 - {}\n'.format(car1.name,car2.name,car3.name,car4.name,car5.name))
def prices_of_cars():
    print('{} = {}\n{} = {}\n{} = {}\n{} = {}\n{} = {}\n'.format(car1.name,car1.price,car2.name,car2.price,car3.name,car3.price,car4.name,car4.price,car5.name,car5.price))
def Models():
    print('{} ({})\n{}({})\n{}({})\n{} ({})\n{} ({})\n'.format(car1.name,car1.brand,car2.name,car2.brand,car3.name,car3.brand,car4.name,car4.brand,car5.name,car5.brand))
car5 = Car('Alto', 2007,'Olive','Suzuki',1300000)
car2 = Car('Civic',2012,'Black','Honda',1000000)
car3 = Car('Lancer',2002,'Red','Mitsubishi',2500000)
car4 = Car('Santana',2019,'White','Hyundai',1600000) 
car1 = Car('Corolla',1999,'Golden','Toyota', 200000)
print('\nCars Available for Sale')
print('=======================')
names_of_cars()
print('\nPrice List')
print('=======================')
prices_of_cars()
print('\nBrands')
print('=======================')
Models()
~~~
