# What is Decorator?
In object-oriented programming, the decorator pattern is a design pattern that allows behavior to be added to an
 individual object, dynamically, without affecting the behavior of other objects from the same class. 

# Why use Decorator?
The decorator pattern is often useful for adhering to the Single Responsibility Principle, as it allows functionality to be divided between classes with unique areas of concern. The decorator pattern is structurally nearly identical to the chain of responsibility pattern, the difference being that in a chain of responsibility, exactly one of the classes handles the request, while for the decorator, all classes handle the request.

# How to use Decorator?
Decorators are very powerful and useful tool in Python since it allows programmers to modify the behavior of function or class. Decorators allow us to wrap another function in order to extend the behavior of wrapped function, without permanently modifying it.

In Decorators, functions are taken as the argument into another function and then called inside the wrapper function
. Below is an example of adding a timer decorator to the factorial() function.

```python
# importing libraries 
import time 
import math 
  
# decorator to calculate duration 
# taken by any function. 
def calculate_time(func): 
      
    # added arguments inside the inner1, 
    # if function takes any arguments, 
    # can be added like this. 
    def inner1(*args, **kwargs): 
  
        # storing time before function execution 
        begin = time.time() 
          
        func(*args, **kwargs) 
  
        # storing time after function execution 
        end = time.time() 
        print("Total time taken in : ", func.__name__, end - begin) 
  
    return inner1 
  
  
  
# this can be added to any function present, 
# in this case to calculate a factorial 
@calculate_time
def factorial(num): 
  
    # sleep 2 seconds because it takes very less time 
    # so that you can see the actual difference 
    time.sleep(2) 
    print(math.factorial(num)) 
  
# calling the function. 
factorial(10) 

# output:
# 3628800
# Total time taken in :  factorial 2.000936985015869
```

Sources: 
1. [Decorator pattern](https://en.wikipedia.org/wiki/Decorator_pattern)
2. [Geeksforgeeks.org](https://www.geeksforgeeks.org/unit-testing-python-unittest/)