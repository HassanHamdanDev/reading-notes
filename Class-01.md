

# Introductory HTML and JavaScript

### Introduction 

1. HTML

*We will spend the first chapter looking at how HTML is used to create web pages. You will see that you start by writing down the words you want to appear on your page. You then add tags or elements to the words so that the browser knows what is a heading, where a paragraph begins and ends, and so on.*


2. CSS

*Presentation: How to control things like the color of text, the fonts you want to use and the size of those fonts, how to add background colors to pages , and how to add background images.*


3. Practical

*We end up with some helpful information that will assist you in building better websites.*
*We look at some new tags that will be introduced in HTML5 to help describe the structure of your pages*

### Structure

* HTML pages are text documents.
* HTML uses tags (characters that sit inside angled 
brackets) to give the information they surround special 
meaning.
* Tags are often referred to as elements.
* Tags usually come in pairs. The opening tag denotes 
the start of a piece of content; the closing tag denotes 
the end.
* Opening tags can carry attributes, which tell us more 
about the content of that element.
* Attributes require a name and a value.
* To learn HTML you need to know what tags are 
available for you to use, what they do, and where they 
can go.

### Extra Markup

```
- DOCTYPES tell browsers which version of HTML you 
are using.
- You can add comments to your code between the 
<!-- and --> markers.
- The id and class attributes allow you to identify 
particular elements.
- The <div> and <span> elements allow you to group 
block-level and inline elements together.
- <iframes> cut windows into your web pages through 
which other pages can be displayed.
- The <meta> tag allows you to supply all kinds of 
information about your web page.
- Escape characters are used to include special 
characters in your pages such as <, >, and ©

```

### HTML5 Layout

*The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.*

- The new elements provide clearer code (compared 
with using multiple <div> elements).
- Older browsers that do not understand HTML5 
elements need to be told which elements are 
block-level elements.
- To make HTML5 elements work in Internet Explorer 8 
(and older versions of IE), extra JavaScript is needed, 
which is available free from Google.


### Process & Design

> It's important to understand who your target audience 
> is, why they would come to your site, what information 
> hey want to find and when they are likely to return.
> Site maps allow you to plan the structure of a site.
> Wireframes allow you to organize the information that 
> will need to go on each page.
> Design is about communication. Visual hierarchy helps 
> visitors understand what you are trying to tell them.
> You can differentiate between pieces of information 
> using size, color, and style. 
> You can use grouping and similarity to help simplify 
> the information you present.

### JavaScript 

#### Introduction

```
Being able to change the content of an HTML page while it is loaded in the browser is very powerful.

Slideshows can display a number of different images within the same space on a given page. They can play automatically as a sequence, or users can click through the slides manually. They allow more content to be displayed within a limited amount of space.

Validating forms is important when information is supplied by users. JavaScript lets you alert the user if mistakes have been made. It can also perform sophisticated calculations based on any data entered and reveal the results to the user.

The examples on these two pages give you a taste of what JavaScript can do within a web page, and of the techniques you will be learning throughout this book.
You might not want to force visitors to reload the content of an entire web page, particularly if you only need to refresh a small portion of a page.
Just reloading a section of the page can make a site feel like it is faster to load and more like an application.

In the coming chapters, you will learn how and when to access or modify content, add programming rules, and react to events.
If you have a lot of information to display on a page, you can help users find information they need by providing filters. Here, buttons are generated using data in the attributes of the HTML elements.
When the user clicks on one of the buttons, they are only shown the images with that keyword

```



#### The ABC of Programming

```

It is best to keep JavaScript code in its own JavaScript 
file. JavaScript files are text files (like HTML pages and 
CSS style sheets), but they have the . j s extension. 
The HTML <script> element is used in HTML pages 
to tell the browser to load the JavaScript file (rather like 
the <link> element can be used to load a CSS file). 
If you view the source code of the page in the browser, 
the JavaScript will not have changed the HTML, 
because the script works with the model of the web 
page that the browser has created.

```