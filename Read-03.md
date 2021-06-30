

# Structure web pages with HTML

- ## Wireframe and Design

1. Prepare your research for quick reference

Lift your wireframes off the paper and onto a whiteboard, and play around with them.

2. Add some detail and get testing

So you have a flow and you have your screens, and you’ve corroborated your ideas with some clued-up colleagues.

3. Tooltips to indicate any functionality that could be included in a prototype transition

With this tool, you can simply photograph and upload your hand-sketched wireframes, and then connect them to user button overlays.

- ## Mozilla HTML Basics

### My test page

In the mists of time, when HTML was young , doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML, which could mean automatic error checking and other useful things. This element wraps all the content on the entire page and is sometimes known as the root element. This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers.

### Headings

In the same way that a book has the main title, chapter titles, and subtitles, an HTML document can too. Now try adding a suitable title to your HTML page just above your element.

### Lists

A lot of the web's content is lists and HTML has special elements for these.

### Examples

>  * <h1>My main title</h1>

>   * <img src="images/firefox-icon.png" alt="My test image">

>  * <p>This is a single paragraph</p>


- ## Semantics

In HTML, for example, the <h1> element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page."

* <h1>This is a top level heading</h1>

By default, most browser's user agent stylesheet will style an <h1> with a large font size to make it look like a heading (although you could style it to look like anything you wanted).

On the other hand, you could make any element look like a top level heading. Consider the following:

* <span style="font-size: 32px; margin: 21px 0;">Is this a top level heading?</span>

This will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits as described above. It is therefore a good idea to use the right HTML element for the right job.

- ### These are some of the roughly 100 semantic elements available:

* <article>
* <aside>
* <details>
* <figcaption>
* <figure>
* <footer>
* <header>
* <main>
* <mark>
* <nav>
* <section>
* <summary>
* <time>

### Useful Links :
+ [wireframes](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)
+ [HTML Basics](https://developer.mozilla.org/en-US/docs/Web/HTML)
+ [Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)