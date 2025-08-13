---
title: "Can't Catch Me!"
weight: 5
chapter: false
---

## Popping the cupcake Back Down - Timing is Everything!

Now that we've got our cupcake jumping out of its hole, we also need to get the cupcake to pop back down again to make smashing it a little trickier! We do this by simply removing the `up` class we added earlier to our `popUp` function.

{{% notice style="warning" title="Before - Replace this code" %}}
```js
function popUp() {
	let hole = holes[0];
	hole.classList.add('up');
}
```

{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```js
function popUp() {
	let hole = holes[0];
	hole.classList.add('up');
	hole.classList.remove('up');
}
```
{{% /notice %}}

Press **Start**, what happens? Did you see it appear? Our code is running a little too fast for us to see! The cupcake is appearing and then immediately disappearing again, let's slow things down.

We're going to set a time for how long we want the `up` class to stay with our cupcake.

{{% notice style="warning" title="Before - Replace this code" %}}
```js
function popUp() {
	let hole = holes[0];
	hole.classList.add('up');
	hole.classList.remove('up');
}
```
{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```js
function popUp() {
	let hole = holes[0];
	let time = 500;
	hole.classList.add('up');
	setTimeout(function() {
		hole.classList.remove('up');
 }, time)
}
```
{{% /notice %}}

> **Introducing a Delay:** 
> 
> By using the `setTimeout` function we can tell JavaScript, "Hey, wait a little while - say, 500 milliseconds (that's half a second!) - and then hide the cupcake. This delay is stored in a variable called `time`.


You should now be able to see the cupcake appearing and disappearing when you start the game.

Try changing the value of `time` and see what happens (remember, this value is in milliseconds, so 500 milliseconds is 0.5 seconds).

{{% notice style="tip" title="Tip" %}}

If your code doesn't work as expected, check your brackets! In JavaScript brackets should always have partners. This goes for parentheses(), square brackets[] and braces{} - just count the left ones and make sure they all have a buddy.

{{% /notice %}}

## Check your code!

This is what you should have in CodePen so far:

```js {title="js"}
let timeUp = false;
let holes = document.querySelectorAll('.hole');
let scoreBoard = document.querySelector('.score');

function startGame() {
    timeUp = false;
    popUp();
    setTimeout(endGame, 10000);
}

function endGame() {
    timeUp = true;
}

function popUp() {
    let hole = holes[0];
    let time = 500;
    hole.classList.add('up');
    setTimeout(function () {
        hole.classList.remove('up');
    }, time);
}
```
