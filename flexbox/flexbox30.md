# Flexbox30

{% embed url="https://github.com/samanthaming/Flexbox30" %}



## Flexbox30

Learn Flexbox in 30 days with 30 code tidbits ✨

### Table of Contents

1. [Introduction](https://github.com/samanthaming/Flexbox30#flexbox-intro)
2. [Flex Container & Flex Items](https://github.com/samanthaming/Flexbox30#flex-container-and-flex-items)
3. [Immediate Child Only](https://github.com/samanthaming/Flexbox30#immediate-child-only)
4. [Flexbox Axes](https://github.com/samanthaming/Flexbox30#flexbox-axes)
5. [Flexbox Module](https://github.com/samanthaming/Flexbox30#flexbox-module)
6. [Parent Properties](https://github.com/samanthaming/Flexbox30#parent-properties)
7. [Display](https://github.com/samanthaming/Flexbox30#display)
8. [block vs inline](https://github.com/samanthaming/Flexbox30#block-vs-inline)
9. [flex-direction](https://github.com/samanthaming/Flexbox30#flex-direction)
10. [flex-wrap](https://github.com/samanthaming/Flexbox30#flex-wrap)
11. [flex-flow](https://github.com/samanthaming/Flexbox30#flex-flow)
12. [justify-content \[row\]](https://github.com/samanthaming/Flexbox30#justify-content-row)
13. [space-around vs space-evenly](https://github.com/samanthaming/Flexbox30#space-around-vs-space-evenly)
14. [justify-content \[column\]](https://github.com/samanthaming/Flexbox30#justify-content-column)
15. [align-items \[row\]](https://github.com/samanthaming/Flexbox30#align-items-row)
16. [baseline](https://github.com/samanthaming/Flexbox30#baseline)
17. [align-items \[column\]](https://github.com/samanthaming/Flexbox30#align-items-column)
18. [align-content](https://github.com/samanthaming/Flexbox30#align-content)
19. [Child Properties](https://github.com/samanthaming/Flexbox30#child-properties)
20. [order](https://github.com/samanthaming/Flexbox30#order)
21. [flex-grow](https://github.com/samanthaming/Flexbox30#flex-grow)
22. [flex-grow calculation](https://github.com/samanthaming/Flexbox30#flex-grow-calculation)
23. [flex-shrink](https://github.com/samanthaming/Flexbox30#flex-shrink)
24. [flex-shrink calculation](https://github.com/samanthaming/Flexbox30#flex-shrink-calculation)
25. [flex-basis](https://github.com/samanthaming/Flexbox30#flex-basis)
26. [flex-basis vs widths](https://github.com/samanthaming/Flexbox30#flex-basis-vs-widths)
27. [flex](https://github.com/samanthaming/Flexbox30#flex)
28. [align-self](https://github.com/samanthaming/Flexbox30#align-self)
29. [Flexbox Properties](https://github.com/samanthaming/Flexbox30#flexbox-properties)
30. [Flexbox Cheatsheet](https://github.com/samanthaming/Flexbox30#flexbox-cheatsheet)
31. [Aligning with Auto Margins](https://github.com/samanthaming/Flexbox30#bonus-aligning-with-auto-margins)
32. [Resources](https://github.com/samanthaming/Flexbox30#resources)
33. [Say Hello](https://github.com/samanthaming/Flexbox30#say-hello)
34. [Download & Share](https://github.com/samanthaming/Flexbox30#download-and-share)
35. [Contribution](https://github.com/samanthaming/Flexbox30#contribution)
36. [License](https://github.com/samanthaming/Flexbox30#license)

### Flexbox Core Concepts

#### [Day 1: Introduction](https://github.com/samanthaming/Flexbox30#flexbox-intro)

Before Flexbox, we were mainly using floats for layout. And for those CSS developers, we all know the frustrations and limitations of the old way -- especially the ability to vertically center inside a parent. Ugh, that was so annoying! Not anymore! Flexbox for the win!

![Flexbox Introduction](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/1-flexbox-intro.png)

#### [Day 2: Flex Container & Flex Items](https://github.com/samanthaming/Flexbox30#flex-container-and-flex-items)

In order to get Flexbox to work, you need to set up the Parent-Child relationship. The parent is the flex container, and everything within it is the children or flex items.

![Flex Container &amp; Flex Items](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/2-flex-container-and-flex-items.png)

#### [Day 3: Immediate Child Only](https://github.com/samanthaming/Flexbox30#immediate-child-only)

One VERY important thing I want to point out is that the flex container only wraps around its immediate children. The flex container doesn't wrap beyond one layer deep. Only the immediate children. So there is NOT a grandchildren or grand-grandchildren relationship. Only Parent ↔️ Immediate Children!

Of course, you can establish a Flexbox as long as there is a parent-child relationship. So a child can also be the flex container to its children. But it will be a separate flex container. And it doesn't carry over the grandparent flex properties.

This is probably one of the most important concepts that helped me understand how Flexbox works. And knowing this will help solve a lot of those "hey, why isn't this working" moments 😅

![Immediate Child Only](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/3-immediate-child-only.png)

#### [Day 4: Flexbox Axes](https://github.com/samanthaming/Flexbox30#flexbox-axes)

Flexbox operates in a 2 axes system: a main and a cross axis. The main axis is your defining direction of how your flex items are placed in the flex container. Determining the cross axis is very simple, it's in the direction that's perpendicular to your main axis.

Remember in math class, we were taught **x** and **y** axis. Well, throw that out. Because the main axis can be horizontal or vertical. The **x** axis is not always the main axis. This was a mistake I made, so hopefully you won’t make the same incorrect assumption as I did 😅

![Flexbox Axes](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/4-flexbox-axes.png)

#### [Day 5: Flexbox Module](https://github.com/samanthaming/Flexbox30#flexbox-module)

Let's zoom in on one of the layouts and check out the anatomy of our Flexbox. On each axis, there is a start and an end. If it's on the main axis, the starting position is called **main start** and if the ending position is called **main end**. The same concept applies to the cross axis. Knowing your start and end is important because you can control where your flex items are placed.

And this concludes our Flexbox Fundamentals.

![Flexbox Module](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/5-flexbox-module.png)

[**⬆ back to top**](https://github.com/samanthaming/Flexbox30#table-of-contents)

### Parent Properties

#### [Day 6: Parent Properties](https://github.com/samanthaming/Flexbox30#parent-properties)

Now you know Flex operates in a Parent-Child relationship. So we have 2 entities involved to get this tango started. And each entity will have its own set of unique CSS properties that can be applied to them. That's why it's important that you know which element is the parent and which element\(s\) is the child. Let's get started with the parent properties 🤰

![Parent Properties](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/6-parent-properties.png)

#### [Day 7: Display](https://github.com/samanthaming/Flexbox30#display)

To start this Flexbox party, we need to first create our flex container. This is done by applying `flex` to the `display` property on the parent element. Bam! Now all its immediate children will become flex items 🎊

There are 2 types of flex container: `flex` will create a _block_ level flex container. And `inline-flex` will create an _inline_ level flex container. More on _block_ and _inline_ tomorrow 😉

![Display](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/7-display.png)

```text
.parent {
  display: flex /* default */
        or inline-flex
}
```

#### [Day 8: block vs inline](https://github.com/samanthaming/Flexbox30#block-vs-inline)

Very simply explained, `block` element takes up the entire width of the container. They look like building blocks where each block is stacked on each other. Whereas `inline` element only takes up the space it needs. So they appear to be in a line, or side by side of each other.

![block vs inline](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/8-block-vs-inline.png)

#### [Day 9: flex-direction](https://github.com/samanthaming/Flexbox30#flex-direction)

This is the property that allows us to define our main axis. Remember I mentioned that our main axis can be horizontal or vertical. So if we want the main axis to be horizontal, that's called **row**. And if we want it to be vertical, that's called **column**. Also, remember we had a **main start** and **main end**. We simply add a `reverse` suffix to set our "main start" in the reverse direction. Pretty cool eh 👍

![flex-direction](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/9-flex-direction.png)

```text
.parent {
  flex-direction: row /* default */
               or row-reverse
               or column
               or column-reverse
}
```

#### [Day 10: flex-wrap](https://github.com/samanthaming/Flexbox30#flex-wrap)

By default, flex items will try to shrink itself to fit onto one line, in other words, `no wrap`. However if you want the flex items to maintain its size and have the overflow spread on multiple lines in the containers, then you can turn on `wrap`.

This property is what will allow flex items in your container to occupy more than one line.

![flex-wrap](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/10-flex-wrap.png)

```text
.parent {
  flex-wrap: nowrap /* default */
          or wrap
          or wrap-reverse
}
```

#### [Day 11: flex-flow](https://github.com/samanthaming/Flexbox30#flex-flow)

So we've learned `flex-direction` and `flex-wrap`. If you understand those 2, you'll get `flex-flow`! Because it's just a shorthand for these two properties 👏

You can set both properties at the same time. Or you can just pass one of them. The default value is `row nowrap`. So if you just set one value, the property that you didn't set will just take on the default value.

![flex-flow](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/11-flex-flow.png)

```text
.parent {
  flex-flow: row nowrap /* default */
          or <flex-direction> <flex-wrap>
          or <flex-direction>
          or <flex-wrap>
}
```

#### [Day 12: justify-content \[row\]](https://github.com/samanthaming/Flexbox30#justify-content-row)

Here comes the fun part. This is the property that sets alignment along the main axis. In this example, the main axis lies horizontally. In other words, the flex-direction is set to `row`.

This is probably my most used parent property. You just choose the layout you like and BAM Flexbox automatically does it for you. And it's absolutely responsive. As your grow or shrink the window width, Flexbox will do the behind-the-scene calculation and ensure that your chosen layout is maintained. It's like one of those kitchen appliances where "you set it and forget it" 🍗

![justify-content row](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/12-justify-content-row.png)

```text
.parent {
  justify-content: flex-start /* default */
                or flex-end
                or center
                or space-around
                or space-between
                or space-evenly
}
```

#### [Day 13: justify-content \[column\]](https://github.com/samanthaming/Flexbox30#justify-content-column)

The main axis can also lie vertically. In that case, flex-direction is set to `column`. Here's how the flex items will be aligned in that instance.

![justify-content column](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/14-justify-content-column.png)

```text
.parent {
  flex-direction: column;
  
  justify-content: flex-start /* default */
                or flex-end
                or center
                or space-around
                or space-between
                or space-evenly
}
```

#### [Day 14: space-around vs space-evenly](https://github.com/samanthaming/Flexbox30#space-around-vs-space-evenly)

You might not notice the subtle difference between space-around and space-evenly. So let's talk about it. In `space-evenly`, the empty space in between the flex items is always equal. However, in `space-around`, only the inner items will have equal spacing in between each other. The first and last item will only be allocated half the spacing. Giving the visual appearance of it being more spread out. One may say these folks like to live life on the edge 😂

![space-around vs space-evenly](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/13-space-around-vs-space-evenly.png)

#### [Day 15: align-items \[row\]](https://github.com/samanthaming/Flexbox30#align-items-row)

So justify-content controls how items are laid out on the main axis. What about their layout in the cross axis? Don't worry, that's where `align-items` come into play. Remember the cross axis is always perpendicular to the main axis. So if the main axis is sitting horizontally, where flex-direction is `row`. Then , the cross axis is sitting vertically. Aren't you glad we spend almost a week on the fundamentals, that knowledge is all being applied now 🤓

![align-items row](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/15-align-items-row.png)

```text
.parent {
  align-items: stretch /* default */
            or flex-start
            or flex-end
            or center
            or baseline
}
```

#### [Day 16: baseline](https://github.com/samanthaming/Flexbox30#baseline)

The baseline value is a bit tricky. So let's make sure we understand what that is. Baseline has to do with typography or text. It is the imaginary line where the text sits. If you have the same font size, you really don't visually see a difference. However when you have different font sizes, then the text seems all over the place because the baseline is off. The way to ensure a uniform baseline where all the different sizes of text can rest on is to use the `baseline` value 👍

![baseline](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/16-baseline.png)

#### [Day 17: align-items \[column\]](https://github.com/samanthaming/Flexbox30#align-items-column)

Now let's take a look at how our flex items are aligned if the cross axis is sitting horizontally. In other words, flex-direction is `column`.

![align-items column](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/17-align-items-column.png)

```text
.parent {
  flex-direction: column;
  
  align-items: stretch /* default */
            or flex-start
            or flex-end
            or center
            or baseline
}
```

#### [Day 18: align-content](https://github.com/samanthaming/Flexbox30#align-content)

Remember we had `flex-wrap` where we allow flex items to wrap on separate lines. Well, with `align-content` we can control how those row of items are aligned on the cross axis. Since this is only for wrapped items, this property won't have any effect if you only have a singular line of flex items.

![align-content](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/18-align-content.png)

```text
.parent {
  align-content: stretch /* default */
              or flex-start
              or flex-end
              or center
              or space-between
              or space-around
}
```

[**⬆ back to top**](https://github.com/samanthaming/Flexbox30#table-of-contents)

### Child Properties

#### [Day 19: Child Properties](https://github.com/samanthaming/Flexbox30#child-properties)

Yay, you did it! We made it through the parent properties. Up next, let dig into the child properties. Take a breather today, tomorrow we go full speed again 🏎

![Child Properties](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/19-child-properties.png)

#### [Day 20: order](https://github.com/samanthaming/Flexbox30#order)

By default, flex items are displayed in the same order they appear in your code. But what if you want to change that? No problem! Use the `order` property to change the ordering of your items 🔢

![order](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/20-order.png)

```text
.child {
  order: 0 /* default */
      or <number>
}
```

#### [Day 21: flex-grow](https://github.com/samanthaming/Flexbox30#flex-grow)

I mentioned in the beginning that Flexbox is great for responsive design. This is where it shines. The `flex-grow` property allows our flex item to grow if necessary. So if there is extra free space in my container, I can tell a particular item to fill it up based on some proportion. That's pretty nuts! When I was learning CSS, I remember everything is pretty static. Now with this property, it's like it has its own brain and it will adjust its size depending on the container. That's so great. I don't have to monitor the size. It will adjust accordingly. This was a quite the mind blow for me 🤯

![flex-grow](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/21-flex-grow.png)

```text
.child {
  flex-grow: 0 /* default */
          or <number>
}
```

#### [Day 22: flex-grow calculation](https://github.com/samanthaming/Flexbox30#flex-grow-calculation)

Being able to grow and fill the free space is pretty cool. Because we don't set the final width of our flex item, the size it grows to always seem so random to me. So let's look at the math. Honestly you don't need to know this to understand Flexbox. The browser takes care of this automatically for you. But knowing what's behind this sorcery might demystify this process and help you understand it better. It's like once you know the trick to the magic, you're no longer tricked by the magic 😉

**Expand to see the calculation**

![flex-grow calculation](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/22-flex-grow-calculation.png)

#### [Day 23: flex-shrink](https://github.com/samanthaming/Flexbox30#flex-shrink)

![flex-shrink](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/23-flex-shrink.png)

So `flex-grow` will expand to fill the extra space if there are any. The opposite of that is `flex-shrink`. What happens when you run out of space. This is the property that controls how much your flex items will shrink to fit. Note the larger the number, the more it will shrink 👍

```text
.child {
  flex-shrink: 1 /* default */
            or <number>
}
```

#### [Day 24: flex-shrink calculation](https://github.com/samanthaming/Flexbox30#flex-shrink-calculation)

This is another optional knowledge. But if you're like me and is curious how the browser calculates flex-shrink. Join me in this rabbit hole 🐰

The math behind `flex-shrink` is a bit more complicated then `flex-grow`. You need to take into account of it's existing proportion and shrink it accordingly to the flex shrink amount. Hence, a few more calculation involved. Again, if this is throwing you off. Skip it. You don't need to know this to understand Flexbox. Luckily the browser takes care of it for you, how wonderful 😌

**Expand to see the calculation**

![flex-shrink calculation](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/24-flex-shrink-calculation.png)

#### [Day 25: flex-basis](https://github.com/samanthaming/Flexbox30#flex-basis)

With the flex-grow and flex-shrink property, we know the flex size changes. With the `flex-basis` property, this is where we set it's the initial size. You can think of this property as the width of our flex items. So your next question might be what's the difference between width and flex-basis. Of course, you can still use width and it will still work. The reason it works is because if you didn't set the flex-basis, it will default to the width. So your browser will always try to find the `flex-basis` value as the size indicator. And if it can't find it, then it has no choice but to go with your width property. Don't make the browser do extra work. Do it the proper flex way and use `flex-basis`.

You may notice I referenced width in my previous formulas. That's because I had not cover flex-basis at that point. So if we want to be **flex** correct, please replace where I mentioned width with flex-basis 😝

![flex-basis](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/25-flex-basis.png)

```text
.child {
  flex-basis: auto /* default */
           or <width>
}
```

Valid width values are absolute [`<length>`](https://developer.mozilla.org/en-US/docs/Web/CSS/length) and [`<percentage>`](https://developer.mozilla.org/en-US/docs/Web/CSS/percentage). You can see some examples and read more on MDN web docs:

* [`MDN: <length>`](https://developer.mozilla.org/en-US/docs/Web/CSS/length)
* [`MDN: <percentage>`](https://developer.mozilla.org/en-US/docs/Web/CSS/percentage)

#### [Day 26: flex-basis vs widths](https://github.com/samanthaming/Flexbox30#flex-basis-vs-widths)

Here you can see very clearly that when an item has a flex-basis and a width. The browser will always use the value set with `flex-basis` . Again, another reason to use the proper flex way 😉

But watch out, if you also set a `min-width` and `max-width`. In those cases, `flex-basis` will lose and will not be used as the width.

![flex-basis vs widths](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/26-flex-basis-vs-widths.png)

#### [Day 27: flex](https://github.com/samanthaming/Flexbox30#flex)

Sometimes, setting `flex-grow`, `flex-shrink` and `flex-basis` separately are tiring. Well, don't you worry. For the lazy programmers, I mean the efficient programmers 😜 You can set all 3 with the `flex` shorthand. The added bonus of this way is you don't have to set all 3 value, you can skip the properties you're not interested in and just set the one you are. And for the ones you skipped, it will just take on the default value. Awesome 👍

![flex](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/27-flex.png)

```text
.child {
  flex: 0 1 auto /* default */
     or <flex-grow> <flex-shrink> <flex-basis>
     or <flex-grow>
     or <flex-basis>
     or <flex-grow> <flex-basis>
     or <flex-grow> <flex-shrink>
}
```

#### [Day 28: align-self](https://github.com/samanthaming/Flexbox30#align-self)

Remember our `align-items` property where we can set the flex item along the cross axis. The thing with `align-items` is that it forces ALL of the flex items to play with the rules. But what if you want one of them to break the rule. No worries, for you independent thinkers, you can use `align-self`. This property accepts all of the same values given to `align-items`, so you can easily break from the pack 😎

![align-self](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/28-align-self.png)

```text
.child-1 {
  align-self: stretch /* default */
           or flex-start
           or flex-end
           or center
           or baseline
}
```

### Summary

#### [Day 29: Flexbox Properties](https://github.com/samanthaming/Flexbox30#flexbox-properties)

YAY!!! You did it! You learned all the properties of Flexbox! You're a Flexbox ninja now! We covered a lot in this short amount of time. Go back and re-visit the ones you still don't understand. Don't just read my Flexbox lessons. Check out other Flexbox tutorials. Sometimes reading a different perspective will help solidify your knowledge and fill in any gaps. Remember the best way to get better is to apply. I gave you the knowledge, now it's on YOU to apply and build something with it 💪

![Flexbox Properties](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/29-flexbox-properties.png)

#### [Day 30: Flexbox Cheatsheet](https://github.com/samanthaming/Flexbox30#flexbox-cheatsheet)

Final tidbit! Let me give you one more tidbit for the road. Memorizing all the available properties is not easy. Even after doing creating this entire tutorial, I still don't have all these properties memorized. Being a good programmer is not about how much you memorize, it's about problem solving. And that's why it's important for a programmer to continue to stay humble and learn. It's all about expanding our toolkit so when we do face a problem, we have a variety of tools that we can select from to fix it 🧰

Congratulation for completing Flexbox30! I hope you learned a lot and thank you for letting my tidbits be part of your programming journey 💛

![Flexbox Cheatsheet](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/30-flexbox-cheatsheet.png)

[**⬆ back to top**](https://github.com/samanthaming/Flexbox30#table-of-contents)

#### [Bonus: Aligning with Auto Margins](https://github.com/samanthaming/Flexbox30#auto-margins)

Bonus content! Another way to align Flexbox child elements is to use auto margins. Although this isn't a Flexbox property, it's still important to be aware of it because it has a very interesting relationship with Flexbox. Check out my code notes on it if you're interested 👉 [Flexbox: Aligning with Auto Margins](https://github.com/samanthaming/Flexbox30/blob/master/flexbox-aligning-with-auto-margins/README.md)

![Flexbox Cheatsheet](https://github.com/samanthaming/Flexbox30/raw/master/code-tidbits/bonus-auto-margins.png)

### 📚 Resources

**Learning Flexbox**

* [MDN web docs: Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)
* [MDN web docs: Basic Concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
* [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [Yoksel: Flex Cheatsheet](https://yoksel.github.io/flex-cheatsheet/)
* [JoniBologna.com: Flexbox Cheatsheet](http://jonibologna.com/flexbox-cheatsheet/)
* [Interneting is hard: Flexbox](https://internetingishard.com/html-and-css/flexbox/)

**Official Spec**

* [W3C: Flexbox](https://www.w3.org/TR/css-flexbox-1/)

**Community Suggestion**

* [Flexbox Zombies](https://flexboxzombies.com/) $
* [Flexbox Froggy](https://flexboxfroggy.com/)
* [Wes Bos: What the Flexbox?!](https://flexbox.io/)

