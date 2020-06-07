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


