# JS Debugging

Ch 10 : Error Handling & Debugging

![img](https://i.ytimg.com/vi/wrtqiTl2Xuo/maxresdefault.jpg)


### UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code

If you are anticipating that something in your code
may cause an error, you can use a set of statements
to handle the error (you meet them on p480).
This is important because if the error is not handled,
the script will just stop processing and the user will
not know why. So exception-handling code should
inform users when there is a problem.
       
Whenever the interpreter comes across an error,
it will look for error-handling code. In the diagram
below, the code has the same structure as the code
you saw in the diagrams at the start of the chapter.
The statement at step 1 uses the function in step 2,
which in turn uses the function in step 3. Imagine
that there has been an error at step 3.
       
When an exception is thrown, the interpreter
stops and checks the current execution context for
exception-handling code. So if the error occurs in the
getName () function (3), the interpreter starts to look
for error handling code in that function.
       
If an error happens in a function and the function
does not have an exception handler, the interpreter
goes to the line of code that called the function.
In this case, the get Name () function was called by
greetUser(), so the interpreter looks for exceptionhandling
code in the greetUser() function (2).
If none is found, it continues to the next level,
checking to see if there is code to handle the error
in that execution context. It can continue until it
reaches the global context, where it would have to it
terminate the script, and create an Error object.
       
 So it is going through the stack looking for errorhandling
code until it gets to the global context.
If there is still no error handler, the script stops
running and the Error object is created.
       
### ERROR OBJECTS CONTINUED 

Syntax Error
SYNTAX IS NOT CORRECT
This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.
MISMATCHING OR UNCLOSED QUOTES
document .write ("Howdyl );
SyntaxError: Unexpect ed EOF

MISSING CLOSING BRACKET
document .getElementByid('page' I
SyntaxErr or : Expected token ' ) '
MISSING COMMA IN ARRAY
Would be same for missing] at the end
var l ist = ['Item 1', 'Item 2 ' l 'rtem 3'];
SyntaxError: Expected token ']'

MALFORMED PROPERTY NAME
It has a space but is not surrounded by quote marks
user = { f i rstl name: "Ben", lastName: "Lee"};
Synt axError: Expected an identifier but
found 'name ' instead

Ref erenceError
VARIABLE DOES NOT EXIST
This is caused by a variable that is not declared or is
out of scope.
VA RIABLE IS UNDECLARED
var wi dth = 12 ;
var area = width * llt!ftNU! ;
ReferenceError: Can ' t find vari able:
height

NAMED FUNCTION IS UNDEFINED
document.write ( randomFunction() ) ;
ReferenceError: Can't find variable :
randomFunction

EvalError
INCORRECT USE OF eval() FUNCTION
The eva l () function evaluates text through the
interpreter and runs it as code (it is not discussed
in this book). It is rare that you would see this type
of error, as browsers often throw other errors when
they are supposed to throw an Eva 1 Error.
                         
 URI Error
INCORRECT USE OF URI FUNCTIONS
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;
CHARACTERS ARE NOT ESCAPED
decodeURI('http: //bbc . com/ news . phplla=l') ;
URlError: URI error


Type Error
VALUE IS UNEXPECTED DATA TYPE
This is often caused by trying to use an object or
method that does not exist.
INCORRECT CASE FOR document OBJECT
l!Jocument.wri te ( 'Oops! ');
TypeError: 'undefined' is not a funct ion
(eval uating 'Document.write('Oops! ')')
INCORRECT CASE FOR write() METHOD
document. eJrite('Oops ! ') ;
TypeError: 'undefined' is not a function
(evaluating 'document.Write( 'Oops! ') ')
METHOD DOES NOT EXIST
var box = {};
box .@Mi}id ;
II Create empty object
II Try to access getArea()
TypeError: 'undefined ' is not a function
(evaluating 'box.getArea()')
DOM NODE DOES NOT EXIST
var el = document .getElementByid(llll ) ;
el.innerHTML = 'Mango';
TypeError: 'null' is not an object
(evaluating 'el .innerHTML = 'Mango'')
                         
Error
GENERIC ERROR OBJECT
The generic Error object is the template (or
prototype) from which all other error objects are
created.
                         
RangeError
NUMBER OUTSIDE OF RANGE
If you call a function using numbers outside of its
accepted range.
CANNOT CREATE ARRAY WITH -1 ITEMS
var anArray = new Array(~);
RangeError : Array si ze is not a smal l
enough positive integer
NUMBER OF DIGITS AFTER DECIMAL IN
tofhed() CAN ONLY BE 0-20
var price = 9.99;
price.toFixed( fJI );
RangeError: toFixed() argument must be
between 0 and 20
NUMBER OF DIGITS IN toPrecision() CAN
ONLY BE 1-21
num = 2.3456;
num.toPrecisi on(flJ ) ;
RangeError: toPrecision() argument must
be between 1 and 21
                         
  NaN
NOT AN ERROR
Note: If you perform a mathematical operation using
a value that is not a number, you end up with the
value of NaN, not a type error.
NOT A NUMBER
var t otal = 3 * lilllJil;
                         
 # HOW TO DEAL WITH ERRORS
                         
  Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors.
                         
  1: DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)
IE and Safari also have their own tools (but there is
not space to cover them all).
                         
2: HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement s.
Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.
In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and
offer an alternative option if it fails.
                         
 # SUMMARY
                         
* If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
                         
* Debugging is the process of finding errors. It involves a
process of deduction.
                         
* The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
                         
* JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
                         
* If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.
                         


                         
                         
                         

       
       
       
       
       
       
       
       
       
 
       
       
