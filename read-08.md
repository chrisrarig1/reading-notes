# List Comprehensions

## Create a List with range()

- When using the `range()` function Python loops through each item in the given range and saves a copy of the item in a new list
- Syntax: `[x for x in range(10)]`

## Create a List using Loops and List Comprehensions

- For Loop:
  - `for x in range(10):`
        `list.append(x)`
- List Comprehensions:
  - Returns a list of numbers times two:
    - `list = [x*2 for x in range(10)]`

## Multiplying Parts of a list

- Similar to the last section List Comprehensions:
  - Returns a list of numbers times two:
    - `list = [x*2 for x in range(10)]`

## Showing the First Letter of each word

- authors = `["list of names"]`
  - letters = `[ name[0] for name in authors]`
  - Returns first letters of each name

## Separating the characters in a string

- Using List Comprehensions:
  - `[x for x in "string"]` isolates each character and puts it into a new list separated by commas.

## Lower and Upper case converter

- Using List Comprehensions:
  - lower_case = `[ x.lower() for x in ['A','B','C']]`
  - upper_case = `[ x.upper() for x in ['a','b','c']]`

## Print numbers only from a given string

- This can be done using list comprehension with a filter
  - user_data = "Donald Duck 402-689-2456"
  - phone_number = `[x for x in user_data if x.isdigit()]`

## Parsing a file

- `file = open("file_name.txt", 'r')`
- `text = [ x for x in file]`
- `for x in file:`
    `print(x)`

# Useful Links

- [List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python#htoc-create-a-list-with-range)
- [Primer on Decorators](https://realpython.com/primer-on-python-decorators/)