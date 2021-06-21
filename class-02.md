# Basics of HTML, CSS & JS

## How to Write a Git Commit Message

The seven rules of a great Git commit message
* Keep in mind: This has all been said before.
* Separate subject from body with a blank line
* Limit the subject line to 50 characters
* Capitalize the subject line
* Do not end the subject line with a period
* Use the imperative mood in the subject line
* Wrap the body at 72 characters
* Use the body to explain what and why vs. how

## Duckett HTML book
![img](https://designshack.net/wp-content/uploads/duckettbook-f.jpg)

When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.
In this chapter we focus on how to add markup to the text that
appears on your pages. You will learn about:

● Structural markup: the elements that you can use to
describe both headings and paragraphs

●Semantic markup: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on


## Text

* Headings 

HTML has six "levels" of
headings:
<h1> is used for main headings
<h2> is used for subheadings
If there are further sections
under the subheadings then the
<h3> element is used, and so
on...
  
  * paragraph
  
  To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.
  
  * Bold & Italic
  
  
  <b> By enclosing words in the tags
<b> and </b> we can make
characters appear bold.
The <b> element also represents
a section of text that would be
presented in a visually different
way (for example key words in a
paragraph) although the use of
the <b> element does not imply
any additional meaning.
    
    <i> By enclosing words in the tags
<i> and </i> we can make
characters appear italic.
The <i> element also represents
a section of text that would be
said in a different way from
surrounding content — such as
technical terms, names of ships,
foreign words, thoughts, or other
terms that would usually be
italicized.
      
      * Superscript & Subscrip
  
      <sup>
The <sup> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.
        
        <sub>
The <sub> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H2
0.
          
          * White Space
          
          In order to make code easier to
read, web page authors often
add extra spaces or start some
elements on new lines.
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.
          
          * Line Breaks & Horizontal Rules
          
          <br />
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag <br />.
          
          <hr />
To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the <hr /> tag.
There are a few elements that
do not have any words between
an opening and closing tag. They
are known as empty elements
and they are written differently.
An empty element usually
has only one tag. Before the
closing angled bracket of an
empty element there will often
be a space and a forward slash
character. Some web page
authors miss this out but it is a
good habit to get into.
          
          
          ## Introducing CSS
          
          CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.
Once you have learned how to write a CSS rule, learning CSS
mostly involves learning the different properties you can use.
So this chapter will:
          
● Introduce you to how CSS works
          
● Teach you how to write CSS rules
          
         
● Show you how CSS rules apply to HTML pages
          
The remaining chapters in this section will look at all of the
various CSS properties you can use.
          
          CSS allows you to create rules that control the
way that each individual box (and the contents
of that box) is presented.
          
          Here you can see a simple web page that is
styled using CSS.
This example uses two documents: the HTML file (example.html)
and a separate CSS file (example.css). The fifth line of HTML uses the
<link> element to indicate where the CSS file is located.
On the next page, you will see how CSS rules can also be placed in your
HTML pages and we will discuss when you might want to do this.
<!DOCTYPE html>
<html>
<head>
 <title>Introducing CSS</title>
 <link href="css/example.css" type="text/css"
 rel="stylesheet" />
</head>
<body>
 <h1>From Garden to Plate</h1>
 <p>A <i>potager</i> is a French term for an
 ornamental vegetable or kitchen garden ... </p>
 <h2>What to Plant</h2>
 <p>Plants are chosen as much for their functionality
 as for their color and form ... </p>
</body>
</html>
body {
font-family: Arial, Verdana, sans-serif;}
h1, h2 {
color: #ee3e80;}
p {
color: #665544;}
          
   
  ## Duckett JS book
          
   ![img](https://i.ytimg.com/vi/wrtqiTl2Xuo/maxresdefault.jpg)
          
         
          
    ##   Basic JavaScript Instructions
          
      *  THE LANGUAGE:
SYNTAX AND GRAMMAR
like any new language, there are new
words to learn (the vocabulary) and rules
for how these can be put together (the
grammar and syntax of the language).
          
          
          * GIVING INSTRUCTIONS:
          FOR A BROWSER TO FOLLOW
Web browsers (and computers in general)
approach tasks in a very different way than
a human might. Your instructions need to
reflect how computers get things done. 
          
          

          ## Decisions and Loops
         
          
          Looking at a flowchart (for all but the most basic scripts),
the code can take more than one path, which means the
browser runs different code in different situations. In this
chapter, you will learn how to create and control the flow of
data in your scripts to handle different situations. 
          
          Scripts often need to behave differently depending upon how the user interacts with the web
page and/or the browser window itself. To determine which path to take, programmers often
rely upon the following three concepts:
          
          * EVALUATIONS
You can analyze values in
your scripts to determine
whether or note they
match expected results.
          
          * DECISIONS
Using the results of
evaluations, you can
decide which path your
script should go down.
          
          * LOOPS
There are also many
occasions where you will
want to perform the same
set of steps repeatedly. 
          
          
