# What is reading files?
Reading file is necessary in every programming language, and it is a common method to exchange data. The program
 reads files to get data then writes files to store the results.

# Why reading file?
Files is is simple way to store data. Actually, very piece of data or information is stored in a file, even in the
 database. Thence, reading file is a basic operation when programming.


# How to reading file?
In Python, the basic operation of files is like:

1. Create a text file:
```python
f = open('myfile.txt', 'w')
```


2. Write a text file:
```python
f.write('I am a line.')
```

3. Save a text file:
```python
f.close()
```

4. Read a file:
```python
f = open('myfile.txt', 'r')
content = f.read()

```
