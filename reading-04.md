# React and Forms

## Forms

1. What is a ‘Controlled Component’?

    - A input form element whose value is controlled by React through the combination of maintaining a state and updating it based on user input

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

    - We have to update the state when they enter them. The handle change runs on every keystroke

3. How do we target what the user is entering if we have an event handler on an input field?

    - Setting the state using event.target.value. This happens when the handleChange runs.

## Conditional Ternary

1. Why would we use a ternary operator?

    - To shorten your **if** statement into one line of code

2. Rewrite the following statement using a ternary statement:

```js
   {x.ternary = x === y ? 'true' : 'false';}
```

## Things I want to know more about

- How we are planning on implementing the form to our projects

# Useful Links

- [Ternary](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
- [Forms](https://reactjs.org/docs/forms.html)