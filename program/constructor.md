# What is constructor?
A constructor is a special method of a class or structure in object-oriented programming that initializes an object of that type. A constructor is an instance method that usually has the same name as the class, and can be used to set the values of the members of an object, either to default or to user-defined values.


# Why use constructor?
Constructors are generally used for instantiating an object.The task of constructors is to initialize(assign values) to the data members of the class when an object of class is created.In Python the __init__() method is called the constructor and is always called when an object is created.


# How to use constructor?
Constructors are not called explicitly and are invoked only once during their lifetime. In the case of a hierarchy of classes where a derived class inherits from a parent class, the execution sequence of the constructor is a call to the constructor of the parent class first and then that of the derived class. Constructors cannot be inherited.
In Python, to access the constructor using the code like this:
```python
class Add: 
    num1 = 0
    num2 = 0
 
    # parameterized constructor 
    def __init__(self, a, b): 
        self.num1 = a 
        self.num2 = b 
```



Source:(https://www.techopedia.com/definition/5656/constructor)