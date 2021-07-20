# HTML Links, CSS Layout,and JS Functions

## HTML Links

- When creating your page it can be handy to allow navigation to other pages or resources for your user. It is possible to achieve this through the use of `<a>` **Anchor** tags. Code example below:

  - `<a href="website_url.com"> Title Shown on your page </a>`

- Using the anchor tag can also allow a person to link an **Email** `mailto:` or another page on the same website. When creating a link to another website using the **Target** `target="_blank` attribute allows a new window to open instead of forcing the viewer to leave your site.

## CSS Layout

### Boxes

- There are two different types of boxes in which your content is considered. A **Inline-Box** or a **Block-Level Box**

  - **Inline-Box**: `<img>,<p>,<ul>,<li>` pushes the text between the other text on the page.
  - **Block-Level Box**: `<h1>,<p>,<ul>,<li>`This starts a new line for the text and acts as a building block for the page.

- When using a **Block-Level** element it is possible and common to put other elements inside the box.

### Positioning

- **Positioning Schemes** allow you to control the flow and position of your content on the web page. There are five main **Positioning Schemes**

  - **Normal Flow**: Each block element generates a new line and the content flows done vertically.
  - **Relative**: This shifts content in a different direction away from its normal flow position while not affecting the other content.
  - **Absolute**: This positions the content in relation to the content inside of it.
  - **Fixed**: This decides the position of the content or element based on the browser window.
  - **Floating**: This allows the element to flow around the surrounding content.

## JS Functions

- *Functions* are statements that perform assigned tasks or generate values.
- A *Function* is made up of four parts:
    1. The name of the function
    2. The parameters of the function
    3. The JavaScript that the function performs
    4. The return
- Here is a example we used in 102:
  - `function getname(){`
    `let name = prompt('What is your name?');`
    `return name;}`
  - In order for this to run we would need to call the function like so:
    `getname();`

- It is possible to return more than one value returned from a function using an information array like so:
    `getfuncname(1,2,3,4)[1];`
- You can use/call a function as many times as you want.
- Less coding in the long run if you wanted to use that JavaScript inside the function multiple times.

# Useful Links

- [JavaScript](https://www.w3schools.com/js/js_functions.asp)
- [HTML Links](https://www.w3schools.com/html/html_links.asp)
- [CSS Position](https://www.w3schools.com/css/css_positioning.asp)


# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley, 2011.
- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.