# Game of Greed 1

## How to use Random Module

- The random module allows access to a number of functions but the one we are focusing on is the random number generator
- The random number generator is a good tool to use when you need to pick a random element from a list, a random number for a game or even generating a password for a website

- *Randint*: This generates a random integer. It accepts two integer arguments and generates a integer between them.
Code: `import random`
        `print random.randint(0,5)`
        `possible outputs -> 1,2,3,4,5`

- *Random*: to generate a larger number you multiply it.
Code: ` import random`
        `random.random() * 100`
        `possible outputs -> 1-100`

- *Choice*: Generates random value from a list
Code: `import random`
        `myList= [2,3,red,black]`
        `random.choice(myList)`

- *Shuffle*: shuffle the order of the elements in a list
Code: `from random import shuffle`
        `x = [[i] for i in range(10)]`
        `shuffle(x)`
        `print(x)`

- *Randrange*: random generator based on start, stop, and step arguments
Code: `random.randrange(start, stop[, step])`
        `import random`
        `for i in range(3):`
            `print random.randrange(0,70,5)`

## Risk Analysis

- *Risk*: the probability of any unwanted incident
- Using Risk Analysis allows for a plan to be generated so that problems can be taken into consideration while generating software
- Risk Analysis does have some faults:
  - Could take more time than given
  - Defect leakage
- *Risk Assessment*:
  - **Effect**: determine the impact
  - **Cause**: determine what causes the problem
  - **Likelihood**: the occurrence of the risk 
- *How to Perform Risk Analysis*
  1. Searching the risk
  2. Analyzing the impact of each individual risk
  3. Measures for the risk identified

## Test Coverage

- Test coverage is a great tool for finding untested code but the quality of the test may be lacking
- High coverage usually falls to low testing quality
- TDD should allow for 80-90 percent coverage
- It is possible to test too much. One sign is that your tests are slowing down
- Coverage tools are a great way to see which pieces of code are not being tested

## Big O Notation

- Internet transfer time is O of n. it scales linearly with respect to the amount of data
- O(n) is adjusted based on the amount of times require to iterate through a list:
  - O(n^2): runs through the list twice
- Rules:
    1. if you have 2 different steps in your algorithm you add them up
      - O(a) + O(b)
    2. Drop constants
      - when you have two O(n) sub-functions in a Algorithm the total function = O(n) not O(2n)
    3. Different inputs -> Different variables
      - If you input is two arrays you describe how long it takes to run through those arrays. O(array1 * array2)
    4. Drop non dominate terms
      - If you have a Algorithm with two functions one with O(n) and the other with O(n^2). Since the O(n^2) is dominate you drop the O(n)

# Useful Links

- [Big O](https://www.youtube.com/watch?v=v4cd1O4zkGw)
- [Random](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)