# Object-Oriented Programming and HTML Tables

## Tables

- An **HTML Table** is a table that shows information in a grid format.
- Basic table structure consist of the tags `<table>`, `<tr>`, `<td>`, and `<th>`
  - `<table>`: This is used to create a table.
  - `<tr>`: This is used to start each row.
  - `<td>`: This is used to input the cell data.
  - `<th>`: This tag is to display the heading of the table.
- Long tables can be split into `<thead>`, and `<tbody>`, and `<tfoot>` similar to **HTML** format.

## Objects

- **Constructor Notation**: This a different form of an **Object Literal** in which a function is generated with place holders for those same properties described in the **Object Literal**. Code example below:

```js
  function Dog(name,toy,age) {
      this.name = name;
      this.toy = toy;
      this.age = age;
  }
```

- To update a **Constructor Notation** you use the *new* tag while creating a new variable. I.E.

```js
    let dog2 = new dog ('Lana', 'Ball', 4);
```

- Using **DOMS** you can use the above **HTML** tables coding to create a table using the data from you **Constructor Notation**

# Useful Readings

- Duckett, Jon. HTML & CSS: Design and Build Web Sites. Wiley, 2011.
- Duckett, Jon. JAVASCRIPT & JQUERY: Interactive Front-End Web Development. Wiley, 2014.