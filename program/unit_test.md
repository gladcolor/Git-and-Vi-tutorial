# What is Unit Test?
I think this definition is very clean:
>Unit Testing is the first level of software testing where the smallest testable parts of a software are tested. This is used to validate that each unit of the software performs as designed.
The unittest test framework is python’s xUnit style framework.
>--GeeksforGeeks.org, https://www.geeksforgeeks.org/unit-testing-python-unittest/
# Why use Unit Test?
Before the code is used or embedded into higher level program, it should be proved working as excepted. Unit Test is
 the first approach to show the effectiveness of the code. Otherwise, the error in the code needs much more endeavor
  to find, costing a large amount of resources.


# How to use Unit Test?
In Python, a built-in moudle is provided for developers to conduct Unit Test. The official documentation list a great
 exmaple below. Normally, the Unit Test code is written in a .py file, separating from the .py file of the code needs
  to be tested. 

```python
import unittest

class TestStringMethods(unittest.TestCase):

    def test_upper(self):
        self.assertEqual('foo'.upper(), 'FOO')

    def test_isupper(self):
        self.assertTrue('FOO'.isupper())
        self.assertFalse('Foo'.isupper())

    def test_split(self):
        s = 'hello world'
        self.assertEqual(s.split(), ['hello', 'world'])
        # check that s.split fails when the separator is not a string
        with self.assertRaises(TypeError):
            s.split(2)

if __name__ == '__main__':
    unittest.main()
```