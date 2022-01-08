# Game of Greed 4

## Dunder Methods

- These are a set of predefined methods.

- They let you emulate the behavior of built in functions.
- **__init__**:
  - Takes care of setting up the object.
- **__str__**:
  - This gives us a nicely printed representation of an object
- **__repr__**:
  - The official string representation of an object
- **__len__**:
  - This method allows you to avoid the return of an error and makes a class iterable
  - `def __len__(self):`
        `return len(self_transactions)`
- **__getitem__**:
  - This method allows you to return certain items.
  - `def __getitem__(self, position):`
        `return self._transactions[position]`
- **__reversed__**:
  - Allows you to reverse the items in the class
  - `def __reversed__(self):`
    `return self[::-1]`
- **__eq__**:
  - Allows you to compare values
  - `def __eq__(self, other):`
        `return self.balance == other.balance`
- **__lt__**:
  - Allows you to compare values
  - `def __lt__(self, other):`
        `return self.balance < other.balance`
- **__add__**:
  - A method to add values to the class
- **__call__**:
  - This allows you to use a print function while iterating through a class

## Probability

- What are the chances of an event happening?
- **Event**: is the outcome of interest
- **Sample Space**: The set of all possible outcomes
- **Normal Distribution**: The distribution of many random variables as a bell-shaped graph
- **Central Limit Theorem**: The more trials the more the average approaches true probability
- **Three Sigma Rule**: How many observations fall within a certain distance of the mean.
- **Z-score**: How many standard deviations away from the mean is the data
  - `zscore = (point - mean)/standard deviation`

# Useful Links

- [Dunder Method](https://dbader.org/blog/python-dunder-methods)
- [Probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)