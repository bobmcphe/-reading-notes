# Class 07

## Ch. 6 - Tables
Because a lot of information that exists needs to be organized and structured in a grid, the `<table>` tag allows for this. Naturally, grids (or tables), have rows and columns. These two entities intersect to form 'cells.' Just like MS Excel, you can make a cell span more than one column or row, using the `<colspan>` or `<rowspan>` respectively. Further, tables that are remarkably long can be divded up for ease of use. 

## Ch. 3 - Objects - Constructor Notation
The constructor notation version of creating an object is great for saving memory, and also time if there will be a lot of similar objects being created. This section also covers updating an object, which can use either the dot notation, or the bracket notation. Most common will be the dot notation. Both can create a new property if it does not exist. We can also delete a property using these notations, by simply typing `delete` in front of the line of code(e.g. `delete hotel.name;`).

When we need to instantiate a new object using the constructor function, it is required that we use the `new` code to do so. Within functions, the `this`  is a contextual peice of code that always references the object. When a function is written inside of an object, it is called a method. 

Name/Value Pairs
Javascript understands the data in name/value pairs. For example, a variable will have a name and only one value, e.g. `var X = 12`. 
But objects are like complex variables, and so they store multiple name/value pairs, either properties or methods. This can get a bit complicated, in fact, since an array can include an object, and objects can include arrays. Not only do we create objects, but browsers come with their own built-in objects. In fact, the built-in objects include: browser object model, document object model, global javascript objects. What, then, is an object model? An object model is a group of objects. An example of a global JS object would be the Math object. 


