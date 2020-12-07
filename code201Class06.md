# Summary of the "Problem Domain", "Objects Literals" and the "Document Object Model" (DOM).

## The Problem Domain

The problem domain basically explains that one cannot fix if one does not understand what needs fixing. Software engneering is tedious work. A lot of time and energy goes into doing this work. To be efficient and effective software developers must first undertand the problem thu and thru before starting to write code. Coding is not a one size fit all kind of work. The approach to getting things done is very dynamic with many moving parts. There is team work, there is iterations of the code being written. there is testing of the code to see if it works and more. Imaging given unclear instructions and documentation on what is needed, developers then begin working on phase one a project only to be told that is NOT what is needed. This is the reason why it is important to "be one' with the problem domain. 

## Chapter 3: “Object Literals” (pp.100-105)

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code. Literal notation is the easiest and most popular way to create objects. Here's an example code as taken from the text. This code starts by creating  an object using literal notation.

var hotel = {
  name: 'Quay',
  rooms: 40,
  booked: 25,
  checkAvailability: function(){
    return this.rooms - this.booked;
  }
};

var elName=document.getElementById('HotelName');
elName.textContent = Hotel.name;

var elRooms = document.getElementById ('Rooms');
elRooms.textContent = hotel.checkAvailability();

The object is called a hotel represented by the name Quay with 40 rooms, 25 of them being booked. The hotel's website will be updated with data from this object. It will show the hotel's name by accessing the objects name property. It wil show the number of vacant rooms by using the checkAvailability() method.

## Chapter 5: “Document Object Model” (pp.183-242)

Document Object Model specifies how a browsers should create a model of the HTML page and how javscript can access and update its content. The DOM cover two major areas:

1. Making the model of the HTML page
1. Accessing and changing the HTML page

A browser takes a snapshot of a webpage's DOM and stores it in it's memory. This is called a DOM tree. This is what it looks like (like an org chart):

![](images/Dom-Tree.png)

The DOM tree has four types of nodes:

1. The document node - repersenting the entire page with every element on it.
1. The elements node - To access the DOM tree yo start by looking for element. When they are found you can acces its text and attribute node.
1. The attribute node - You can acces the attribute node to change css values.
1. Text node - Once you have access to the element node you can access the text nodes.
