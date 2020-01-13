# Class-06 Reading Notes

## Object Literals

Programs need objects in order to make sense of the world we know and live in. Objects group together variables and functions, and even other objects, to create a model.  When a variable is attached to an object, it becomes a property, when a function is attached to an object, it becomes a method. 

1. objects consist of name/value pairs. 
1. Objects are created using literal notation, and accessed using dot notation, generally.
1. However, you can also access the properties of an object by useing the square brackets.


## Chapter 5. Document Object Model

As browsers created a web page, it also automatically creates a DOM tree, which in turn is a series of four basic nodes. Everything on the page is represented by a node. Essentially, "Each node is an object with methods and properties" according to Duckett, (pg 187).

The four basic kinds of nodes are text nodes (which cannot have any child elements), attribute nodes, element nodes, and document nodes. However, each site should only have one document node, is my impression. DOM manipulation can either change or rearrange one or more elements at a time. 

Any method whose purpose is to find an element within the DOM tree is termed "DOM quiery." getElementById() is the fastest way to select an element. But elements can be selected by a variet of ways (e.g. class, attributes, tag name, etc.). In fact, we can even loop through a node list to find what we want. Another way to navigate the DOM tree is by 'traversing the DOM', but this can be difficult sometimes due t browsers trying to add a text node where there is a whitespace in the code. Element nodes are helpful, in that we can access and update their content, the HTML simply through DOM manipulation. But it's important to recall that an element node can contain multiple text nodes and other child elements. 

Unfortunately, old browsers do not provide good support for the DOM, and so jQuery has become popular as a result. Nevertheless, modern browsers are very helpful in this regard, even offering tools for viewing the DOM tree. 

