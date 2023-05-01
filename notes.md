# My Tech Notes

Edit Notes Online (needs auth), [https://github.dev/0xdec0de5/my-notebook/blob/main/notes.md](https://github.dev/0xdec0de5/my-notebook/blob/main/notes.md)

### Python

#### Packaging

My PyPi account, [https://pypi.org/manage/projects/](https://pypi.org/manage/projects/)

PyPi packages (guide), [https://packaging.python.org/en/latest/](https://packaging.python.org/en/latest/)

- Creating initial package, [https://packaging.python.org/en/latest/flow/](https://packaging.python.org/en/latest/flow/)

#### General

__Classes__

Instance vs. Class/Static vars, [https://docs.python.org/3/tutorial/classes.html#class-and-instance-variables](https://docs.python.org/3/tutorial/classes.html#class-and-instance-variables)

```python
class Dog:

    kind = 'canine'         # class variable shared by all instances

    def __init__(self, name):
        self.name = name    # instance variable unique to each instance

```

__Unit Tests__

example of lifecycle in a Test class

```python
import unittest

class MyTest(unittest.TestCase):
    @classmethod
    def setUpClass(cls):
        pass  # very first to run - static

    @classmethod
    def tearDownClass(cls):
        pass  # very last to run - static

    def setUp(self):
        pass  # runs in front of every test fn

    def tearDown(self):
        pass  # runs after every test fn

    def test_a_test(self):
        # setUp runs
        self.assertTrue(True)
        # tearDown runs

```
