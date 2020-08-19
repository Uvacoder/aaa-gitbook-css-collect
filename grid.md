# Grid

|  | start |
| :--- | :--- |
| [https://1linelayouts.glitch.me/](https://1linelayouts.glitch.me/) | 7/6 |
| [Building a hexagonal grid using CSS grid](https://ninjarockstar.dev/css-hex-grids/) | 6/19 |
| [Understanding CSS Grid: Grid Template Areas](https://www.smashingmagazine.com/2020/02/understanding-css-grid-template-areas/) | 2/19 |
| [https://medium.com/free-code-camp/things-ive-learned-about-css-grid-layout-932777c2d6d7](https://medium.com/free-code-camp/things-ive-learned-about-css-grid-layout-932777c2d6d7) | 11/22/2019 |

```css
.container {
  display: grid;
  grid-gap: 20px; //spacing between columns and rows (tracks)
  grid-template-columns: 200px auto 1fr; //first column 200px, second will fill, and third will take 1 fractional rows
  grid-template-columns: repeat(5, 100px); //will repeat 5 columns of 100px
  grid-template-rows: 200px 100px 400px; //first three rows will be respective pixel size
  grid-auto-rows: 500px; //sets the height for implicit rows
}

```

