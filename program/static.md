# What is Static?
Static methods in Python are extremely similar to python class level methods, the difference being that a static method is bound to a class rather than the objects for that class.
 

# Why Static?
A static method can be called without an object for that class. This also means that static methods cannot modify the
 state of an object as they are not bound to it. Static method provides convenience when using the method from a class. Static methods have a very clear use-case. When we need some functionality not w.r.t an Object but w.r.t the complete class, we make a method static. This is pretty much advantageous when we need to create Utility methods as they aren’t tied to an object lifecycle usually.

# How to use Static?
Using @staticmethod is a  subtle way of creating a Static method.
```
class Calculator:

    # create addNumbers static method
    @staticmethod
    def multiplyNums(x, y):
        return x + y

print('Product:', Calculator.multiplyNums(15, 110))
```
Finally, note that in a static method, we don’t need the self to be passed as the first argument.

[Source:Python static method](https://www.journaldev.com/18722/python-static-method)


Someone will notice the term Static Variable. In computer programming, a static variable is a variable that has been allocated "statically", meaning that its lifetime (or "extent") is the entire run of the program. This is in contrast to shorter-lived automatic variables, whose storage is stack allocated and deallocated on the call stack; and in contrast to objects, whose storage is dynamically allocated and deallocated in heap memory. 

Here is an example for dealing with the class variable in Python:

```
class myClass(object):
    i = 3
print(myClass.i)  # 3
```

```
class myClass(object):
    i = 3
print(myClass.i)  # 3

myClass.i = 10
print(myClass.i)  # 10, the i can be changed.
```

```
class myClass(object):
    i = 3
print(myClass.i)  # 3

myc = myClass()
myc.i = 20

print(myc.i)  # 20, the i in the instance of myc can be changed.
print(myClass.i)  # 3, the i in myClass is not changed.

myClass.i = 30
print(myClass.i)  # 30, the i in myClass is changed.
print(myc.i)  # 20, the i in the instance of myc can be changed.

myc2 = myClass()
print(myc2.i)  # 30 
```