# HTML Images; CSS Color & Text

# HTML Images

HTML Images Syntax
The HTML <img> tag is used to embed an image in a web page.

Images are not technically inserted into a web page; images are linked to web pages. The img tag creates a holding space for the referenced image.

The <img> tag is empty, it contains attributes only, and does not have a closing tag.

The <img> tag has two required attributes:

src - Specifies the path to the image
alt - Specifies an alternate text for the image

### The src Attribute
The required src attribute specifies the path (URL) to the image.

Note: When a web page loads; it is the browser, at that moment, that gets the image from a web server and inserts it into the page. Therefore, make sure that the image actually stays in the same spot in relation to the web page, otherwise your visitors will get a broken link icon. The broken link icon and the alt text are shown if the browser cannot find the image.

### The alt Attribute
The required alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).


* If a browser cannot find an image, it will display the value of the alt attribute

![img](https://lh3.googleusercontent.com/proxy/OAKZcdVuO2GTrky98wHbHNUw09IqgYFwSaum_y4QyrSxQnhGLn-ZR3STuKNdxfogMs3m6XSxwK1W-48Ob3uqLllAuMpn_4WUWOPqUn-3d2dCDyVQt4I)




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
  
  CSS Margin
 CSS margin property defines a margin (space) outside the border.
  
  Link to External CSS
External style sheets can be referenced with a full URL or with a path relative to the current web page.
  
  
  
 ![img](https://www.syncfusion.com/books/w3_css_succinctly/Images/w3-css-colors.png)
  
