# Testing and Modules

## TDD with Python

- First thing is think small. Baby steps for testing.
- Test names should be considered live documentation. I.E. `def test_should_return_true ():`
- The test module should also follow the same name as the module we are testing. Also to separate test files from production code
- **AAA**
  - *Arrange*: organize the data needed to execute that piece of code
  - *Act*: execute code being tested
  - *Assert*: check that the output is as expected
- **The Cycle**
  1. Write a test and make it fail
  2. Write the feature and make it pass
  3. Refactor your code

## `__name__==__main__`

- This defines the source file for the python interpreter
- Using this method with multiple modules stops the need for commenting out the function call in the original module.

## Recursion

- What is **Recursion:**
  - It is the process in which a function calls itself directly or indirectly
- **Base Condition:**
  - This is the small problem and when solved multiple times will lead to the desired solution of the main problem
- **Direct Recursion**
  - This is a function in which it invokes a function of the same name
- **Indirect Recursion**
  - Functions are not the same name
- **Recursive** programming provides clean coding but requires more memory space than normal coding

# Useful Links

- [Recursion](https://www.geeksforgeeks.org/recursion/)
- [TDD](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
- [What does if `__name__==__main__` do?](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)