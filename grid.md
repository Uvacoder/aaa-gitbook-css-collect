# Grid

|  | start |
| :--- | :--- |
| [Top 7 CSS Grid Layout Concepts With Examples](https://betterprogramming.pub/top-7-css-grid-layout-concepts-with-examples-18c85e4d0b27) | 5/10 |
| [CSS Grid Cheat Sheet Illustrated in 2021](https://dev.to/joyshaheb/css-grid-cheat-sheet-illustrated-in-2021-1a3?utm_source=digest_mailer&utm_medium=email&utm_campaign=digest_email) | 3/7 |
| [A Deep Dive Into CSS Grid minmax\(\)](https://ishadeed.com/article/css-grid-minmax/) | 11/20 |
| [grid layoutit](https://grid.layoutit.com/) | 10/16 |
| [A Guide to CSS Grids for Designers: Flexbox, CSS Grid, Floats & Clears](https://blog.prototypr.io/a-guide-to-css-grids-for-designers-flexbox-css-grid-floats-clears-9487659aed92) | 9/25 |
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
  grid-template-columns: [left] 1fr [content-start] 500px [content-end] 1fr [right]; //named columns
  grid-template-rows: 200px 100px 400px; //first three rows will be respective pixel size
  grid-auto-rows: 500px; //sets the height for implicit rows
  grid-auto-flow: row; //default
  grid-template-areas: 
    "sidebar-1 content sidebar-2" 
    "sidebar-1 content sidebar-2" 
    "footer footer footer";
  grid-auto-flow:dense; //auto flows grid to fill out the grid holes
}

.item9 {
  grid-column: span 2; //target item will span 2 columns
  grid-row: span 3; //target will span 3 columns
  grid-column-start: 2; //starts at the 2nd track column
  grid-column-end: 6; //ends at the 6th track column
  grid-column: 2 / -1; //start at 2 track and end at last column
  grid-column: content-start; //reference to self named line from 18. grid-template-columns
}

.item1 {
    grid-area:sidebar-1;
}
.item2 {
    grid-area:sidebar-2;
}
.footer {
    grid-area: footer;
}

@media (max-width:768px) {
    .container {
          grid-template-areas: 
            "content content content" 
            "sidebar-1 sidebar-1 sidebar-2" 
            "footer footer footer"
    }
}
```

|  |  |  |
| :--- | :--- | :--- |
| [align-items](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items) | stretch, center, start, end | The [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) **`align-items`** property sets the [`align-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/align-self) value on all direct children as a group. In Grid Layout, it controls the alignment of items on the Block Axis within their [grid area](https://developer.mozilla.org/en-US/docs/Glossary/Grid_Areas). |
| [grid-auto-flow](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-flow) | row, column, row dense | The **`grid-auto-flow`** CSS property controls how the auto-placement algorithm works, specifying exactly how auto-placed items get flowed into the grid. |
| [justify-items](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-items) | stretch, center, start, end | The [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) **`justify-items`** property defines the default [`justify-self`](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-self) for all items of the box, giving them all a default way of justifying each box along the appropriate axis. |

