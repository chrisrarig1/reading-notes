# Class 04 Reading

## Classes and Objects

- *Classes* are a template to create your objects in
- *Objects* are a grouping of variables and functions
- To access an object variable inside a class we use dot notation i.e. `myclass.variable`
- To access an object function inside a class we use dot notation to call the function i.e `myclass.function()`
- *`__init__()`* This is a function that is called when assigning values in a class

## Thinking Recursively

- Break problems into smaller chunks to make it easier to solve
- *Recursive Functions* are routines that calls itself directly or indirectly

## Python Testing with Pytest

- *Fixtures* are objects available to all tests
- Using `pytest.fixture` allows functions to be run prior to the test functions. It is used to feed certain data pieces to th test
- *Code Coverage* this is a feature that can check to ensure all your test have run all code.
- To use code coverage download the package pytest-cov and invoke `pytest --cov` and `coverage html`

# Useful Links

- [Thinking Recursively](https://realpython.com/python-thinking-recursively/)
- [Pytest](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)
- [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)