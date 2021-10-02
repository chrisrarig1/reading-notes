# Putting it all together

## Thinking in React

1. What is the single responsibility principle and how does it apply to components?

    - A component should ideally only do one thing. This principle allows a components to only be responsible for doing one thing and if the component ends up getting larger it should be split into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

    - A **Static** version does not allow for interactivity.The data does not change therefore *state* is not allowed to be used.

3. Once you have a static application, what do you need to add?

    - We need to add a *minimal set of mutable state*

4. What are the three questions you can ask to determine if something is state?

    - Is it passed in from a parent via props? If so, it probably isn’t state.
    - Does it remain unchanged over time? If so, it probably isn’t state.
    - Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. How can you identify where state needs to live?

    - By following these steps.
        1. Identify every component that renders something based on that state.
        2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
        3. Either the common owner or another component higher up in the hierarchy should own the state.
        4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

1. What is a “higher-order function”?

    - Functions that operate on other functions, either by taking them as arguments or by returning them

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

    - It is passing the argument of numbers into the function *m* and returning a **boolean** based on if argument *m* is greater than argument *n*

3. Explain how either map or reduce operates, with regards to higher-order functions.

    - *Map*: changes an array by applying a function to all od its elements and building a new array.
    - *Reduce*: builds a value by repeatedly taking a single element from the array and combining it with the current value.

## Things I want to know more about

- I would like to see the development process for a *Static App* in action

# Useful Links

- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
- [Higher Order](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)