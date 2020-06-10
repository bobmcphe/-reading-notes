# CLASS 3

## Templating with Mustache

Mustache is an awesome logic-less means of providing a template. Logic-less does not mean, in my opinion, that Mustache is irrational or anti-logic, as such, but only that the template only provides a basic system for data, and cannot take any sort of pseudo-thought, such as if-then conditionals. 

It is worthy of note that Mustache is only one of many options out there, the simplest, and not itself a templating engine. 

It works well, for example, with taking the data in a JSON file and allowing a degree of dynamic loading on the HTML side of the house, for example: 

`
{
  "name": "Chris",
  "company": "<b>GitHub</b>"
}
`

The above code would load in the html via the template:

`
<h1>{{name}}</h1>
<h2>{{company}}</h2>
`

## Flexbox

The first thing to understand about flexbox is that it applies directly to the parent of the item(s) you wish to style, unlike float. The initial (without getting into the details) capabilities the developer needs to know is `flex-direction`, `flex-wrap`, `justify-ccontent`, `align-items` and `align-content`. The difference between `align-items` and `align-content` can be a little confusing at first. But as I understand it, the `align-items` pertains to the items of a single row, whereas the latter refers to the different rows themselves.

When one does use, say, `justify-ccontent`, you normally have the following options:

1. `flex-start` -shift all objects to beggining
1. `flex-end` - sheft objects to end
1. `center` - self-explanatory
1. `baseline` (for align-content and align-items)
1. `space-between` - even spaces between objects, to exclude outer edges of outer objects
1. `space-around` - makes even spacing around each object


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