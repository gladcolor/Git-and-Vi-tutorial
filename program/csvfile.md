# What is CSV file?
CSV is a Comma Separated Values (CSV) file in a plain text file that contains a list of data. 

![](img/csv1.jpg)


# Why use CSV file?
CSV files are often used for exchanging data between different applications. It is simple, human readable, and is very
 easy to
 check manually.
 
# How to use CSV file?
In Python, there is a built-in module to read and write CSV files. The official document list basic usage in [here
](https://docs.python.org/3/library/csv.html):

The simplest example of reading a CSV file:
```python
import csv
with open('some.csv', newline='') as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
```

The corresponding simplest possible writing example is:
```python
import csv
with open('some.csv', 'w', newline='') as f:
    writer = csv.writer(f)
    writer.writerows(someiterable)
```



