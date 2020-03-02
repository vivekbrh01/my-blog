---
title: "JavaScript Introduction | Part- I"
description: "What is JavaScript?"
date: "2020-03-02T07:35:06.305Z"
categories: []
published: false
---

  

### [What is JavaScript?](https://javascript.info/intro#what-is-javascript)

engines have different “codenames”. For example:

-   [V8](https://en.wikipedia.org/wiki/V8_%28JavaScript_engine%29) — in Chrome and Opera.
-   [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey) — in Firefox.

### [What can in-browser JavaScript do?](https://javascript.info/intro#what-can-in-browser-javascript-do)

Modern JavaScript is a “safe” programming language. It does not provide low-level access to memory or CPU, because it was initially created for browsers which do not require it.

JavaScript’s capabilities greatly depend on the environment it’s running in. For instance, [Node.js](https://wikipedia.org/wiki/Node.js) supports functions that allow JavaScript to read/write arbitrary files, perform network requests, etc.

In-browser JavaScript can do everything related to webpage manipulation, interaction with the user, and the webserver.

For instance, in-browser JavaScript is able to:

-   Add new HTML to the page, change the existing content, modify styles.
-   React to user actions, run on mouse clicks, pointer movements, key presses.
-   Send requests over the network to remote servers, download and upload files (so-called [AJAX](https://en.wikipedia.org/wiki/Ajax_%28programming%29) and [COMET](https://en.wikipedia.org/wiki/Comet_%28programming%29) technologies).
-   Get and set cookies, ask questions to the visitor, show messages.
-   Remember the data on the client-side (“local storage”).

### [What CAN’T in-browser JavaScript do?](https://javascript.info/intro#what-can-t-in-browser-javascript-do)

JavaScript’s abilities in the browser are limited for the sake of the user’s safety. The aim is to prevent an evil webpage from accessing private information or harming the user’s data.

Examples of such restrictions include:

-   JavaScript on a webpage may not read/write arbitrary files on the hard disk, copy them or execute programs. It has no direct access to OS functions.
-   Modern browsers allow it to work with files, but the access is limited and only provided if the user does certain actions, like “dropping” a file into a browser window or selecting it via an `<input>` tag.
-   There are ways to interact with camera/microphone and other devices, but they require a user’s explicit permission. So a JavaScript-enabled page may not sneakily enable a web-camera, observe the surroundings and send the information to the [NSA](https://en.wikipedia.org/wiki/National_Security_Agency).
-     
    
-   Different tabs/windows generally do not know about each other. Sometimes they do, for example when one window uses JavaScript to open the other one. But even in this case, JavaScript from one page may not access the other if they come from different sites (from a different domain, protocol or port).
-   This is called the “Same Origin Policy”. To work around that, _both pages_ must agree for data exchange and contain a special JavaScript code that handles it. We’ll cover that in the tutorial.
-   This limitation is, again, for the user’s safety. A page from `http://anysite.com` which a user has opened must not be able to access another browser tab with the URL `http://gmail.com` and steal information from there.
-     
    
-   JavaScript can easily communicate over the net to the server where the current page came from. But its ability to receive data from other sites/domains is crippled. Though possible, it requires explicit agreement (expressed in HTTP headers) from the remote side. Once again, that’s a safety limitation.

Such limits do not exist if JavaScript is used outside of the browser, for example on a server. Modern browsers also allow plugin/extensions which may ask for extended permissions.

What makes it unique?

-   Full integration with HTML/CSS.
-   Simple things are done simply.
-   Support by all major browsers and enabled by default.
-   JavaScript also allows to create servers, mobile applications, etc.
