# Focus style

{% embed url="https://zellwk.com/blog/creating-focus-style" %}

When you create a custom focus style, you want to think about four things:

1. Adding an outline
2. Creating animations that contain movement
3. Changing the background color
4. Changing the text color

I wrote more about this in my article on [designing focus](https://zellwk.com/blog/create-focus-style). During my research, I found three kinds of focus style I liked.

1. The one on Smashing Magazine
2. The one on WTF Forms
3. The one on Slack

![Focus styles on Smashing Mag, WTF Forms and Slack](https://zellwk.com/images/2019/create-focus/combined.png)

Today, I want to show you how to create these focus styles and use them effortlessly across your website.

### Creating the focus for Smashing Magazine <a id="creating-the-focus-for-smashing-magazine"></a>

Smashing Magazine uses a large dotted outline for focus. To create this focus style, you set the `outline` property to `3px dotted`.

![Focus styles on Smashing Magazine.](https://zellwk.com/images/2019/create-focus/smashing.png)

```css
*:focus {
  outline: 3px dotted #761b15;
}
```

If you want to change the color of the outline, you can change the `outline-color` property.

```css
.red-background *:focus {
  outline-color: white;
}
```

Alternatively, you can use CSS Variables.

```css
:root {
  --outline-color: #761b15;
}

*:focus {
  outline: 3px dotted var(--outline-color);
}

.red-background {
  --outline-color: white;
}
```

### Creating focus styles for WTF Forms <a id="creating-focus-styles-for-wtf-forms"></a>

The focus style for WTF forms contains two parts:

1. A white border
2. A blue border

![Focus styles for WTF Forms.](https://zellwk.com/images/2019/create-focus/wtf.png)

This style can be created with `box-shadow`. The idea is you create two shadows:

1. The first shadow with the background’s color
2. The second shadow with the focus’s color

```css
*:focus {
  outline: none;
  box-shadow: 0 0 0 .075rem #fff, 
              0 0 0 .2rem #0069d4;  
}
```

If you want to change the focus color, you need to rewrite the entire `box-shadow`.

```css
.blue-background *:focus {
  outline: none;
  box-shadow: 0 0 0 .075rem #0069d4, 
              0 0 0 .2rem #fff;  
}
```

Note: WTF Forms does not have styles for links and buttons. Only form elements. It doesn’t have styles for a darker background either. I created this demo according to what I thought looks okay.

There’s an easier way. If you used CSS variables, you only need to switch the colors.

```css
:root {
  --focus-inner-color: #fff;
  --focus-outer-color: #0069d4;
}

*:focus {
  outline: none;
  box-shadow: 0 0 0 .075rem var(--focus-inner-color), 
              0 0 0 .2rem var(--focus-outer-color);
}

.blue-background {
  --focus-inner-color: #0069d4;
  --focus-outer-color: #fff;
}
```

### Creating focus styles for Slack <a id="creating-focus-styles-for-slack"></a>

The focus style on Slack contains two parts:

1. A dark blue outline
2. A light-blue border

![Focus styles on Slack.](https://zellwk.com/images/2019/create-focus/slack.png)

This focus style can be created with the same technique as WTF Forms.

```css
*:focus {
  outline: none;
  box-shadow: 0 0 0 2px hsla(210, 52%, 42%, 1.00), 
              0 0 0 .6rem hsla(200, 72%, 83%, 0.75);
}
```

The CSS Variables trick works wonders if you need to change colors.

```css
:root {
  --focus-inner-color: hsla(210, 52%, 42%, 1.00);
  --focus-outer-color: hsla(200, 72%, 83%, 0.75);
}

*:focus {
  outline: none;
  box-shadow: 0 0 0 2px var(--focus-inner-color), 
              0 0 0 .6rem var(--focus-outer-color);
}

.dark {
  --focus-inner-color: hsla(0, 0%, 100%, 0.75);
  --focus-outer-color: hsla(0, 0%, 100%, 0.25);
}
```

If you use this technique on elements with borders, you might want to remove the borders. It’s not pretty to see two stacking borders.

![](https://zellwk.com/images/2019/create-focus/double-borders.png)

```css
button:focus {
  border-color: transparent;
}
```

### Combined demo <a id="combined-demo"></a>

I combined the different methods onto one demo for you to play with. Here it is:

Thanks for reading. Did this article help you out? If it did, I hope you consider [sharing it](https://twitter.com/share?text=Creating%20a%20custom%20focus%20style%20by%20@zellwk%20%F0%9F%91%87%20&url=https://zellwk.com/blog/creating-focus-style/). You might help someone else out. Thanks so much!

