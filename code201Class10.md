# Ch. 10, “Error Handling & Debugging”

There are three types of errors in programming: (a) Syntax Errors, (b) Runtime Errors, and (c) Logical Errors.

## Syntax Errors

Syntax errors, also called parsing errors at interpret time in JavaScript.

For example, the following line causes a syntax error because it is missing a closing parenthesis.

<script type = "text/javascript">
      window.print(;
</script>

When a syntax error occurs in JavaScript, only the code contained within the same thread as the syntax error is affected and the rest of the code in other threads gets executed assuming nothing in them depends on the code containing the error.

## Runtime Errors

Runtime errors, also called exceptions, occur during execution (after compilation/interpretation).

For example, the following line causes a runtime error because here the syntax is correct, but at runtime, it is trying to call a method that does not exist.

<script type = "text/javascript">
      window.printme();
</script>

Exceptions also affect the thread in which they occur, allowing other JavaScript threads to continue normal execution.

## Logical Errors

Logic errors can be the most difficult type of errors to track down. These errors are not the result of a syntax or runtime error. Instead, they occur when you make a mistake in the logic that drives your script and you do not get the result you expected.

You cannot catch those errors, because it depends on what type of logic you want to put in your program.

## The try...catch...finally Statement

The latest versions of JavaScript added exception handling capabilities. JavaScript implements the try...catch...finally construct as well as the throw operator to handle exceptions.

You can catch programmer-generated and runtime exceptions, but you cannot catch JavaScript syntax errors.

Here is the try...catch...finally block syntax

<script type = "text/javascript">
      try {
         // Code to run
         [break;]
      } 
      catch ( e ) {
         // Code to run if an exception occurs
         [break;]
      }
      [ finally {
         // Code that is always executed regardless of 
         // an exception occurring
      }]
</script>

The try block must be followed by either exactly one catch block or one finally block (or one of both). When an exception occurs in the try block, the exception is placed in e and the catch block is executed. The optional finally block executes unconditionally after try/catch.