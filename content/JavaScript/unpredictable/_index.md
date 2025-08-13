---
title: "So Unpredictable!"
weight: 10
chapter: false
---

To properly mix everything up so our game isn't too predictable, we also want the cupcakes to stay up for a random period of time rather than always for 500ms (or maybe 1000ms if our random number generator picks the same cupcake twice).

To do this we'll write a function which will take a minimum and a maximum value, and randomly choose a number between the two. At the bottom of your code, let's add a new function called `randomTime`:

```js {title="js"}
function randomTime(min, max) {
    let time = Math.round(Math.random() * (max - min) + min);

    return time;
}
```

{{% notice info %}}

**What is Math.random()?**
Good question, `Math.random()` produces a number between 0 (inclusive) and 1 (exclusive). So multiplying the random number by (max - min) and then adding min shifts the random value to lie between your desired minimum and maximum values.


**What is Math.round()?**
To convert the decimal into an integer, we use `Math.round()`. This rounds to the nearest whole number, which is acceptable for this scenario. There are alternative methods if you need more [rounding](https://javascript.info/number#rounding) precision.

{{% /notice %}}


We can then use our `randomTime` function to randomly pick a time interval. In the example below we've set the minimum as 200ms and the maximum as 1,000ms (1s).

{{% notice style="warning" title="Before - Replace this code" %}}
```js
function popUp() {
	let hole = randomHole(holes);
	let time = 500;

	hole.classList.add('up');

	setTimeout(function() {
		hole.classList.remove('up');

		if(timeUp == false) {
				popUp();
		}
	}, time)
}
```
{{% /notice %}}

{{% notice style="tip" title="After - Updated code" %}}
```js
function popUp() {
	let hole = randomHole(holes);
	let time = randomTime(200, 1000);

	hole.classList.add('up');

	setTimeout(function() {
		hole.classList.remove('up');

		if(timeUp == false) {
				popUp();
		}
	}, time)
}
```
{{% /notice %}}

Now run your game again, and you should see the cupcakes are a lot less predictable!

## Check your code!

This is what you should have in CodePen so far:

```js {title="js"}
let timeUp = false;
let holes = document.querySelectorAll('.hole');
let scoreBoard = document.querySelector('.score');
let score = 0;

function startGame() {
    timeUp = false;
    score = 0;
    scoreBoard.textContent = score;
    popUp();

    setTimeout(endGame, 10000);
}

function endGame() {
    timeUp = true;
}

function popUp() {
    console.log('Here I am!');
    let hole = randomHole(holes);
    let time = randomTime(200, 1000);

    hole.classList.add('up');

    setTimeout(function () {
        hole.classList.remove('up');

        if (timeUp == false) {
            popUp();
        }
    }, time);
}

function randomHole(holes) {
    let holeNumber = Math.floor(Math.random() * holes.length);
    let hole = holes[holeNumber];

    return hole;
}

function smash(cupcake) {
    console.log('smashed!');

    cupcake.parentNode.classList.remove('up');
    score = score + 1;
    scoreBoard.textContent = score;
}

function randomTime(min, max) {
    let time = Math.round(Math.random() * (max - min) + min);

    return time;
}
```
