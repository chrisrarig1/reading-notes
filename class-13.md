# Local Storage

## Cookies!!!

- Cookies were created to store small amounts of data but have a downside:
    1. They slow down your app
    2. They send unencrypted data over the internet
    3. They are limited in size

- These limitations do not help when a website requires large amounts of data that will not disappear when the website is refreshed.

## HTML5 Storage

- **HTML5** is a method of storing key value pairs locally. This allows for the data to remain present even after the application is closed. However this data is never transmitted therefore more secure.

- To check if your current app is using **HTML5** storage one can write a simple function to verify:
    `function supports_html5_storage() {`
  `try {`
    `return 'localStorage' in window && window['localStorage'] !== null;`
  `} catch (e) {`
  `return false;`
  `}`
`}`

## Using HTML5 Storage

- Data is stored in **HTML5** using a named key. The data can be anything supported by *JS*. The format of the stored data however is not that of a string. Due to this a `pareInt()` or `parseFloat()` is required.

- You can treat Local Storage like an array. Using `getItem()` and `setItem()` is the generalized way of access items but one can get rid of these terms and use `[]` i.e.:
    `let data = localStorage.getItem("a");`
    `// ...`
    `localStorage.setItem("a", data);`
can translate to:
    `let data = localStorage["a"];`
    `// ...`
    `localStorage["a"] = data;`

- To clear the storage area use:
    `interface Storage{`
        `deleter void removeItem(in DOMString key);`
        `void clear();`
    `}`
- To return the total number of values in storage one can iterate through the storage similar to an array.
    `interface Storage {`
        `readonly attribute unsigned long length;`
        `getter DOMString key(in unsigned long index);`
    `}`

## Storage In Action

- In the example given to us in the reading it shows how changes or movements in a game are saved. Every time a change occurs in a game a function is called that a iterates through a set of data saving the data of importance i.e.

`for (var i = 0; i < kNumPieces; i++) {`
`localStorage["halma.piece." + i + ".row"] = gPieces[i].row;`
`localStorage["halma.piece." + i + ".column"] = gPieces[i].column;`
    `}`

# Useful Links

- [THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS](http://diveinto.html5doctor.com/storage.html)