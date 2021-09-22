# States and Props

1. Based on the diagram **render** happens before **componentDidMount**
2. The **Mounting** phase is the first phase in the *React* life cycle. It includes Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount.
3. Constructor -> render -> React Updates -> componentDidMount -> componentWillUnmount
4. componentDidMount-This is called upon to execute the *REACT* code when the component is already placed in the *DOM*

## React State Vs Props

1. What types of things can you pass in the props?
    - You can pass arguments you would use in a function

2. What is the big difference between props and state?
    - Props are passed into a component and state is handled inside a component. Props are dealt with outside.
3. When do we re-render our application?
    - When we change the state inside a component
4. What are some examples of things that we could store in state?
    - Anything that can or will be updated by the user. Text, numbers, counters, or titles.

# Useful Links

- [React](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
- [State vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)