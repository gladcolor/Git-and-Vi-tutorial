# What is Exception?
In most programming language, if the code cannot deal with the data, it will trigger an error then stop to
 work. To avoid this situation and make sure the code can run continuously, Exceptions is used to cope with exceptional situations occur in your program. 
For example, if the program is going to read a file and the file does not exist, it needs to know how to act in this
 occasion. 

# Why use Exception?
The program will face many invalid, unexpected inputs or situations, once the code cannot handle these occasions
, Exception catch the error of the code then let the program go to another branch to ensure the program still can run
 smoothly. 

# How to use Exception?
Try-Except statement is used in Python to implement Exception. A nice instruction of Exception in Python can be found
 here.
[Python Exceptions: An Introduction](https://realpython.com/python-exceptions/)

In this article, the picture below shows the most common usage of Exception in Python. 
![](https://files.realpython.com/media/try_except.c94eabed2c59.png)

An simple examle is below:
 ```python
try:    
    with open('file.log') as file:
        read_data = file.read()
except Exception as e:
    print(e)
```



