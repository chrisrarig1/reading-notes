# HTML Lists, CSS Box Model, and JS Control Flow

## HTML Lists

- There are 3 different types of lists:
    1. **Ordered Lists**
        - Tags: `<ol>` `<li>` `</li>` `</ol>`
        - The list items are numbered
    2. **Unordered Lists**
        - Tags: `<ul>` `<li>` `</li>` `</ul>`
        - These lists involve bullet points that show no order
    3. **Definition Lists**
        - Tags: `<d1>` `<dt>`(contains term)`</dt>` `<dd>`(contains definition)`</dd>``</d1>`
        - Used for terms and definitions
- Lists can be nested and definitely make formatting very easy.

## Boxes

- When determining how **HTML** is viewed by **CSS** it is important to remember that according to **CSS** everything is in a box. We can control the formats of these boxes by adjusting their dimensions like width and height. Coding example below:
  - Width: `width: 50px` `min-width: 50px` `max-width: 50px`
  - Height: `height: 50px` `min-height: 50px` `max-height: 50px`

- The boxes can also receive formatting themselves through borders, padding, and margins
![boxes](https://miro.medium.com/max/565/1*6DrszcyPybYDGziiS9CWdg.png)

## Switch

- **Switch** are statements that allow you to take a value and run it through cases. If the value matches that case then the code block associated with that case runs. If none of the cases equal the value then a default code block will run. Code example below:
  - `let set = 3`
  `switch(set)`
  `case 1: msg = 'Nope'; break;`
  `case 2: msg = 'Not yet'; break;`
  `case 3: msg = 'This one runs!!'; break;`
  `default: msg = 'None of the above equal set'; break;`

## Loops

- **Loops** are for statements that will run continuously until a certain condition is met. There are 3 kinds of loops for, while, and do while.
  - **For**: This is used if you need the code run a known number of times
    - `for(let ii=0;ii< howmany; ii++){ document.write();}`
      - (declare variable,set condition,what happens after iteration)
  - **While**: This is used when the number of times needed to run is unknown
    - `while (x < 25) { document.write();}`
      - Runs while(condition) is true
  - **Do While**: Similar to the **While** statement, but runs the statement prior to condition test
    - `do{ document.write();} while (x<25))`
      - The statement is printed while condition `x<25` is met

# Useful Links

- [JavaScript](https://www.w3schools.com/js/js_loop_for.asp)
- [CSS Box Model](https://www.w3schools.com/css/css_boxmodel.asp)

# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley, 2011.
- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.