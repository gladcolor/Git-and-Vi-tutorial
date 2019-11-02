# What is factory?
In object-oriented programming (OOP), a factory is an object for creating other objects – formally a factory is a function or method that returns objects of a varying prototype or class from some method call, which is assumed to be "new". More broadly, a subroutine that returns a "new" object may be referred to as a "factory", as in factory method or factory function. This is a basic concept in OOP, and forms the basis for a number of related software design patterns.

Factory is a type of object to create new objects according to the input parameters.


# Why use factory?
In class-based programming, a factory is an abstraction of a constructor of a class, while in prototype-based programming a factory is an abstraction of a prototype object. A constructor is concrete in that it creates objects as instances of a single class, and by a specified process (class instantiation), while a factory can create objects by instantiating various classes, or by using other allocation schemes such as an object pool. A prototype object is concrete in that it is used to create objects by being cloned, while a factory can create objects by cloning various prototypes, or by other allocation schemes.

Factories may be invoked in various ways, most often a method call (a factory method), sometimes by being called as a function if the factory is a function object (a factory function). In some languages factories are generalizations of constructors, meaning constructors are themselves factories and these are invoked in the same way. In other languages factories and constructors are invoked differently, for example using the keyword new to invoke constructors but an ordinary method call to invoke factories; in these languages factories are an abstraction of constructors but not strictly a generalization, as constructors are not themselves factories.


# How to use factory?

```python
'''
implement factory pattern
'''
import csv

class CSVReader(object):
    '''client side CSVReader caller'''
    def callCreateCSVReader(type, filepath, filename):
        Reader = createCSVReader(type)
        return Reader(filepath, filename)

def createCSVReader(type):
    '''server side CSVReader caller'''
    if type == "TwoFieldsCSV":
        return getTwoValuesCSVData
    elif type == "ThreeFieldsCSV":
        return getThreeValuesCSVData
    else:
        return ValueError(type)


def getFieldNames(csv_reader) -> dict:
    '''set field names'''
    return csv_reader.fieldnames

def readCSVData(filepath,filename) -> list:

    '''
    read csv data and save them to list
    every row is the dictionary object
    '''

    '''list to contain each row dictionary'''
    csv_data = []

    with open(filepath+filename, mode='r') as csv_file:
        '''read csv data via csv DictReader'''
        csv_reader = csv.DictReader(csv_file)
        '''get csv data field names'''
        fieldNames = getFieldNames(csv_reader)

        for row in csv_reader:
            csv_data.append(row)

    csv_file.close()

    return (fieldNames,csv_data)

def getTwoValuesCSVData(filepath,filename):

    fieldNames,csvData = readCSVData(filepath,filename)

    value1 = fieldNames[0]
    result = fieldNames[1]

    return (value1,result,csvData)

def getThreeValuesCSVData(filepath,filename):

    fieldNames,csvData = readCSVData(filepath,filename)

    value1 = fieldNames[0]
    value2 = fieldNames[1]
    result = fieldNames[2]

    return (value1,value2,result,csvData)

if __name__ == '__main__':
    csv_reader = CSVReader()
    value1,value2,result,csvData = csv_reader.callCreateCSVReader("ThreeFieldsCSV","./csv_files/","Unit Test Multiplication.csv")

```


[Source: Factory in Wikipedia](https://en.wikipedia.org/wiki/Factory_(object-oriented_programming)