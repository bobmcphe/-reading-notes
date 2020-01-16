# Class-08 Reading Notes

## Chapter 7: “Forms”
 `<Form>` elements requires an action attribute. The information gained from forms is sent in name/value pairs, which if I understand is stored on a server. As Duckett explains, "HTML5 introduces new form elements which make it easier for visitors to fill in forms." This would include email and and url. 

## Chapter 14: “Lists, Tables & Forms” 
This chapter has a variegated assortment of tidbits. For example, unordered lists can use discs, circles, squares, or even no bullet at all. Ordered lists can use various means, such as all caps, all lower case, romans numerals, numbered, alphabetical, and a few combinations thereof. Even special images can be used to create basically whatever kind of bullet we want. 

Tables can also be modified in various ways. For example, in addition to the bare bones mimimum needed to populate a table, you can use the `show` attribute and the `hide` to show or hide borders, respectively. Also, you can use the `inherit` attribute to cascade the attributes of one table that is nested inside another table. `Border-spacing` and `border-collapse` allow further control of the borders. Specifically, `border-collapse` creates a single border from more than one, where possible. 

Another feature is the ability to style buttons. This can be done with a lot of the standard features elsewhere, but there is certainly one notable-and commonly used-feature, the `:hover`. The `:hover` is actually a pseudo-class, and controls what happens when the cursor hovers over the button. 

Form fieldsets are important in "determining the edges of the form." This, too, is subject to the standard capabilities, such as, `color`, `width`, `padding` and so on. The cursor also can be changed to suite various styles, as needed. The book lists the following commonly used values here:

1. auto 
1. crosshair 
1. default 
1. pointer 
1. move 
1. text 
1. wait 
1. help 
1. url("cursor.gif");

Another interesting section is the "Web Developer Toolbar." This is an extension which can be downloaded and added to the browser. For example, it will conveniently allow the developer to simply click on an element and see how it is styled in the CSS file, and by simply hovering over an element, it will show a read outline communicating the degree of space that is taken up around an element. 
