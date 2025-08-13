---
title: "Fonts"
weight: 5
chapter: false
---

There are a lot of different things we can do with fonts, including changing their family and size.

## Family

Head over to [Google Fonts](https://fonts.google.com/) and pick out a font that you like.

Select that font then view all your selected fonts:

![Screenshot of Google Font.](../../images/fonts_1.png)

Select the `@import` option:

![Screenshot of how to use Google Font](../../images/fonts_2.png)

Copy the code **between the `<style>` tags**.

Paste this code at the **top of your css file**.

```css {title="css"}

/* Your fonts here */
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
/* */
```

Then head back to Google Fonts and copy the `font-family` line of code.

Let's style our headings with your selected font:

```css {title="css"}
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;
}

h2 {
	font-family: 'Pacifico', cursive;
}

h3 {
	font-family: 'Pacifico', cursive;
}
```

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Find another font to use for the nav, footer and paragraphs.

{{% /notice %}}

## Size

Let's try changing the size of our text too.

Add the following to your CSS:

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;

}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

h1 {
	font-family: 'Pacifico', cursive;
    font-size: 50px;
}
```
{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the font size of the `h2`, `h3`, and `p` tags.

{{% /notice %}}

## Colour

We can change the color of our fonts using the `color` attribute.

Add the following to your CSS:

```css {title="css"}
/* Your CSS here */

a {
	color: #ffffff;
}
```

{{% notice style="warning" title="Test" icon="vial" %}}

The colour of the `a` tags in the `nav` should turn white.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the colour of the `h1`, `h2` and `h3` headings.

{{% /notice %}}

Here's what your page should look like so far (using your own fonts):

![](../../images/animals_fonts.jpeg)
