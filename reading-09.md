# Functional Programming

1. What is functional programming?

    - It is a style of building the structure and elements of a program using mathematical functions while avoiding changes in state and mutable data

2. What is a pure function and how do we know if something is a pure function?

    - A pure function returns the same result if given the same arguments
    - The function does not use any external object

3. What are the benefits of a pure function?

    - They are stable, consistent,predictable, and easier to test

4. What is immutability?

    - Unchanging over time or unable to be changed

5. What is Referential transparency?

    - If a function consistently yields the same result for the same input.

# Modules and Require()

1. What is a module?

    - A module is a section of code that deals with a specific action.

2. What does the word ‘require’ do?

    - It will include external modules that exist in separate files

3. How do we bring another module into the file the we are working in?

    - `var name = require('./filename')`

4. What do we have to do to make a module available?

    - By setting `module.exports = var name` to the things we want available

## Things I want to know more about

- The proper organization of our JS files

# Useful Links

- [Functional-Programming](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
- [Node/Require](https://www.youtube.com/watch?v=xHLd36QoS4k)