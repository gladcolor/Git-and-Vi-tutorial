# What are property and attribute?
Property and attribute, are almost the same thing used by most programming languages. They are the variables stored
 inside in class. Developers can assign values to properties or attributes, or change the values.



# Why use property and attribute?
The answer is quite simple: classes need places to store data, such as input, output, or temporary results. Statuses
 are also can be recorded by properties or attributes. 


# How to use property and attribute?
Python uses the term of attribute. The sample below shows how to use the attribute in Python

```python
class Computer():
    cpu = 'i7'
    def getCPU(self):
        print(self.cpu)
        
    def setCPU(self, cpu_name):
        self.cpu = cpu_name

computer = Computer()
computer.getCPU()    # i7
computer.setCPU('AMD')
computer.getCPU()    # AMD
``` 




