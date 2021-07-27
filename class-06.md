# Problem Domain, Object Literals, and Document Object Model

## Problem Domain

- Understanding the problem or problem domain in which you are try correct by coding is essential to make the process smoother for you, but also to write better code.
- Narrowing the focus of your problem to just one particular instance will help clarify and simplify that problem.
- John Sonmez (Sonmez) uses a great example in his article. Video games!!! Each level has a problem domain and starts small and gets more difficult the farther you go.
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

## Document Object Model

- A **DOM** is a web browser generated picture of the structure of the websites information with four types of nodes.
    1. **Document Node**: Describes the entire page
    2. **Element Node**: These are the **HTML** that develop the structure of the page.
    3. **Attribute Nodes**: These are the styles inside of opening **HTML** tags
    4. **Text Nodes**: Text generated inside the elements
- Accessing parts of the **DOM** can be done by specifying the **Object** and **Method** i.e. `document.getElementById('car')`. This can also be done using `.getElementByTagName` and `.querySelectorAll`.
- It is also possible to access **Attributes** once you have access to **Method**. i.e. `document.getElementById('car').getAttribute('color')`

### Looping Nodes

- You can loop through each node on a node list and apply certain changes to each item. This is similar to what we have been doing in recent labs with arrays. By stating the node length in `i < var.length;` this will ensure all nodes within the node list will be altered.

### Altering HTML

- It is possible using the **DOM** method to alter HTML content. Other methods include `document.write()` and `element.innerHTML`

# Useful Links

- [Problem Domains](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)
- [DOM](https://www.w3schools.com/js/js_htmldom.asp)

# Useful Readings

- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.
- Sonmez, John. “Understanding the Problem Domain Is the Hardest Part of Programming.” Simple Programmer, Simple Programmer, 28 Jan. 2018, simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming. 