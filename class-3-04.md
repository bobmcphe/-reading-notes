# CSS Grid
According to some, CSS Grid is the most powerful tool in CSS. Unlike Flexbox, it is a 2-D instead of 1-D system, and can provide the same sort of functionality, essentially, that float or flex can, in less code and a more intuitive manner.

You determine the parent element will display its contents as a grid via:

`display:grid'`

Then determine the grid template with something like:

`grid-template-columns: 00px 00px;` 

It is possible, however, to use a new measurement unit specific to grid, the `fr`. This stands for fraction ratio, (e.g. 1/2, 1/4, etc).

It is also useful to know and use the `grid-gap` capability, which controls the gutters. Grid has the following properties, in fact:

1. Grid-template-rows
1. Grid-template-columns
1. Grid-template-areas
1. Grid-auto-rows
1. Grid-auto-columns
1. Grid-auto-flow
1. Column-count

Here is partial code for the so-called 'holy grail' layout*:

  .container {
    display: grid;
    grid-template-columns: 200px 1fr 200px;
    grid-template-rows: auto 1fr auto;

  }

  With Grid, doing CSS is deceptively easy. (* example code taken from: https://glitch.com/edit/#!/grid-grail?path=styles.css%3A13%3A0)

# REGEX

Below is a short REGEX cheatsheet

1. \D - not a digit
1. \d - digit
1. \W - not a word
1. \w - a word
1. \S - not a whitespace
1. \s - a whitespace
1. [A-Z] - a range from A to Z
1. [^abc] - not abc
1. ^ - beginning
1. $ - ending
1. . - matches any character
1. \b - word boundary
1. \B - not a word boundary
1. flag i - case insensitive
1. flag g - global search
1. flag u - unicode
1. flag m - multiline
1. * - gready operator which expands the search as far as possible
1. {} - gready operator which expands the search as far as possible
1. + - gready operator which expands the search as far as possible
1. (?=) - look ahead
1. (?<=>)- look behind

