# Learning Journal 4

# Functions 

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}



Function parameters are listed inside the parentheses () in the function definition.

Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.



Function Invocation
The code inside the function will execute when "something" invokes (calls) the function:

* When an event occurs (when a user clicks a button)
* When it is invoked (called) from JavaScript code
* Automatically (self invoked)


Function Return
When JavaScript reaches a return statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.


Functions often compute a return value. The return value is "returned" back to the "caller":


## Why Functions?
You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

## The () Operator Invokes the Function
Using the example above, toCelsius refers to the function object, and toCelsius() refers to the function result.

Accessing a function without () will return the function object instead of the function result.

## Functions Used as Variable Values
Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

![img](https://cdn.programiz.com/sites/tutorial2program/files/javascript-recursion.png)


# CSS

## What is CSS?
Cascading Style Sheets (CSS) is used to format the layout of a webpage.

With CSS, you can control the color, font, the size of text, the spacing between elements, how elements are positioned and laid out,
what background images or background colors are to be used, different displays for different devices and screen sizes, and much more!

### Using CSS
CSS can be added to HTML documents in 3 ways:

* Inline - by using the style attribute inside HTML elements
* Internal - by using a <style> element in the <head> section
* External - by using a <link> element to link to an external CSS file
The most common way to add CSS, is to keep the styles in external CSS files. However, in this tutorial we will use inline and internal styles, because this is easier to demonstrate, and easier for you to try it yourself.
  
 * Inline CSS
An inline CSS is used to apply a unique style to a single HTML element.

An inline CSS uses the style attribute of an HTML element.
  
 * Internal CSS
An internal CSS is used to define a style for a single HTML page.

An internal CSS is defined in the <head> section of an HTML page, within a <style> element.
  
  * External CSS
An external style sheet is used to define the style for many HTML pages.
  
  The external style sheet can be written in any text editor. The file must not contain any HTML code, and must be saved with a .css extension.
  
###  CSS Colors, Fonts and Sizes
Here, we will demonstrate some commonly used CSS properties. You will learn more about them later.

The CSS color property defines the text color to be used.

The CSS font-family property defines the font to be used.

The CSS font-size property defines the text size to be used.
  
### CSS Border
The CSS border property defines a border around an HTML element.

Tip: You can define a border for nearly all HTML elements.
  
### CSS Padding
The CSS padding property defines a padding (space) between the text and the border.
  
 ### CSS Margin
The CSS margin property defines a margin (space) outside the border.
  
 ### Link to External CSS
External style sheets can be referenced with a full URL or with a path relative to the current web page.
  
  
  


# Branches 
  
  
using windows terminal 

  to creat and switch branch:
  git checkout -b "problem"
  code .   (make the changes in the vs)
  
  git add .
  git commit -m 'problem'
  git push origin problem
  
  make a pull request and merge
  
  git checkout main
  get pull origin main
  
  
  
  
  




