---
layout: post
title:  "Basics of Javascript functions"
date:   2017-08-25 12:38:31 -0400
---


This blog is a summary on the basics of using functions in Javascript.  Learning functions was confusing for me at first, especially coming from learning a different programming language (Ruby) at the beginning of this online course.  Hopefully, this blog will solidify understanding what functions are and how they work.
  
A Javascript function is a block of code designed to perform a particular task.  Functions give the JavaScript interpreter code instructions that it can run over and over again.  Functions are written, known as *declaring*, with the function keyword.  When a function is declared, start with the function keyword, followed by a name for the function, followed by a pair of parentheses, and then a pair of curly braces.  Function instructions are placed between the curly braces; which is known as the function body.  

**Declare Example: **
‘function functionName() {
	instructions in function body
};

When a function's instructions are executed, that is known as *calling* the function.  When you declare the function, nothing happens. That's because the function has to be called with () like so:

**Call Example:**
‘functionName()’

Parameters are placeholders that  put between the parentheses when declaring the function. 

**Declare Example: **
‘function functionName(parameterName) {
	instructions in function body
};

Arguments can pass (some information or value) to a function between its parentheses.  When the function is called (invoked),  you can pass any argument(s) to the invocation that get stored as local, function-level variables that are available anywhere in the function body. 

**Call Example:**
 ‘functionName(argument)’

To summarize, the argument(s) = actual values that  pass to the function, and the parameter(s) = named references where those passed-in values are stored. An argument can be any JavaScript expression — any piece of JavaScript code that evaluates to a value — from something as simple as ‘5’ or ‘string’ to something as complex as an entire function. If there are any argument(s) called, the number of arguments and its order should match the original number and order of the parameters.  

Arguments can only be accessed within the body of the function by referring to the parameter name; what is called a  ‘template literal’ like in the following example: console.log(`${parameterName}!`) .   If  you try to call a parameter name outside of its function in the JavaScript console, a ReferenceError comes up that the parameterName is ‘not defined.’

When JavaScript reaches a **return statement**, the function will stop executing.  If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.  The command return ends the execution inside the function, meaning that if  ‘return’, nothing will happen after that.  When  ‘return’ inside a function, the value is given back entirely outside the function.  When  you call a function in the browser's console, the browser always tells us what the function returns.

Functions in JavaScript are** first-class objects**, which means  you can treat them just as  you would numbers, strings, arrays, and other JavaScript objects. Functions can be:

•	*stored in variables, 
•	passed as arguments to functions, referred as callbacks,
•	created within functions and 
•	returned from functions.*

Functions in JavaScript are** first-class functions**, meaning you have the ability to *pass functions as arguments* to values for other functions.  When  you want to pass a function as a value,  pass it by reference, by omitting the parentheses.  Because of this process of calling back,  “functions that  pass to other functions” as referred to as callbacks.  That's because they're called back after the body of the function they're passed to is completed.  Callbacks are mostly used for asynchronous operations.

Here is a callback example.  The main function (mainFn()) that receives the callback function (callbackFn()) as an argument will invoke the passed-in callbackFn() at some later point, perhaps waiting until other processes have completed or until data that the callbackFn() relies upon becomes available.  You define a callback function but delegate control of when it should be invoked to another function.

**Closure** is a function that has access to the variables (i.e. parameters and regular variables) and methods declared in the parent scope, even after the parent function has been executed.  You can use closures to emulate 'private' variables and methods, as well as use them to make creating certain functions quicker and more dynamic.

An **in-line function** is a function that is the first (and only) parameter of the parent function. However, that function doesn't have to be defined beforehand.  You can pass what's called an anonymous function, that has no name.  As an example, innerFunction() is an inner function of the outerFunction() function, and as such, it has access to all of the variables defined in its parent function (along with any variables in its own scope, if it has any). This means that you
can access the variable argument in our innerFunction() function. However, variable isn't accessible outside of outerFunction() function, giving us some semblance of 'private' variables. This is one possible use case for closures.  The reason innerFunction() still has access to the variables within its parent function long after the parent function has executed is because innerFunction() is a 'closure'.

When a closure is created, its environment is remembered and not discarded. That means that the variables in that scope are shared (just like regular variables), and can also be changed.  Keep in mind that it is now returning an object with references  inner() and other() functions, meaning that now  you do need to use the key names to refer to them.  A closure also provides a shortcut where the name of the variable is the same as the name of the key of the object.  Closures are the most common source of performance issues and memory leaks.

Hope this is a helpful blog!  Thank you for reading!


