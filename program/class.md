# What is class?
In object-oriented programming, a class means a design, or a blueprint for an object or entity in real world. A class
 can store data and has behavior (functions or methods) to process its data.
 
 ![](https://dziganto.github.io/assets/images/class_diagram.png?raw=true)
 
[Picture from: Understanding Object-Oriented Programming Through Machine Learning](https://dziganto.github.io/classes/data%20science/linear%20regression/machine%20learning/object-oriented%20programming/python/Understanding-Object-Oriented-Programming-Through-Machine-Learning/)

# Why class?
Object-oriented programming (OPP) brings features of real-world entities like inheritance, hiding, polymorphism, etc
. The
 main aim of OOP is to bind together the data and the functions that operate on them so that no other part of the code can access this data except that function.

# How to class?
[Karleigh Moore, Evans Njeru, Matas Pocevicius](https://brilliant.org/wiki/classes-oop/) have a nice blog to show how
 to implement a Car class in Python:

```
class Car(object):
    def __init__(self, model, passengers, color, speed):
        self.model = model
        self.passengers = passengers
        self.color = color
        self.speed = speed

    def accelerate(self):
        self.speed = self.speed + 2
        print (self.speed)

bmw = Car("BMW", 4, "red", 5)
ferrari = Car("Ferrari", 2, "black", 10)
ford = Car("Ford", 6, "blue", 6)

bmw.accelerate()
print (bmw.color)

ferrari.accelerate()
print (ferrari.color)
ferrari.accelerate() #note that the speed has been updated from the previous accelerate call

print (ford.passengers)
ford.accelerate()
```

 ![](https://ds055uzetaobb.cloudfront.net/brioche/uploads/pJZt3mh3Ht-prettycars.png?width=1200)
 
 ![](https://webcourses.ucf.edu/courses/1249560/files/64181432/download?verifier=GH3L7R124eDD6AGbwXwFC4OYrzGNNy4UsnarTveV&wrap=1)