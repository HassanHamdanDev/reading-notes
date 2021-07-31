# JS Object Literals; The DOM


## Understanding The Problem Domain Is The Hardest Part Of Programming

```

- A familiar problem

In a good portion of my Pluralsight courses I show the viewer how to build the «Protein Tracker» application.
I am often asked why I keep demonstrating how to build the same simple application over and over again in each of my courses.
The answer is «familiarity».


Very simple functionality, easily explainable, but most importantly, easily understood.
What I found with this simple application was that because it was so easy to understand, the focus was taken off of the problem domain and put instead on the technology.


- So what am I trying to say here?

Simply that by taking away the problem domain, or making it so trivial that it is easily understood, I am able to make both teaching and learning easier.


This all breaks down when you don’t have a picture with clear components that you can identify.
The same thing happens when writing code. Writing code is a lot like putting together a jigsaw puzzle. We put together code with the purpose of building components that we have taken out of the «bigger picture» of the problem domain.


- Programming is easy if you understand the problem domain

A long time ago, I worked for Hewlett Packard writing software for multi-function printers.
Most of the work at the time was basic waterfall development. There wasn’t much Agile happening there—at least at the time I was there.waterfall can define problem domains
There was however something really interesting about the waterfall approach and the extreme amount of specification that was done before anything was built—it was very easy to write the code for a feature.
I remember writing a tab control for the user interface of a printer and having the complete pixel perfect specs handed to me before I began to write any code. I was also given all the possible use cases and told exactly how it should function and what it should do under just about every circumstance.
Guess how easy it was to write the code to produce this tab control? Super easy.


You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.
Games are really good at this. Look at most games today and you’ll find that you start with a very small problem domain. The first level is usually a tutorial that has a basic set of things you can do so that you don’t get overwhelmed. But, as you advance through the levels, you usually find they get harder and introduce new concepts that build gradually on what you know, until you understand a pretty large problem domain.


- Quick update on my new product

I’m still not ready to unveil exactly what I am building, but I do have an active mailing list where you can sign up to find out when I release the product I’m working on to help developers get better career opportunities and market themselves.

```


## Object Literals

```

- Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, 
variables and functions take on new names.

Programmers use a lot of name/value pairs: 
• HTML uses attribute names and values. 
• CSS uses property names and values. 
In JavaScript: 
• Variables have a name and you can assign them a 
value of a string, number, or Boolean. 
• Arrays have a name and a group of values. (Each 
item in an array is a name/value pair because it 
has an index number and a value.) 
• Named functions have a name and value that is a 
set of statements to run if the function is called. 
• Objects consist of a set of name/value pairs 
(but the names are referred to as keys). 

```

## Document Object Model

```

The browser represents the page using a DOM tree. 
DOM trees have four types of nodes: document nodes, 
element nodes, attribute nodes, and text nodes. 
You can select element nodes by their id or cl ass 
attributes, by tag name, or using CSS selector syntax. 
Whenever a DOM query can return more than one 
node, it will always return a Nadel i st. 
From an element node, you can access and update its 
content using properties such as textContent and 
i nnerHTML or using DOM manipulation techniques. 
An element node can contain multiple text nodes and 
child elements that are siblings of each other. 
In older browsers, implementation of the DOM is 
inconsistent (and is a popular reason for using jQuery). 
Browsers offer tools for viewing the DOM tree .

```