# Class 4 Reading NOtes

## Ch. 4 Links

The `<a>` tag is used for hyperlinks, which is directed to a path determined by the href attribute. The text that exists in between the opening `<a>` tag and closing `</a>` tag is what is clickable, and so it needs to be clear and concise as to where it is directing the person; but for UX and SEO.

The anchor tag is able to use both relative and absolute paths. In fact, links can even open up an email program with an email attached by assigning `href="mailto:example@gmail.com"`. Another common feature is to open a link into a new window, which is important for SEO purposes, by using the `target: "_blank"` property. 

## Ch. 15 Layout

CSS treats each element as if it is a block, with block-level elements being considered the parent element which starts on a new line. There are various ways to position these elements; relative, absolute, fixed, and floating. To add to the 2D positioning, we might speak of 3D positioning. That is, sometimes elements can overlap, in which case one must take precedence. This is determined by the Z-index. In addition to all these features is the ability to make the page 'responsive' to screen sizes as well as differences in screen resolution. Screen resolution is the amount of dots a screen can show in a squar inch. Usually, designers try to create a page that is roughly 960-1000 px wide. As a helpful sidenote, the part of the site that is immediatly seen upon being loaded is called 'above the fold,' originally a newspaper term. 

A major help in working with CSS are the CSS frameworks, however, it is possible that these frameworks will come with extra code not needed for the site, which slows things down. The main use of CSS frameworks in vogue at the moment is to use the 960.GS, or ones like it, to create grids for a layout. But since these frameworks provide common rules for common tasks, they can make the life of the developer much easier. 

## Ch. 3 - Functions, Methods, and Objects

Functions are distinct from methods in that methods are built inside, as it were, an object. Functions are simply blocks of code that are specifically designed to complete a particular task. So what, then, is an object? Objects have properties and methods, and are used to contructs a virtual world, so to speak, a model. You can get a single value from a function, or even more than one value, if it is using an array. It is helpful to keep in mind that there are named and anonymous functions. In short, the former are able to be used over and over again, since they can be invoked by name, whereas the latter cannot. 