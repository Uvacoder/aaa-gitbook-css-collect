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
  grid-template-columns: 200px auto 1fr; //first column 200px, second will fill depending on content width, and third will take 1 fractional rows
  grid-template-columns: repeat(5, 100px); //will repeat 5 columns of 100px
      auto-fill // automatically fills grid items
    auto-fit // ends grid automatically at last grid item
    minmax // set minimum and maximum sizes
    fit-content(100px) //fit-content
  grid-template-rows: 200px 100px 400px; //first three rows will be respective pixel size
  grid-auto-rows: 500px; //sets the height for implicit rows
  grid-auto-flow: row; //default
}

.item9 {
  grid-column: span 2; //target item will span 2 columns
  grid-row: span 3; //target will span 3 columns
  grid-column-start: 2; //starts at the 2nd track column
  grid-column-end: 6; //ends at the 6th track column
  grid-column: 2 / -1; //start at 2 track and end at last column
}

```

