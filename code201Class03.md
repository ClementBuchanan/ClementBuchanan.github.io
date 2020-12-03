# Summary: Class 03 was learning about making lists in HTML

## HTML provides us with three types of lists to use when making webpages

### Ordered lists

* Each item in the list are numbered
* Uses <> and </> with ol  elements in them
* Each item in the list is denoted with a <> and </> with li in them

### Unordered lists

* These are bulletted and does not indicated order
* A pair of open <> and closed </> tags with ul in them
* Each item in the list also have openand closed tags <> </> with li in them.


### Definition lists

These are made up of a set of terms wioth definitions. Like ordered and unordered lists definitions lists uses open <> and closed </> tags with:

* Created with the dl element between them
* dt between them for signifying the term being used
* dd betwen them signifying the definition

Lists can be nested inside each other

## CSS Boxes

CSS treats each HTML element like it lives in its own box and is has control over that box.

* The box can have different size and shapes
* Can have rounded or square edges
* Can have colors
* CSS can also control the width, height and what displays inside the box

This is a sample code for styling a css box

td.description {
  min-width: 245px;
  max-width: 450px;
  text-align: center;
  padding: 5px;
  margin: 0px;
}

### Javascript Decisions and loop

Three points to consider when creating Jvascript loops

1. They have key words that are specific to them
    1.  Break - Causes the termination of the loop
    1.  Continue - Stops the curent iteration then pdates and check the curent condition again.

Loops can be confusing so you must be careful when writing them. Thre are several types of loops:

- for loops
- while loops
- do while loops
- 


This is an example of a 'for' loop:

var scores = [24, 32, 44, 15];
var arrayLength = scores.length;
var roundNumber = 0;
var message = ' ';
var i;

for (i = 0; i = < array.length; i ++) {
  roundNumber = (i + 1);
  msg += 'round ' + roundNumber + ': ';
  msg += scores[i] + <br />';
}
document.getElementById('answer').innerHTML = msg;

