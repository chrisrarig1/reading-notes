# HTML Text, CSS Intro, and Basic JavaScript

## HTML Structure Text

- When using text in **HTML** it is required to use tags to allow for structure of your content. Some of these tags will also allow you to format your text to appear more proper on your page. The list below are some examples of **Structure** tags

    - `<h1>,<h2>,<h3>...` Headings listed by priority
    - `<p>` Paragraph designation
    - `<b>` Bold text
    - `<i>` Italic text
    - `<sup>` Superscript
    - `<sub>` Subscript
    - `<br />` Line breaks
    - `<hr />` Horizontal rules

## HTML Semantic

- This type of **HTML** text is not intended to affect the structure of the content, but add emphasis and info to the text. The list below are examples of **Semantic** text
    - `<strong>` Strong emphasis on the word will show BOLD
    - `<em>`Emphasis on a word that changes context of content shows ITALIC
    - `<blockquote>` Used for longer quotes longer than one paragraph
    - `<q>` Used for shorter quotes
    - `<abbr>` abbreviates the word
    - `<cite>` Used for in paragraph citations
    - `<dfn>` Defining terms
    - `<address>` Used for specific author info
    - `<ins>` A indicator for new content added
    - `<del>` Content deleted
    - `<s>` Strike-through

- Using these tags allows you to promote structure and emphasis throughout your content and makes for a easier read for the viewer.

## CSS

- *CSS* Cascading Style Sheets gives your style. As explained in Code 102 it is the interior designer of your web page.

- There are multiple ways to introduce your **CSS** code to your **HTML** code. In our first lab we used the *Internal* method. The other method is having a *External* sheet.

    - **External** requires a `<link>` to reference your **CSS** sheet and tell your **HTML** where to find the sheet and what its relation to the code it has. **I.E**

    `<link rel="stylesheet" href="style.css">`

    - **Internal** requires a `<style>` tag which can be included in the Head section of your **HTML** code. You can also insert a `style=" "` inside a tag if you only want the changes to apply specifically to that tag. **I.E**

        - **Head**:
            `<head>`
            `<style>`
            `h2{color: blue;} </style> </head>`

        - **Inside Tag**
            `<footer style="background-color:red;">`

- While using **CSS** you can identify certain pieces of content that you want to update using selectors. Some common selectors are `* ()` which selects all elements on the page and `h1 h2 h3 ()` which selects the elements with matching tags. Identifying these elements allows the user to format anything from font, color, and much more. However, it is important to remember that **CSS** rules cascade.

## Basic JavaScript

- **JavaScript** allows for interaction with the viewer. It puts the final coat of pain on your website.

- Using certain text formats (Boolean, Strings, Numbers) **JavaScript** allows for *variable* declaration. Those variables are considered as temporary place holders for information.

    - Variable (time) declaration:

        - `let time = new Date().getHours(); `

### Decisions and Loops

- **Decisions** can be in many forms through **JavaScript**. *Conditional* Statements (if/else statements), and *Switch* statements are a few. Below are examples of some decision statements:
    
    - if/else:

        `if (name = Chris) { document.write("Hi Chris");}`
        `else{ document.write("Please leave")}`

    - In this if/else statement we have two responses to the value of the variable `name`. If the variable equals Chris we will get the response "Hi Chris"and if not we will get the response please leave.

- **Loops** are functions that will continuously run until a condition is met.There are three kinds of loops: for, while and do...while. The example below is a for loop.

    - `function hrsplayed(){let howmany = prompt ('How many hrs a week do you play video games?');`
    `for(let ii=0;ii< howmany; ii++){` 
    `document.write(<img class="boo">)}}`

- In this statement the function runs until it equals the answer of the `howmany` prompt generating an image each time it runs.

# Useful Links

- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [HTML BASICS](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
- [W3Schools: Add CSS](https://www.w3schools.com/css/css_howto.asp)


# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley, 2011.
- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.