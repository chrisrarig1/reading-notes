# React 1

- Hello World: `ReactDOM`
  `.createRoot(document.getElementById('root'))`
  `.render(<h1>Hello, world!</h1>);` 

## JSX

- JSX is a syntax extension to JavaScript
- *Embedding Expressions*:
`const name = 'Josh Perez';`
`const element = <h1>Hello, {name}</h1>;`
- *Embedding Functions*:

```JS
function formatName(user) {
  return user.firstName + ' ' + user.lastName;
}

const user = {
  firstName: 'Harper',
  lastName: 'Perez'
}

const element = (
  <h1>
    Hello, {formatName(user)}!
  </h1>
)
```

- *Rendering Elements*:
  - `const element = <h1>Hello, world</h1>;`
  - `root.render(element);`
- *Updating a Rendered Element*:

```JS
const root = ReactDOM.createRoot(
  document.getElementById('root')
);

function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  root.render(element);
}

setInterval(tick, 1000);
```

## Components and Props

- *Class Props*:

```JS
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

- *Function Props*

```JS
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

## State

```JS
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = {date: new Date()};
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}
```

- Passing Props:

```JS
  constructor(props) {
    super(props);
    this.state = {date: new Date()};
  }
```

- Data flows down from parent component to child

## Handling Events

- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.

```JS
<button onClick={activateLasers}>
  Activate Lasers
</button>
```

- Handling a Click:

```JS
class LoggingButton extends React.Component {
  handleClick() {
    console.log('this is:', this);
  }

  render() {
    // This syntax ensures `this` is bound within handleClick
    return (
      <button onClick={() => this.handleClick()}>
        Click me
      </button>
    );
  }
}
```

- Passing Arguments:
  - `<button onClick={(e) => this.deleteRow(id, e)}>Delete Row</button>`
  - `<button onClick={this.deleteRow.bind(this, id)}>Delete Row</button>`

## CSS

- [Utility First CSS](https://tailwindcss.com/docs/utility-first)

## Next.js

- [Learn Next.js](https://nextjs.org/learn/basics/create-nextjs-app)
- [Why I’m Using Next.js in 2020](https://www.youtube.com/watch?v=rtgbaKBhdkk)