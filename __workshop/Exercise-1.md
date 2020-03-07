# Questions

**With a partner**, answer these questions as completely as possible. Feel free to look at past lecture notes, the web, anything. 

Take the time to explain it to each other. 

The power of this exercise is in the act of _formulating_ and _explaining_ the concepts to someone else (your teammate).

## One

Run the app. Write out the steps, the _pseudo code_, required to create this app. It doesn't have to be totally accurate, or in the right order.

Only move on to the next question when you have enough detail that you would be able to start coding it yourself.

```js
// Answer here
//set header with title
//set div with input bar 
//setup function to display in todo on button press
//possibly an array being displayed in a list with forEach
//display it as a list item in a div inside the todo list
//fix bugs
```

## Two - `server.js`

Take a look at the `server.js` file.

We have a new module in there, `body-parser` that is required on line `4`. What is it for? What is its use-case? What other lines are related to this module?

_The NPM site might be a good place to start. Feel free to provide links as relevant._

```js
// Answer here
//body-parser parses information in a string to verify if the information is legitimate by comparing it to a database

// RELATED LINES: 
//line 18
//line 24

//https://www.npmjs.com/package/body-parser

//https://www.google.com/search?q=parse&rlz=1C1CHBF_enCA878CA878&oq=parse&aqs=chrome..69i57j35i39l2j0l3j69i60l2.594j0j7&sourceid=chrome&ie=UTF-8
```

## Three - `server.js`

Look at lines `23` and `24`. Explain the methods used. How are they different? What are the usecases for each?

```js
// Answer here
//line 24 post method grabs the user input through the req.body parsing and assigns it to a constant item, which is pushed into the items array which is then rendered in the homepage and displayed through a forEach. 
//line 23 just renders the homepage
```

## Four - `server.js`

Line `6`. That's new. What do you think it's for?

```js
// Answer here
//assigns the functions from handlers.js into the server. Prevents server side coding
```

## Five - `handlers.js`

Explain line `1`. Where, why and how is `items` being used?

```js
// Answer here
//items is being used in handleFormData to update the array of items of the todo list.
//items is also being used in handleHomePage to render the items array into the homepage through the forEach loop
```

## Six - `handlers.js`

Why is there `redirect` on line `11`;

```js
// Answer here
//the redirect updates the homepage with the current value of the items array
``` 

## Seven - `handlers.js`

The `handle404` function is a more complex than we've seen thus far, what is the extra functionality for?

```js
// Answer here
//if the html is faulty it goes back to a default
```

## Eight - `ejs`

Take a look at `homepage.ejs` and `todoInput.ejs`. What is happening in there? Explain line-by-line...

```js
// Answer here
//1. inputs the header
//2. creates a div that contains the todo input
//3. inputs todo
    //1. calls the post method
    //2. labels the input bar with an action that calls the /form-data page
    //3. provides an input bar
    //4. provides with a button
    //5. closes the form
// 4. closes the div
// 5. creates a div that contains the todo list
// 6. creates an unorganized list for the todo list
// 7. starts a forEach loop for the items array
// 8. outputs every item in  the items array as a list item
// 9. closes the forEach loop
// 10. closes the ul
// 11. closes the div that contains the todo list
// 12. inputs the footer
```

## Nine - `styles.scss`

What are lines `2` to `7` for this file? Where are these values being used? Take a look at `_homepage.scss` as well? What do you notice?

```js
// Answer here
//lines 2 to 7 are scss variables
//those variables are used in the _homepage.scss
```

## Ten - `_homepage.scss`

Line `16`. See if by searching the Sass documentation, you can determine what _exactly_ is going on here. That `#{}` notation very specific to this use-case. Why?

```js
// Answer here
//converts the value inside the curly brackets into a number for the calc method
```