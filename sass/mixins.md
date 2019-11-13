# Mixins

### Animation

```css
@mixin elem_animate($speed: .3s) {
    -webkit-transition: all $speed ease-in-out;
    -moz-transition: all $speed ease-in-out;
    transition: all $speed ease-in-out;
}

@mixin slideOff($duration: 1s,$iterations:1,$direction:normal,$ease:ease-in-out,$fill:none,$delay:0){
  animation-name: slideOff;
  animation-duration: $duration; /* or: Xms */
  animation-iteration-count: $iterations;
  animation-direction: $direction; /* or: normal */
  animation-timing-function: $ease; /* or: ease, ease-in, ease-in-out, linear, cubic-bezier(x1, y1, x2, y2) */
  animation-fill-mode: $fill; /* or: backwards, both, none */
  animation-delay: $delay; /* or: Xms */
  @keyframes slideOff {
    0% { background-position-x: 0; }
    50% { transform:translateX(15px); opacity:0;}
    55% { transform:translateX(-15px); opacity:0;}
    100% { background-position-x: 0; opacity: 1;}
  }
}

@mixin slideDown($duration: 1s,$iterations:1,$direction:normal,$ease:ease-in-out,$fill:none,$delay:0){
  animation-name: slideDown;
  animation-duration: $duration; /* or: Xms */
  animation-iteration-count: $iterations;
  animation-direction: $direction; /* or: normal */
  animation-timing-function: $ease; /* or: ease, ease-in, ease-in-out, linear, cubic-bezier(x1, y1, x2, y2) */
  animation-fill-mode: $fill; /* or: backwards, both, none */
  animation-delay: $delay; /* or: Xms */
  @keyframes slideDown {
    0% { background-position-x: 0; }
    50% { transform:translateY(22px); opacity:0;}
    55% { transform:translateY(-22px); opacity:0;}
    100% { background-position-x: 0; opacity: 1;}
  }
}
```

### IE

```css
  @mixin ie($class){
    _:-ms-lang(x), #{$class} {
      @content;
    }
  }

```

### 

|  |  |
| :--- | :--- |
| [line height crop](https://medium.com/codyhouse/line-height-crop-a-simple-css-formula-to-remove-top-space-from-your-text-9c3de06d7c6f) | @mixin |

### Media Queries

```css
// Mixin for min-width media query, accepts a width parameter
@mixin mq-min($width) {
    @media screen and (min-width: $width) {
        @content;
    }
}

// Mixin for max-width media query, accepts a width parameter
@mixin mq-max($width) {
    @media screen and (max-width: $width) {
        @content;
    }
}
```

