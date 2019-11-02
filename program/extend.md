# What is extending class？
Extending class, or more formally, inheritance, is one of the core concepts of object-oriented programming languages
. 
>It is a mechanism where you can to derive a class from another class for a hierarchy of classes that share a set of
 attributes and methods.
>--[Thorben Janssen](https://stackify.com/oop-concept-inheritance/)
# Why extend class?
In object-oriented programming, inheritance enables new objects to take on the properties of existing objects. A class that is used as the basis for inheritance is called a superclass or base class. A class that inherits from a superclass is called a subclass or derived class. The terms parent class and child class are also acceptable terms to use respectively. A child inherits visible properties and methods from its parent while adding additional properties and methods of its own.

Source:[OBJECT-ORIENTED PROGRAMMING CONCEPTS: INHERITANCE](https://www.adobe.com/devnet/actionscript/learning/oop-concepts/inheritance.html)

# How to extend class?
[GeeksforGeeks.com](https://www.geeksforgeeks.org/inheritance-in-python/) give us a simple but good example to extend class in Python.

```python
# A Python program to demonstrate inheritance  
   
# Base or Super class. Note object in bracket. 
# (Generally, object is made ancestor of all classes) 
# In Python 3.x "class Person" is  
# equivalent to "class Person(object)" 
class Person(object): 
       
    # Constructor 
    def __init__(self, name): 
        self.name = name 
   
    # To get name 
    def getName(self): 
        return self.name 
   
    # To check if this person is employee 
    def isEmployee(self): 
        return False
   
   
# Inherited or Sub class (Note Person in bracket) 
class Employee(Person): 
   
    # Here we return true 
    def isEmployee(self): 
        return True
   
# Driver code 
emp = Person("Geek1")  # An Object of Person 
print(emp.getName(), emp.isEmployee()) 
   
emp = Employee("Geek2") # An Object of Employee 
print(emp.getName(), emp.isEmployee()) 
```

