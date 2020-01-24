# Class 14 Reading Notes

## CSS's Transform, Transition, and Animations

The CSS transform function is as follows:
```
div {
    transform: scale(1.5);
}

```

Thus the transform feature would be used with the pseud-class :hover like so:

```
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```

Transitions, which admit of shortcuts, are similar, and can also be applied to the :hover pseudo-class. However, the transition-timing-function property is required, and is set with the first state of the object, like so:

```
.box {
  background: #2db34a;
  border-radius: 6px;
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}
```

But as great as transitions are, they are still limited. A more functional and adaptable ability is allowed in CSS with the animation property. It is important to realize that, similar to the transition feature, this too needs to have two code blocks, as seen below:

```
.original {
  perspective: 200px;
}
.box {
  transform: rotateX(45deg);
}
.original-1 {
  perspective-origin: 0 0;
}
.original-2 {
  perspective-origin: 75% 75%;
}
.original-3 {
  perspective-origin: 20px 40px;
}
```

It is important to note that this animation feature makes us of the other features (e.g. transform). The different states are chosen, at the points the coder would like to choose, and how far along the transition is to have progressed. 

Footnote: all code was taken from the reading. 

