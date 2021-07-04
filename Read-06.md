
# Design web pages with CSS

* ## What is CSS
Presenting a document to a user means converting it into a form usable by your audience. Browsers, like Firefox, Chrome, or Edge , are designed to present documents visually, for example, on a computer screen, projector or printer. Browsers are the main type of user agent we think of when talking about CSS, however, it is not the only one.


#### CSS Modules

*As there are so many things that you could style using CSS, the language is broken down into modules. At this stage you don't need to worry too much about how CSS is structured, however it can make it easier to find information if, for example, you are aware that a certain property is likely to be found among other similar things and are therefore probably in the same specification*.

#### CSS Specifications

*This group is made of representatives of browser vendors and other companies who have an interest in CSS. New CSS features are developed, or specified, by the CSS Working Group. Sometimes because a particular browser is interested in having some capability, other times because web designers and developers are asking for a feature, and sometimes because the Working Group itself has identified a requirement. CSS is constantly developing, with new features coming available*.

* ## How to Add CSS

 **Three Ways to Insert CSS**

There are three ways of inserting a style sheet:
```
External CSS

Internal CSS

Inline CSS
```
- * **External CSS**

With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.
```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.

Here is how the "mystyle.css" file looks:
```
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```
* ## CSS Color
```
body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}
```
* ### [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)


* ### [Myers Web Reset Stylesheet](https://meyerweb.com/eric/tools/css/reset/)
