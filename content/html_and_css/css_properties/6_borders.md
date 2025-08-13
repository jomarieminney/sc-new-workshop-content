---
title: "Borders"
weight: 6
chapter: false
---

We can also add borders to elements.

Try adding the following to the first image:

{{% notice style="warning" title="Before - Replace this code" %}}
```css
/* Your CSS here */

header img {
	height: 100px;

}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```css
/* Your CSS here */

header img {
	height: 100px;
	border: 1px solid #000000;
}
```
{{% /notice %}}

{{% notice style="warning" title="Test" icon="vial" %}}

You should see a thin black border appear around the first image.

{{% /notice %}}

`border: 1px solid #000;` is short hand for "create a border that is `1px` wide, solid and black.

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Try changing the width and colour of the border.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

There are several different border styles - [here\'s a list of them](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style).
Try changing the style of the border.

{{% /notice %}}

{{% notice style="info" title="Challenge!" icon="lightbulb" %}}

Add a border to each card.

{{% /notice %}}

Here's what your page should look like so far:

![](../../images/animals_borders.jpeg)
