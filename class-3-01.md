# Responsive Web Design
## The Basics

Responsive web design is simply making a site optimized at various sizes. This can be done three methods, which usually include each other, not being mutually exclusive. 

1. Responsive - a site immediately adjusts to any change in screen size, usually accomplished by using rem, %'s and a few other tricks to help the constitutive elements of a site shift.

1. Mobile - usually means a separate website specifically for mobile devies, a method that is usually not ideal.

1. Adaptive - in contrast to responsive, this uses features like media queries to change a layout based on the size of the screen. 

## Responsive Web Design Components

A flexible layout usually consists in three things:

1. media queries
1. flexible media
1. flexible layout, (e.g. flexible grids)

## Floats

Definition: a CSS positioning property. The term originated regarding the paper print, where by a picture would be shifted either far left or far right and letting the text 'wrap' around the image. We have four different values for the float property:

1. left
1. right
1. inherit
1. none

### Float's clear property

The clear property allows the flow to be reset, and this can be helpful at times. Instead of staking two items in-line, it can, for example, cause one element to drop underneath the most outer element. 

## Grids
It's essentially impossible to not have a grid, so it is worth understanding them and how they work. Sometimes, in fact, grid framworks are used, which help with managing complex grids. Some basic key facts can make approaching grids easier:

1. All block elements will normally seek to be as wide as it's parent element. 
1. Breaking down your grid into columns makes it easier to manage and understand.
1. Decide which column will house your main content, and which will bar will be your 'side content'
1. Be familiar with `moz-box-sizing`, and `webkit-box-sizing` 
1. Internet Explorer tends to have issues, so you might want to find workarounds for that.

### Gutters

Gutters are porpurtedly the most difficult thing about good grids. Making columns whereby the ratios add up to one, is the trick, (with responsiveness in mind). 

