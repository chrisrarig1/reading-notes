# Problem Domain, Object Literals, and Document Object Model

## Problem Domain

- Understanding the problem or problem domain in which you are try correct by coding is essential to make the process smoother for you, but also to write better code.
- Narrowing the focus of your problem to just one particular instance will help clarify and simplify that problem.
- John Sonmez uses a great example in his article. Video games!!! Each level has a problem domain and starts small and gets more difficult the farther you go.
- Remember these two points:
    1. Make the problem easier to understand
    2. Just understand problem domains better.

## Object Literals

- **Objects** are labeled as variables, but are groups of functions and variables. In **Objects** `var dogs =` functions become known as **Methods** `timetoplay` and variables become known as **Properties** `name,toy,food`

```js
    
    var dogs = {
        name : Lana,
        toy : Bone,
        food : Iams,
        favoritetoy : Ball,
        timetoplay: function(){
            return timeofday;
        }
```

- To access anything from an object throughout your code you can call it using `Object_Name.property_or_method;`.