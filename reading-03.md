# Passing Functions as Props

## Lists and Keys

1. What does .map() return?

    - Its returns a new array.

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    - You can loop through an array using the **map()** function and then include them in *JSX* using curly braces.

3. Each list item needs a unique ____.

    - *Key* or string

4. What is the purpose of a key?

    - A *Key* helps React identify which items have been changed, added, or removed

## Spread Operator

1. What is the spread operator?

    - It is **...** that allows you to expand an iterable object into a list of arguments

2. List 4 things that the spread operator can do.

    - Add items to and array, combine arrays or objects, and spreading an array out into a function's arguments

3. Give an example of using the spread operator to combine two arrays.

```js
{
    let array = [1,2,3];
    let array2 = [4,5,6];
    arr = [...array,...array2];
    [1,2,3,4,5,6]
}
```

4. Give an example of using the spread operator to add a new item to an array.

```js
{
    let array =[1,2,3];
    let array2 =[4];
    array.push(...array2)
}
```

5. Give an example of using the spread operator to combine two objects into one.

```js
{
    let array ={hi:"Bob"}
    let array2 = {bye:"Ted"}
    let array3 = {...array,...array2}
}
```

## Passing Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?

    - The developer creates the function that loops through the object and the function is located in the object code

2. In your own words, what does the increment function do?

    - It loops through the object array and finds the index based on the given name and then updates that object and passing the array into a new array

3. How can you pass a method from a parent component into a child component?

    - By passing it just like any other prop. Adding it to the parent component then you can call it using this.props

4. How does the child component invoke a method that was passed to it from a parent component?

    - By calling it like a typical function using this.props.

## Things I want to know more about

- I would like to see and know more about how much this can be utilized

# Useful Links

- [How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)
- [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
- [Spread Operators](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)