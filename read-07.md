# Python Scope

## LEGB Rule

- *Local*: Python scope that contains the names that you define inside a function. Created at the call of the function
- *Enclosing*: is a scope only used for nested functions. This contains the names your define in the enclosing function
- *Global*: Anything you define at the top of your code. Can be used throughout your code
- *Built-in scope*: Scope that is created or loaded whenever the code script is ran or an interactive session is started.

## Global and Nonlocal

- *Global statement*: This statement allows you to define a list of names that can be treated as global names
  - Code:`global name`

- *Nonlocal statement*: These allow non-local names to be modified 
  - Code: `nonlocal var`

## Big O Notation

- Deals with time and space complexity
- *Time*:Basically how long an algorithm takes to run
- *Space*: How much memory is required
- Used to compare algorithms when throwing a lot of data at it
- Allows you to see the efficiency of an algorithm and gives you an idea of whether or not you need to reevaluate your algorithm
- Worst case scenario
- *Big O Notation*
  - O[1]: Constant run time
  - O[log n]: Log run time
  - O[n]: Linear run time
  - O[n logn]: Log-Lin run time
  - O[n^k]: Poly run time

# Useful Links

- [Big O](https://www.youtube.com/watch?v=5Uqawfl0VHQ)
- [Scope](https://realpython.com/python-scope-legb-rule/#using-scope-related-built-in-functions)