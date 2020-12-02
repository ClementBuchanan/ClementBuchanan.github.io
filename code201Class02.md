# Class 02


## Text
On a website HTML elements are used to describe structure of te page. Ex. Headings, sub-headings and paragraphs. When creating a webpage markups (tags)
are added to the content of the page to provide extra meaning to the information:

Structural markups are the elements used to describe bothe the headings and the paragraphs. Here are examples of structural markups:

* Headings - There are six headings. H1 - H6. H1 headings are the biggest in size and H6 headings are smaller in size.
* Paragraphs - To create a paragraph the sentences are surounded by an open <>
and a closed </> woth the letter 'p' inside them.
* Bold & Italics - similar to the use of the open and <> and closed </> tags, if a word is to be bold we use the letter 'b' inside the tags. The same goes for italicized words. Use the letter 'i' inside the tags.

Semantec markup are the elements used to provide additional information such as where emphasis is polaced in a sentence. They are not intended to affect the structure of you webpage. Examples pof these are:

* strong - used inside of tags to indicate that the element has high importance.
* em - Used inside of tags indicates emphasis that changes the meaning of the word or sentence is it surrounds.
* abbr -  Abbreviations and acronyms are used with  the 'abbr' inside of tags.

### Introduction To CSS

* What does it do - In a nutshel, css makes the website look pretty. It control the design of the site.

* How does it work - It can be either internal/inline or external. This means that is can be coded into the html page or it can have its own external (css) file.

* Rules and properties - There are many rules and properties to css. Example,

The link property:
  1. File extension is .css
  1. Href - specifies a path to the css file inside the css folder.
  1. Type - atribute that specifies the type of document being linked to.

The style rule:
  1. Allows all pages to use the style rule.
  1. Keeps the content separate from how the page looks.
  1. Means you can changes the style across multiple pages by altering just one page.

  This is an example of a css code:

  body {
    font-family: arial;
    background-color: rgb(233, 125, 10);
    border: 10px;}
  H1 {
    color: rgb(255, 255, 120);
  }

### Basic JavaScript Instructions

Javasript is a set o insructions given for a website to follow. Like any language with words and vocabulary it has syntax and grammar.

* It is a series of instructions to follow one-by-one.
* Javascript is case sensitive.
* Statements can be organized into code blocks.

Here's an example of a javasrcipt code:

var today = newDate();
var hourNow = today.getHour();
var greeting;

if (hourNow > 18) || < 24 ) {
  greeting = 'Good evening';
} else if (hourNow = > 12 || < 18) {
  greeting = 'Good afternoon';
} else if (hourNow = > 0 || < 12) {
  hourNow = 'Good morning';
} else {
  greeting = 'Welcome';
}

docuent.write(greeting);

}

### Decisions and Loops

The flow of data in the script can be handle with evaluations, decisions and loops:

* Evaluations analyze values to determine whether or not they match the expected results.
* Decisions uses the evaluation results to decide which path the evaulation results should take.
* Loops performs the same set of steps repeatedly.

Here's an example of what this looks like:

if (score > 50); {
  document.write('You passed!');
} else {
  document.write ('Please try again.');
}
