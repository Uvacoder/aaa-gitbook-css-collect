# Typography

|  |  |
| :--- | :--- |
| [Intrinsic Typography is the Future of Styling Text on the Web](https://css-tricks.com/intrinsic-typography-is-the-future-of-styling-text-on-the-web/) | 4/20 |
| [6 Practical Tips - Typography System Creation](https://blog.prototypr.io/6-practical-tips-typography-system-creation-9909c6f3a89c) | 12/8 |

### Font-smoothing

```text
-webkit-font-smoothing: antialiased;
-moz-osx-font-smoothing: grayscale;
```

### @font-face

```css
@font-face {
  font-family: ‘MyWebFont’;
  src: url(‘webfont.eot’);
  src: url(‘webfont.eot?#iefix’) format(‘embedded-opentype’),
       url(‘webfont.woff’) format(‘woff’),
       url(‘webfont.ttf’) format(‘truetype’),
       url(‘webfont.svg#svgFontName’) format(‘svg’);
 }
```

