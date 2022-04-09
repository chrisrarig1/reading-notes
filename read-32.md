# React 2

## Conditional Rendering

- Inline If with Logical && Operator:
  - `{unreadMessages.length > 0 &&`
        `<h2>`
         `You have {unreadMessages.length} unread messages.`
        `</h2>`
      `}`

- Inline If-Else with Conditional Operator:
  - condition ? true : false:
    - `The user is <b>{isLoggedIn ? 'currently' : 'not'}</b> logged in`

- Preventing Component from Rendering
  - This can be done by using a Boolean variable and setting a conditional statement which allows the element to render if true and not if false

## Lists and Keys

- `map()`: this function iterates through an array returning a new array.
- This function can be used to iterate through an array and will render multiple components
- `const listItems = numbers.map((number) =>`
  `<li>{number}</li>`
`);`
- Then we can all this function in the parent element:
  `<ul>{listItems}</ul>`

### Keys

- Keys help React identify which items have changed, are added, or are removed
- `<li key={number.toString()}>`
- Most often you would use IDs from your data as keys
- `<li key={todo.id}>`

## Forms

```HTML
<form>
  <label>
    Name:
    <input type="text" name="name" />
  </label>
  <input type="submit" value="Submit" />
</form>
```

- We can store the data from the form by altering or setting state
- `handleChange(event) {`
    `this.setState({value: event.target.value});`
  `}`
- Then we would include the functions in the HTML
- `<form onSubmit={this.handleSubmit}>`
- `<input type="text" value={this.state.value} onChange={this.handleChange} />`

### Handling Multiple Inputs

- This can be done by assigning a name to the input tags:
  - `<input name='ave' type='number'/>`

## Composition vs Inheritance

### Containment

- `{props.children}`: this lets other components pass arbitrary children to them by nesting JSX

## Thinking In React

1. Break The UI Into A Component Hierarchy
2. Build A Static Version in React
3. Identify The Minimal (but complete) Representation Of UI State
4. Identify Where Your State Should Live
5. Add Inverse Data Flow

# Useful Links

- [React Docs](https://reactjs.org/docs/getting-started.html)
