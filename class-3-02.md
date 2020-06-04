# Basic Jquery Intro

JQuery uses CSS selectors, to search for items and then return or modify it, and it handles events. It is excellent due to cross-browser compatiblity, but unfortunately, tends to be a bit bigger than is ideal. Jquery is nothing more than a Javascript file which your site accesses to simplify the coding process. It is similar to the DOM manipulation process, but a much easier and simplier style. 

Jquery uses methods that enable the user to retrieve information, and update the content of elements. Once this selection is made, the information is stored as a reference to specific node in the DOM without making copies, thus being more efficient with the memory. 


The basic format is:

`$('ul.awesomeness').addID('notAwesome');` The different sections break down in the following way:

$() - a JQuery method.
$('ul.awesomeness') - Jquery object.
.addID('notAwesome'); - Method

'notAwesome' - Parameters

## Different Ways to use and apply Jquery


Here are four different ways you can use Jquery to update the content of an element:

1. .html()
1. .replaceWith()
1. .text()
1. .remove()

Here are four ways to instert or add elements:

1. .before()
1. .after()
1. .prepend()
1. .append()

The following methods allow you to modify attribute values:

1. .attr()
1. .removeAttr()
1. .addClass()
1. .removeClass()

Instead typing out a `for` loop or `while` loop, you can use the `.each()`.

Jquery also has event handlers, usually the `.on()`. Each function for an evend handler receives a specific object for that event, which uses the objects properties and methods which stores information about the event. 

## How to add Jquery to your site

The most common solution is to use a Content Distribution Network (CDN). A CDN hosts a file in various locations and serves the content to the user if that that particular server is the closest. For perceived speed, programmers often place the javascript in the footer section so that it loads last, since it's loading is usually not visually noticed. 

It is worth noting that, if possible, it is best practice to use alternatives to scripts like Javascript or Jquery. For example, using CSS for animations. This can help with speed, but it does have the down side of complicating code maintenance. 