# INHERITANCE -> reusability
# ENCAPSULATION -> data Security
# ABSTRACTION -> data Hiding
# POLYMORPHISM -> 

## Encapsulation: 
ncapsulation refers to the bundling of data and methods/functions that operate on that data into a single unit called a class. It allows for data hiding and protects the internal state of an object from direct access by other code. The class provides interfaces (such as methods) to interact with the data, controlling how it is accessed and modified. Encapsulation promotes information hiding, enhances code maintainability, and provides abstraction.

```python

class Test:
    def __init__(self,email,password,test):
        self.__email = email
        self.__password = password
        self.test = test
        
    def Jay(self):
        print("my email is ",self.email)
        print("my password is ",self.__password)
        

test=test("jay@gmail.com",123,"Jay")


print(Test.__password) # error couse of this private object
print(Test.jay) # aa use thase kem keaa private ni male 

```

## Inheritance: 
Inheritance is a mechanism that allows a class (called a child or subclass) to inherit properties and methods from another class (called a parent or superclass). The child class inherits the characteristics of the parent class, enabling code reuse and promoting the concept of hierarchical classification. It allows the child class to extend or modify the behavior of the parent class. Inheritance establishes an "is-a" relationship between classes, where a child class is a specialized version of the parent class.

```python 
class school_form:
     def detauls(name):
        print("my name is ",name)
    
class Test(school_form):
     def skills():
        print(" im good dancer")  
mydata = Test
mydata.detauls("jay")


```
## Polymorphism: 
Polymorphism means the ability of an object to take on multiple forms or have multiple behaviors. In OOP, polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables code to work with objects of different types through a unified interface. Polymorphism is achieved through method overriding and method overloading.

- Method Overriding: Method overriding occurs when a subclass provides its own implementation of a method that is already defined in its parent class. The method in the subclass overrides the method in the parent class, allowing the subclass to provide a specialized implementation.

```python

Over Riding 
class Perent:
    def jay():
        print("jay")
        
class Child(Perent):
    def jay():
        print("shibakmbhuhga")
        
obj = Child
obj.jay()

- Method Overloading: Method overloading involves defining multiple methods with the same name but different parameters in a class. The appropriate method to be called is determined based on the number of arguments or the data types of the arguments. Method overloading allows the class to provide different ways of invoking a method based on the context.

python
def sum(a,b):
    print(a+b)
    

def sum(a,b,c):
    print(a+b+c)


sum(10,10,10)
```
## Abstraction: 
Abstraction is the process of representing complex real-world entities as simplified models within the program. It focuses on the essential features of an object while hiding the unnecessary details. Abstraction allows programmers to create abstract classes or interfaces that define common behavior or contracts without specifying the implementation details. It provides a higher-level view of objects and helps in managing complexity, promoting modularity and code reusability.

These four pillars of OOP provide a foundation for building modular, extensible, and maintainable code by organizing data and behavior into cohesive units (classes) and promoting code reuse through inheritance and polymorphism.

```python

from abc import ABC, abstractmethod

class ATM(ABC):
    @abstractmethod
    def bob(self):
        pass
    
    @abstractmethod    
    def SBI(self):
        pass
    
class Child(ATM):
    def bob(self,jay):
        print(" This is BOB Bank",jay)
        
    def SBI(self):
        print(" This is SBI Bank")
        
        
obj = Child()
obj.bob("ajaaaasas")

```
