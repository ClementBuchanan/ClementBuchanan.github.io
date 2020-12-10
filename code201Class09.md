# Forms and JS Events

## Chapter 7: “Forms” (p.144-175)

To collect information od any website e use forms which lives inside a forms element. For example, during user registration an a site you would like to collect information such as name, email address, credit card, etc.

A form will take input from the site visitor and then will post it to a back-end application such as ASP Script or PHP script etc. The back-end application will perform required processing on the passed data based on defined logic inside the application.

Here's an example of the HTML <form> tag that is used to create an HTML form and it has following syntax 

<form action = "Script URL" method = "GET|POST">
   form elements like input, textarea etc.
</form>

**Form Attributes**

Apart from common attributes, following is a list of the most frequently used form attributes −
There are various form elements available like text fields, textarea fields, drop-down menus, radio buttons, checkboxes, etc.

1. Action - Backend script ready to process your passed data.
1. Method - Method to be used to upload data. The most frequently used are GET and POST methods.
1. Target - Specify the target window or frame where the result of the script will be displayed. It takes values like _blank, _self, _parent etc.

**HTML Form Controls**

There are different types of form controls that you can use to collect data using HTML form −

1. Text Input Controls
1. Checkboxes Controls
1. Radio Box Controls
1. Select Box Controls
1. File Select boxes
1. Hidden Controls
1. Clickable Buttons
1. Submit and Reset Button

## Chapter 14: “Lists, Tables & Forms” (pp.330-357)

The HTML tables allow web authors to arrange data like text, images, links, other tables, etc. into rows and columns of cells. The HTML tables are created using the **table** tag in which the **tr** tag is used to create table rows and **td** tag is used to create data cells. The elements under **td** are regular and left aligned by default.

<!DOCTYPE html>
<html>

   <head>
      <title>HTML Tables</title>
   </head>
	
   <body>
      <table border = "1">
         <tr>
            <td>Row 1, Column 1</td>
            <td>Row 1, Column 2</td>
         </tr>
         
         <tr>
            <td>Row 2, Column 1</td>
            <td>Row 2, Column 2</td>
         </tr>
      </table>
      
   </body>
</html>

It produces a table with two rws and two columns.


## Chapter 6: “Events” (pp.243-292)

JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page. 

- When the page loads, it is called an event. 
- When the user clicks a button, that click too is an event. 
- Other examples include events like pressing any key, closing a window, resizing a window, etc.

**Types of events**

- onclick Event - This is the most frequently used event type which occurs when a user clicks the left button of his mouse
- onsubmit Event - onsubmit is an event that occurs when you try to submit a form
- onmouseover and onmouseout - These two event types will help you create effects with images or even with text. The onmouseover event triggers when you bring your mouse over any element and the onmouseout triggers when you move your mouse out from that element. 