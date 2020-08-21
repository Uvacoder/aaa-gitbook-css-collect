# Grid

|  | start |
| :--- | :--- |
| [https://1linelayouts.glitch.me/](https://1linelayouts.glitch.me/) | 7/6 |
| [Building a hexagonal grid using CSS grid](https://ninjarockstar.dev/css-hex-grids/) | 6/19 |
| [Understanding CSS Grid: Grid Template Areas](https://www.smashingmagazine.com/2020/02/understanding-css-grid-template-areas/) | 2/19 |
| [https://medium.com/free-code-camp/things-ive-learned-about-css-grid-layout-932777c2d6d7](https://medium.com/free-code-camp/things-ive-learned-about-css-grid-layout-932777c2d6d7) | 11/22/2019 |
| [How I use CSS Grid to Create a One-page Website](https://medium.com/swlh/how-i-use-css-grid-to-create-a-one-page-website-ffc97668d33a) | 8/14 |
| [How to build complex layouts with CSS grid](https://gomakethings.com/how-to-build-complex-layouts-with-css-grid/?mc_cid=99b9850ca0&mc_eid=[UNIQID]) | 4/30 |
| [An introduction to CSS Grid](https://gomakethings.com/an-introduction-to-css-grid/?mc_cid=964ca6754c&mc_eid=[UNIQID]) | 4/28 |
| [CSS Grid Generator](https://cssgrid-generator.netlify.com/) | 3/4 |
| [Layout land youtube](https://www.youtube.com/watch?v=FEnRpy9Xfes&list=PLbSquHt1VCf1x_-1ytlVMT0AMwADlWtc1) | 2/12 |

```css
.container {
  display: grid;
  grid-gap: 20px; //spacing between columns and rows (tracks)
  grid-template-columns: 200px auto 1fr; //first column 200px, second will fill depending on content width, and third will take 1 fractional rows
  grid-template-columns: repeat(5, 100px); //will repeat 5 columns of 100px
    repeat(auto-fill) // automatically fills grid items
    repeat(auto-fit) // ends grid automatically at last grid item
    minmax(150px, 1fr); // set minimum and maximum sizes
    fit-content(100px) // auto fit-content with clamp max-width 100px
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

