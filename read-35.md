# Pythonisms

## Dunder Methods

- A set of predefined methods you can use to enrich your classes.
- `__init__ `- sets up objects for a class
- `__repr__`- the string representation of an object
- `__str__`- the informal way to represent a string
- `__len__`- generates length
- `__reversed__`- reverses order
- `__eq__`- equal too boolean
- `__lt__`- less than boolean
- `__add__`- merge or add
- `__call__`- makes object callable
- `__enter__`- context manager
- `__exit__`- context manager

## Iterators

- Iterators provide a sequence interface to Python objects that’s memory efficient
- `__iter__` - iterator object
- `__next__` - retrieves next value from an iterator
- One way to write iterable objects

## Generators

```PY
def bounded_repeater(value, max_repeats):
    for i in range(max_repeats):
        yield value
```

- The `yield` statement allows you to temporarily suspend execution of a generator function and to pass back values from it.

# Useful Links

- [Dunder-methods](https://dbader.org/blog/python-dunder-methods)
- [Generators](https://dbader.org/blog/python-generators)
- [Iterators](https://dbader.org/blog/python-iterators)