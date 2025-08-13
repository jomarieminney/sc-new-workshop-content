---
title: "Colour"
weight: 3
chapter: false
---

The next thing we'll do is add some colour.
This will also help us to see where one section ends and another starts.

Add the following

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */

nav {
	text-align: right;

}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

nav {
	text-align: right;
	background-color: #87CEEB;
}
```
{{% /notice %}}

{{% notice style="warning" title="Test" icon="vial" %}}

The nav element should turn blue.

{{% /notice %}}

## Colours in CSS

Did you notice how we defined our colour.
We used a strange code instead (`#87CEEB`).
This is called a **Hex Code**, which is a 6 character code for representing colours which works in CSS.

There are several different ways of representing colours in CSS.

For example, there are some **name colours**.
The hex code we've used also has the name `skyblue`.

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Try changing the `background-color` to use `skyblue` instead of the hex code.

{{% /notice %}}

There only a few **named colours** in (216 to be exact!).
That might sound like a lot, but if we use hex codes instead that opens us up to over 16 MILLION colours instead!

We can also represent colours using **RGB codes** too.
For example, `skyblue` is represented as `rgb(135, 206, 235)` in RGB.

For the full list of named colours [check out this site,](https://htmlcolorcodes.com/color-names/) or use a [colour picker.](https://htmlcolorcodes.com/color-picker/)

## Colouring our Page

Let's get back to our CSS!

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */

nav {
	text-align: right;
	background-color: #87CEEB;
}


```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

nav {
	text-align: right;
	background-color: #87CEEB;
}

#section-3 {
	background-color: #885A89;
}
```
{{% /notice %}}

{{% notice style="warning" title="Test" icon="vial" %}}

The background colour behind the cards should be purple.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the background colour of each card to `white`. Bonus: can you find the hex code for `white`?

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the background colour of the each column in `section-5`.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Change the background colour of the `footer`.

{{% /notice %}}

Here's what your page should look like so far:

![](../../images/animals_colour.jpeg)
