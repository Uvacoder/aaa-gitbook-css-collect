# Selectors

|  |  |
| :--- | :--- |
| [Understanding CSS Combinators](https://medium.com/better-programming/understanding-css-combinators-a36e013b1bed) | 9/30 |
| [The Skinny on CSS Attribute Selectors](https://css-tricks.com/attribute-selectors/) | 1/30/2020 |
| [CSS Diner](https://flukeout.github.io/) |  |
| [CSS MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) |  |

### Space: 

It is the descendant selector. It will target all p tags within container div.

```css
.container p {font-weight:bold;}
```

### &gt; Sign:

It will target elements which are **DIRECT** children of a particular element.[?](https://techbrij.com/css-selector-adjacent-child-sibling#)

```css
div#container > p {  border: 1px solid black;}
```

![css selector](https://img.techbrij.com/650/css%20selector%202.JPG)

It will target all P element which are direct children of container div, not children of child div.

### + Sign:

It is Adjacent sibling combinator. It combines two sequences of simple selectors having the same parent and the second one must come **IMMEDIATELY** after the first.

```css
div + p {    color: green; }
```

![css selector](https://img.techbrij.com/650/css%20selector%203.jpg)

It will only select the first element that is immediately preceded by the former selector. In our example, it will target to Second ONLY because the owner P element comes just after Div tag.

### ~ Sign:

It is general sibling combinator and similar to Adjacent sibling combinator. the difference is that the second selector does **NOT** have to immediately follow the first one means It will select all elements that is preceded by the former selector.[?](https://techbrij.com/css-selector-adjacent-child-sibling#)

```css
div ~ p{background-color:blue;}
```

![css selector](https://img.techbrij.com/650/css%20selector%204.jpg)

It will target both second and third.

