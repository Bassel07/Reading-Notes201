# Forms and JS Events

## Duckett HTML book
![img](https://designshack.net/wp-content/uploads/duckettbook-f.jpg)

# Chapter 7: “Forms” 
Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.
HTML borrows the concept of a form to refer to different
elements that allow you to collect information from visitors to
your site.
Whether you are adding a simple search box to your website or
you need to create more complicated insurance applications,
HTML forms give you a set of elements to collect data from
your users. In this chapter you will learn:
* How to create a form on your website
* The different tools for collecting data
* New HTML5 form controls

In addition to enabling users to
search, forms also allow users
to perform other functions
online. You will see forms

when registering as a member
of a website, when shopping
online, and when signing up for
newsletters or mailing lists.

### Why Forms?
The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

Form Controls

![wdefrgthjkiuytrgefdwerthyjuiuytrgewdertyujiy](https://user-images.githubusercontent.com/85109819/124124115-eaf0d500-da2c-11eb-9d6c-dc2bef102674.PNG)

![sssssssssssssssss](https://user-images.githubusercontent.com/85109819/124124377-34412480-da2d-11eb-926b-2461b5552f5a.PNG)


![aaaaaaaaaaaaaaaa](https://user-images.githubusercontent.com/85109819/124124543-66eb1d00-da2d-11eb-9676-668246de9c58.PNG)

![cccccccc](https://user-images.githubusercontent.com/85109819/124124613-808c6480-da2d-11eb-8aea-a5a7c3659309.PNG)

![wwwwwwwww](https://user-images.githubusercontent.com/85109819/124124700-9ef26000-da2d-11eb-81e0-79e26269780b.PNG)


![rrrrrrrr](https://user-images.githubusercontent.com/85109819/124124785-b598b700-da2d-11eb-9934-469753f2e8b3.PNG)

![ffffff](https://user-images.githubusercontent.com/85109819/124124890-d6610c80-da2d-11eb-9885-6512586f3fb5.PNG)

![bergerg](https://user-images.githubusercontent.com/85109819/124125147-2213b600-da2e-11eb-966b-e4941a29e880.PNG)

![wwwwwwwwweeeeeeee](https://user-images.githubusercontent.com/85109819/124125248-3d7ec100-da2e-11eb-86e6-b4bdc97e1add.PNG)

Summary 
* Whenever you want to c XX ollect information from
visitors you will need a form, which lives inside a
<form> element.
   
* Information from a form is sent in name/value pairs.
      
  * Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
      
      * HTML5 introduces new form elements which make it
easier for visitors to fill in forms.
      

# Chapter 14: “Lists, Tables & Forms” 

  There are several CSS properties that
were created to work with specific types
of HTML elements, such as lists, tables,
and forms.
      
 In this chapter you will learn how to:
* Specify the type of bullet point or numbering on lists
* Add borders and backgrounds to table cells
* Control the appearance of form controls
Together, these properties allow you to take finer control over
specific parts of your pages.     

 ##  Summary
   
     * In addition to the CSS p XX roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
      
      * List markers can be given different appearances
using the list-style-type and list-style image
properties.
      
      * Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
      
      * Forms are easier to use if the form controls are
vertically aligned using CSS.
      
      * Forms benefit from styles that make them feel more
interactive.
      

## Duckett JS book
      
# Chapter 6: “Events” 

 ## THREE WAYS TO BIND AN EVENT TO AN ELEMENT    
      
   HTML EVENT HANDLERS
See p251
This is bad practice, but you
need to be aware of it because
you may see it in older code.
Early versions of HTML included
a set of attributes that could
respond to events on the
element they were added to.
The attribute names matched
the event names. Their values
called the function that was to
run when that event occurred.
For example, the following:
<a onclick="hide()">
indicated that when a user
clicked on this <a> element, the
hi de () function would be called.
This method of event handling
is no longer used because it is
better to separate the JavaScript
from the HTML. You should use
one of the other approaches
shown on this page instead.
      
  * TRADITIONAL DOM
EVENT HANDLERS
See p252
DOM event handlers were
introduced in the original
specification for the DOM.
They are considered better than
HTML event handlers because
they let you separate the
JavaScript from the HTML.
Support in all major browsers is
very strong for this approach.
The main drawback is that you
can only attach a single function
to any event. For example, the
submit event of a form cannot
trigger one function that checks
the contents of a form, and a
second to submit the form data if
it passes the checks.
As a result of this limitation, if
more than one script is used on
the same page, and both scripts
respond to the same event, then
one or both of the scripts may
not work as intended.
      
* DOM LEVEL 2 EVENT
LISTENERS
See p254
Event listeners were introduced
in an update to the DOM
specification (DOM level 2,
released in the year 2000).
They are now the favored way of
handling events.
The syntax is quite different and,
unlike traditional event handlers,
these newer event listeners allow
one event to trigger multiple
functions. As a result, there
are less likely to be conflicts
between different scripts that
run on the same page.
This approach does not work
with IE8 (or earlier versions of
IE) but you meet a workaround
on p258. Differences in
browser support for the DOM
and events helped speed
adoption of jQuery (but you
need to know how events work
to understand how jQuery uses
them).
     
      
 ## Summary    
      
  * Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).
      
      * Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.
      
      * When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.
      
      * You can use event delegation to monitor for events
that happen on all of the children of an element.
      
      * The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.
      
      
      
      
      
