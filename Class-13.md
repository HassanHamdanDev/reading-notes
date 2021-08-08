# Local Storage



## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

```

To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. UserData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available. Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS , but it was limited by some of Flash’s design quirks.

By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Flash gives each domain 100 KB of storage «for free.» Beyond that, it prompts the user for each order of magnitude increase in data storage . In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. Gears provides an API to an embedded SQL database based on SQLite.

After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.

```

- HTML5 STORAGE SUPPORT

```

From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage. If { // window.

Like other JavaScript objects, you can treat the localStorage object as an associative array.

Event. If { e = window.

```

- STORAGEEVENT OBJECT

Some browsers shipped with that property before the specification changed. It’s simply a way for the browser to tell you, «hey, this just happened. » .

## HTML5 STORAGE IN ACTION

```

Make a few moves, then close the browser tab, then re-open it. If your browser supports HTML5 Storage, the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected. LocalStorage = gPieces . BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS

While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification.

The Web SQL Database specification has been implemented by four browsers and platforms.

```

## WEB SQL DATABASE SUPPORT

```

Of course, if you’ve used more than one database product in your life, you are aware that «SQL» is more of a marketing term than a hard-and-fast standard. Sure, there is an actual SQL specification , but there is no database server in the world that conforms to that and only that specification.

The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. There are «databases» with «records,» and each record has a set number of «fields.» Each field has a specific datatype, which is defined when the database is created. If you’ve done any SQL database programming, these terms probably sound familiar.

Instead, you use methods provided by the object store to open a cursor on the database named «USERS,» enumerate through the records, filter out records for inactive users, and use accessor methods to get the values of each field in the remaining records. An early walk-through of IndexedDB is a good tutorial of how IndexedDB works, giving side-by-side comparisons of IndexedDB and Web SQL Database. At time of writing, IndexedDB has only been implemented in a beta version of Firefox 4. Google has stated that they are considering IndexedDB support for Chromium and Google Chrome.

And even Microsoft has said that IndexedDB «is a great solution for the web».

```

