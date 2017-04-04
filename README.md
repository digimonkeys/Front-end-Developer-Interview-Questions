#Front-end Job Interview Questions

This file contains a number of front-end interview questions that can be used when vetting potential candidates. It is by no means recommended to use every single question here on the same candidate (that would take hours). Choosing a few items from this list should help you vet the intended skills you require.

**Note:** Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would.

## Table of Contents

  1. [General Questions](#general-questions)
  1. [HTML Questions](#html-questions)
  1. [CSS Questions](#css-questions)
  1. [JS Questions](#js-questions)
  1. [Testing Questions](#testing-questions)
  1. [Performance Questions](#performance-questions)
  1. [Network Questions](#network-questions)
  1. [Coding Questions](#coding-questions)
  1. [Fun Questions](#fun-questions)

## Getting Involved

  1. [Contributors](#contributors)
  1. [How to Contribute](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/CONTRIBUTING.md)
  1. [License](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/LICENSE.md)

#### General Questions:

* What did you learn yesterday/this week?  
 React Higher Order Components  
 Sequelize ORM for NodeJS  
* What excites or interests you about coding?  

Creating stuff. Since childhood I loved processes of creation and also problem solving. I like constant development of my skills and knowledge, learning new things and facing new challenges every day.  

* What is a recent technical challenge you experienced and how did you solve it?  

Working on project based on boilerplate that used old version of webpack. When I tried to add some new indispensable features to it, everything occured to be incompatible and broke. I had to create whole webpack script from scratch.  

* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?  

UI - I usually start with drawing sketch, simply with pencil on paper - later I treat it as general guide to what I want to accomplish. I always put accent on readability and simplicity for users.  

Security - On frontend everything might happen, so I store fragile data on backend.  

Performance - I focus on writing clear, understandable code - when some functionality seems to be slow, then I try to boost its performance. Sometimes, when particular task seems to be heavy and I can solve it in different ways, I register and compare times of execution for different solutions in the first place.  

SEO - I usually dont take care of SEO in projects (it is not my task).  

Maintainability - I use general best practises, eg. take care of simple functions and variables names, split code into small, simple modules. I always put big stress on adapting to my hiring company practises.  

Technology - Lately I prefer to use React with Redux and webpack, but I'm also familiar with Angular and gulp etc (...)  

* Talk about your preferred development environment.
* Which version control systems are you familiar with?  
git, I worked on github and gitlab. I tried using git guis but I prefer to work in command line.  

* Can you describe your workflow when you create a web page?
* If you have 5 different stylesheets, how would you best integrate them into the site?
* Can you describe the difference between progressive enhancement and graceful degradation?  
* What is semantic html?  
Semantic HTML is the use of HTML markup to reinforce the semantics, or meaning, of the information in webpages and web applications rather than merely to define its presentation or look. Semantic HTML is processed by traditional web browsers as well as by many other user agents. CSS is used to suggest its presentation to human users.    

* How would you optimize a website's assets/resources?
* How many resources will a browser download from a given domain at a time?
  * What are the exceptions?
* Name 3 ways to decrease page load (perceived or actual load time).
* If you jumped on a project and they used tabs and you used spaces, what would you do?
I will adapt (just change settings in my editor).
* Describe how you would create a simple slideshow page. Bonus points if without JS.  
We can do it only with CSS3 using ul element and input type = radio. The most important parts of code:  

```
<li>
    <input type="radio" id="slide1" name="slide" checked>
    <label for="slide1"></label>
    <img>
</li>
.your-ul-class img {
    opacity: 0;
    visibility: hidden;
}
.ul-class li input:checked ~ img {
    opacity: 1;
    visibility: visible;
    z-index: 10;
}
```

Full tutorial: http://joshnh.com/weblog/making-a-pure-css-featured-image-slider/  

* If you could master one technology this year, what would it be?
* Explain the importance of standards and standards bodies.  
Standars are super important because apps being written in the same language are compiled by different browsers. Thanks to standards we avoid creating code that would work in half of browsers or only in one of them. Standard creators are: w3c, iso, ansi, unicode consortium, ietf and ecma  

* What is Flash of Unstyled Content? How do you avoid FOUC?  
Flash of unstyled content is displaying unstyled content for user for a while when loading page. Appears when CSS is slow to load or when JS causes multiple page rendering.
To avoid FOUC, you should provide the user with the most optimized CSS (minimized, in one file), and use as little rerendering browser javascript as possible. Use Critical CSS (ie throw the most important inline css rules in the head tag).
Use media queries and serve CSS optimized for lower resolution devices. One can also hide whole page until all styles are loaded.  
https://en.wikipedia.org/wiki/Flash_of_unstyled_content  
http://www.techrepublic.com/blog/web-designer/how-to-prevent-flash-of-unstyled-content-on-your-websites/  

* Explain what ARIA and screenreaders are, and how to make a website accessible.
* Explain some of the pros and cons for CSS animations versus JavaScript animations.
* What does CORS stand for and what issue does it address?

#### HTML Questions:

* What does a `doctype` do?
* What's the difference between full standards mode, almost standards mode and quirks mode?
* What's the difference between HTML and XHTML?
* Are there any problems with serving pages as `application/xhtml+xml`?
* How do you serve a page with content in multiple languages?
* What kind of things must you be wary of when design or developing for multilingual sites?
* What are `data-` attributes good for?
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
* What is progressive rendering?
* Have you used different HTML templating languages before?

#### CSS Questions:

* What is the difference between classes and IDs in CSS?
  IDs are unique, each element can have only one ID and ID's may be used by browser to scroll the page to show that element. Classes are not unique, each element can have multiple classes. Classes have not special meaning for browsers. Element can have both id and classes.
* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
  Resetting remove all CSS styles set by browsers. Normalizing set the same element's styles for every browser and fix some common bugs. I would use normalizing, because I'm sure that every element will look the same in every browser.

  http://stackoverflow.com/questions/6887336/what-is-the-difference-between-normalize-css-and-reset-css
* Describe Floats and how they work.
  Floats can be used to text wrapping around images/elements or to create entire web layouts. Floated elements remain a part of the flow of the web page, unlike elements with fixed position, which are removed from flow of the page and do not participate in adjusting content e.g. to the varying width of the window.

  https://css-tricks.com/all-about-floats/
* Describe z-index and how stacking context is formed.
  The z-index property controls the vertical stacking order of elements that overlap. Without any z-index value, elements stack in the order that they appear in the DOM (the lowest one down at the same hierarchy level appears on top). Nesting is important too, if an element B sits on top of element A, a child element of element A can never be higher than element B.

  https://css-tricks.com/almanac/properties/z/z-index/
* Describe BFC(Block Formatting Context) and how it works.
  A block formatting context is a part of a visual CSS rendering of a Web page. It is the region in which the layout of block boxes occurs and in which floats interact with each other. In a BFC, each box’s left outer edge touches the left edge of the containing block (for right-to-left formatting, right edges touch). The rules for positioning and clearing of floats in apply only to things within the same block formatting context. BFC is also causing margin collapsing.

  https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context
* What are the various clearing techniques and which is appropriate for what context?
  - Empty Div Method:
    <div style="clear:both;"></div>
    I do not use this method, because you have additional, unnecessary div with hardcored style. You can use this method when you create a layout (often in footer)
  - Overflow Method: setting auto or hidden overflow property on parent will expand it to contain the floats.
    If you add overflow: hidden to the containing element, it will automatically adjust its height and take the floated children into account.
  - The Easy Clearing Method: uses the parent's :after to add the clear: both property
    .clearfix:after {
      content: ".";
      visibility: hidden;
      display: block;
      height: 0;
      clear: both;
    }
    I often use this, but it generates content to the page that has nothing to do there in the first place.

  https://css-tricks.com/all-about-floats/
* Explain CSS sprites, and how you would implement them on a page or site.
* What are your favourite image replacement techniques and which do you use when?
* How would you approach fixing browser-specific styling issues?
  - use separate stylesheets that loads when that specific browser is being used.
  - use cross-browsers CSS prefixes (-moz-, -webkit-, etc)
  - resetting or normalizing CSS
* How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
* What are the different ways to visually hide content (and make it available only for screen readers)?
  - visibility: hidden
  - width: 0; height: 0;
  - text-indent: -1000px
  - absolute position off the screen
* Have you ever used a grid system, and if so, what do you prefer?
* Have you used or implemented media queries or mobile specific layouts/CSS?
* Are you familiar with styling SVG?
* How do you optimize your webpages for print?
* What are some of the "gotchas" for writing efficient CSS?
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* List as many values for the display property that you can remember.
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* How is responsive design different from adaptive design?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?

#### JS Questions:

* Explain event delegation
* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works
* What do you think of AMD vs CommonJS?
* Explain why the following doesn't work as an IIFE: `function foo(){ }();`.
  * What needs to be changed to properly make it an IIFE?
* What's the difference between a variable that is: `null`, `undefined` or undeclared?
  - Undeclared is a variable that was not created with var / let / const and was created on a global window / global object.
  - Undefined is a variable that has been declared but has no value assigned to it.
  - Null is a type that has only one null value assigned, the variable has been declared, and the Null object assigned to it.
  - Undefined is a type, null is an object
  * How would you go about checking for any of these states?
    - typeof undefined === 'undefined'
    - typeof null === 'object'
  https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof

* What is a closure, and how/why would you use one?
    Closure - allows you to access the internal scope of the function, even after it has been completed.
    This is achieved by returning the function after calling the master function.
    This allows you to simulate public and private variables.
    * Favorite pattern used to create them?
    - Module pattern
    http://blog.nebula.us/13-javascript-closures-czyli-zrozumiec-i-wykorzystac-domkniecia

* What's a typical use case for anonymous functions?
* How do you organize your code? (module pattern, classical inheritance?)
  Eg. Module pattern, IIFE, Atomic design.

* What's the difference between host objects and native objects?
    Host objects are objects provided by the host environment. They may be different between environments, examples:
    - window, document, location
    Native objects are the ones described and fully defined in the ECMAScript specification, examples:
    - Date, Math, parseInt.
    http://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects
    
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* When would you use `document.write()`?
  Document.write() is always available, it is a good choice for third party vendors to use it to add their scripts.
  Many generated ads use `document.write ()` although it is not welcome.

* What's the difference between feature detection, feature inference, and using the UA string?
* Explain Ajax in as much detail as possible.
  AJAX (Asynchronous JavaScript and XML).
  Web application development technology in which the user interacts with the server in two ways:
    Synchronous - pausing, the operation of the whole page.
    Asynchronous - requires callback function, without freezing the application state.
      There is no assurance that the response to the requests will return to us in the order in which requests are sent.
      It is possible to make asynchronous requests using 3 techniques:
      1. Using the XMLHttpRequest / ActiveObcjectX object (older versions of IE) - the most common way
      2. Floating frames
      3. Cookies

      AJAX is not limited to XML, It also support JSON or pure text.

* What are the advantages and disadvantages of using Ajax?
  Advantages:
    - Continuous and invisible for user updating of data
    - No need to refresh the entire page

  Disadvantages:
    - Does not work when JavaScript is disabled in browser
    - The page is not refreshed, so you can not undo or repeat steps with the browser buttons
    - Delays when the server is heavily loaded
    - Data is loaded dynamically and therefore is not part of the web page. Web search engines do not index dynamically loaded content.

* Explain how JSONP works (and how it's not really Ajax).
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* Difference between document load event and document DOMContentLoaded event?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
  ```javascript
  function duplicate(arr) {
    return arr.concat(arr);
  }
  ```
  * Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat
* Why is it called a Ternary expression, what does the word "Ternary" indicate?
* What is `"use strict";`? what are the advantages and disadvantages to using it?
* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`
* Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
* Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
* Explain what a single page app is and how to make one SEO-friendly.
* What is the extent of your experience with Promises and/or their polyfills?
* What are the pros and cons of using Promises instead of callbacks?
* Variables scope in JS?

In JavaScript, til version ES6, there were only two versions of variables scope - global scope, and local - function scope.
In ES6 there is one more - block scope for variables defined with let and const (scope in {}).

var![var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
let![let](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Statements/let)
const![const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
Other scopes![other scopes](http://stackoverflow.com/a/500459)

* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
* What tools and techniques do you use debugging JavaScript code?
* What language constructions do you use for iterating over object properties and array items?
* Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?
* Explain the difference between synchronous and asynchronous functions.
* Are functions hoisted in js?

There are two ways of declaring a function in JS: function definition and function expression.
Function definitions are hoisted, function expressions arent.

* What is event loop?
  * What is the difference between call stack and task queue?
* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`
* Whats the difference between function and an object?

Function is a specific type of object in JavaScript, that has all the properties of normal object. Only difference is that function can be called / invoked. It's possible, because functions has internal [[Call]] method.
Function prototype is Object, and it's prototype is Function();

* What is event life cycle (event flow) ?

Event life cycle (event flow) describes flow of an event through DOM tree. With every user interaction (or builtin event) browser creates event object and sends it (propagets it) through DOM tree. There are three phases of event life cycle:

 - capturing faze - in this faze event is sent from top of the DOM to the element, that action was taken on.
 - on the object faze - happens when event reach element which user made an action
 - bubbling faze - in this faze event is sent from the element that action was taken on, to the top element of the DOM tree.

Event flow![Event Life Cycle](http://www.quirksmode.org/js/events_order.html)

#### Testing Questions:

* What are some advantages/disadvantages to testing your code?

  Testing your code (unit testing) assures that the code is working as it should, allows you to refactor it and check whether nothing has been broken.

  Tests also require refactorization and need to be maintained, which may be considered as a disadvantage.

* What tools would you use to test your code's functionality?

  * Jasmine - TDD framework
  * Karma - tests runner
  * Selenium driver - End-to-End testing

* What is the difference between a unit test and a functional/integration test?

  Unit tests check whether the individual pieces of code (functions) work as expected on their own. Functional/integration tests check whether bigger parts of application, or even the application as a whole, work and interact with each other properly.

* What is the purpose of a code style linting tool?

  Avoids introducing simple bugs at the stage of writing the code. It assures that code formatting is more consistent between members of the team.

#### Performance Questions:

* What tools would you use to find a performance bug in your code?

  Chrome Dev-Tools Profiler - it allows to check function execution time and pin-point the ones that use the most CPU.

  [more info](https://developers.google.com/web/tools/chrome-devtools/rendering-tools/js-execution)

* What are some ways you may improve your website's scrolling performance?
* Explain the difference between layout, painting and compositing.

#### Network Questions:

* Traditionally, why has it been better to serve site assets from multiple domains?
* Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.
* What are the differences between Long-Polling, Websockets and Server-Sent Events?
* Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
* What are HTTP methods? List all HTTP methods that you know, and explain them.

#### Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

*Question: What is the value of `window.foo`?*
```javascript
( window.foo || ( window.foo = "bar" ) );
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

#### Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Who inspires you in the front-end community?
* Do you have any pet projects? What kind?
* What's your favorite feature of Internet Explorer?
* How do you like your coffee?


#### Contributors:

This document started in 2009 as a collaboration of [@paul_irish](https://twitter.com/paul_irish) [@bentruyman](https://twitter.com/bentruyman) [@cowboy](https://twitter.com/cowboy) [@ajpiano](https://twitter.com/ajpiano)  [@SlexAxton](https://twitter.com/slexaxton) [@boazsender](https://twitter.com/boazsender) [@miketaylr](https://twitter.com/miketaylr) [@vladikoff](https://twitter.com/vladikoff) [@gf3](https://twitter.com/gf3) [@jon_neal](https://twitter.com/jon_neal) [@sambreed](https://twitter.com/sambreed) and [@iansym](https://twitter.com/iansym).

It has since received contributions from over [100 developers](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors).
