# Debugging

## Order of Execution

- It is vital to understand how a code executes in order to understand where a bug could occur. Most code does not execute top to bottom as written. A function may be written at the top of the page and not execute until it is called.

- JavaScript uses **Stacks** to read or hold certain lines of code that is dependent on others. You can visualize this as a waiting cue. As shown in the visual below.
![Stacks](https://miro.medium.com/max/1400/0*ryPdDzB_jghiVi2e.png)

As you can see the *main* part of the code is being pushed down the run que due to being dependent on the results of *first* and *second*.

## Error Objects

- When an error occurs an object is created with certain properties:
  - **Name**: The type of error. There are 7
    1. **Error**- Generic error
    2. **SytnaxError**- Syntax is incorrect
    3. **ReferenceError**- Ref of a variable is not declared or within scope
    4. **TypeError**- An unexpected data type
    5. **RangeError**- Numbers not in acceptable range
    6. **URIError**- `encodeURI()`, `decodeURI()` or similar used incorrectly
    7. **EvalError**- `eval()` function used incorrectly
  - **Message**: Description of the error.
  - **File Number**: Name of the JS file.
  - **Line Number**: Line number of error.

## Debugging Workflow

### Where

- Where is the problem:
  1. View the error message for file and line number
  2. Using `console.log()` to show how far your code is running
  3. Use breakpoints to pause code to isolate the problem

### What

- What is the problem:
  1. Using breakpoints will allow you to view the code around the problem area to see if all variables have the correct expression or values
  2. Break your code up into smaller pieces and test using scenarios or `console.log()` to view values
  3. Check that parameters are set correctly or indexes of arrays are at the correct count.

- Using dev tools available in your browser is also an easy way to find errors and error messages while viewing your page
- All in all debugging requires the art of deduction.

# Useful Links

- [JavaScript Debugging](https://www.w3schools.com/js/js_debugging.asp)

# Useful Readings

- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.