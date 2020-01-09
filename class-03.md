# Class - 03
## Ch. 3 - Lists -

There are three types of lists; ordered, unordered, and definition. Unordered lists are simply bulleted lists, whereas ordered lists are numbered, and thus prioritiezed. A defition list is simply a listed set of text which is needed for definitions. Finally, one can nest a list within a list.

## Ch. 13 - Boxes - 
Conveniently, HTML breaks down into boxes well since it treats each element as if it has its own box. This is crucial for making the most of UX, structuring the website so people know who to visually 'read' the content. All box capabilities break down into either block-level boxes, or inline level boxes. 


## Ch. 4 - 
Decisions and Loops - This section covers a few different topics, so we will start with switches. The switch starts with the switch value, which is the variable that is determinative here. Instead of use 'ifs' the switch use 'cases', and if a case corresponds to the variable, then the switch will terminate the section of code with a break command, and exit. If no case matches, then the switch statement will execute the default position, though I think this is optional. 

Because JS uses type coercion, specifically, weak type, this can lead to errors. When JS comes across a type of data it did not expect to find, it will try to convert it. For example, if it runs into an empty string, it will treat it may treat it as false, or 'falsey.' Likewise with numbers above zero, or any normal string, it will treat these data types as true, or 'truthy.'

This is why using strict equality operators, are often helpful. Another potential problem is when code is 'short circuited.' 

The last subject here is loops, which there are three kinds; for loops, while loops, and do while loops. While loops simply execute a code while a certain condition is true, and do...while loops simply execute a particular line(s) of code before the loop while a condition is true. For loops can be translated back and forth into while loops, but they are a quicker way of writing the code. However, it is important to make sure to do things like increment a code (if, say, looping through an array) or one will end up with an infinite loop.

