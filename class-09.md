# Forms & JS Events

## Forms

- A **Form** allows you to attain information from the viewer through their inputs. I.E. Yahoo or Google

- One can display their **forms** in multiple ways **Adding Text**, **Making Choices**, **Submitting Forms**, and **Uploading Files**
  - **Adding Text**: Text Input, Password Input, and Text Area
  - **Making Choices**: Radio Buttons, Checkboxes, and Drop-down boxes
  - **Submitting Forms**: Submit Buttons and Image Buttons
  - **Uploading Files**: File Upload

### How A Form Works

1. A viewer inputs the information they want and then selects a button in the form box to submit that information
2. The information is then uploaded to websites server for processing
3. The server process the information
4. The server creates an alert, prompt, or new page to respond to the submission

### How To Write A Form

- To start off a form we designate it with the `<form>` tag. Inside the `<form>` tag it is required to put an **Action** `action="www.server.com"` and a **Method** `method="get"`. The **Action** tag is a URL input while the **Method** tag is either `"get"` or `"push"`.

## Lists, Tables, and Forms

- There are multiple **CSS** methods that allow for the user to affect specific kinds of tables, lists, and forms

- Using `list-style` properties allows you to add design to your list or remove the default style. You can change the bullet style to a numbered system or a shape system. There are even options to change the positioning of the second line of a list item `list-style-position=`. Using this it can allow for more of a free flowing look to your list or an ordered look.

- **Tables** can also be updated specifically using **CSS**. One can adjust spacing or styling on a specific table using basic **CSS** properties that are used on ordinary **HTML** elements. This where it is possible to adapt your table giving it more flexibility when it comes to browser conformity.

- **Forms** using **CSS** one can give the form boxes a little more flare an show importance. It is wise to align the form properties in a vertical way. This make sit easier for the user to view.

## Events

- **Events** are a cause and effect action. Hey the user did this so the website will respond with this. An event can be described as something as small as a screen scroll. Certain events can even trigger a **JavaScript** function
- **Binding** this is where you can designate which **Event** you are waiting for to happen and what **Element** your expecting to happen on. This gives you the ability to be specific so the entire page isn't susceptible to triggering the **Event**
- **Event Delegation** allows you to monitor **Events** to ensure they are happening at teh appropriate moment and functioning properly

### Form Events

- There are three events that take place when a user is attempting a form response *Submit*, *Change*, and *Input*
  - **Submit**: Clicking submit can cause a JavaScript function or statement to fire up and compare or evaluate the input.
  - **Change**: This happens when the user changes for elements
    - A selection was made from a drop down
    - A button was selected
    - A checkbox was updated
  - **Input**: When the input box is updated with the viewers response or input.

# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley, 2011.
- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.

# Useful Links

- [Events](https://www.w3schools.com/js/js_events.asp)
- [Styling Tables](https://www.w3schools.com/css/css_table.asp)