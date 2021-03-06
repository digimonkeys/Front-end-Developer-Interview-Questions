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
I prefer easily configurable Sublime 3 with its additional packages and briliant editorial functions. My browser of choice is chrome with its dev tools, but I also use firebug. I have some knowledge about linux, but currently I use windows 10. I also use tools like gulp, webpack, window managers, linters etc.  

* Which version control systems are you familiar with?  
git, I worked on github and gitlab. I tried using git guis but I prefer to work in command line.  

* Can you describe your workflow when you create a web page?  
I start with gathering client requirements. Ten I create environment - bundling scripts from webpack, gulp etc. Next comes site skeleton, semantics, filling with content and fixes, styling, animations and adding interactivity.  


* If you have 5 different stylesheets, how would you best integrate them into the site?

* Can you describe the difference between progressive enhancement and graceful degradation? Bonus points for describing feature detection.  
progressive enhancement considers creating site for old browsers and then enhancing application with fetures for newer browsers  

graceful degradation is creating app for new versions of eg. browsers, but in a way that lets the app maintain some basic functionalities if some of environment features happen to be unavalaible  

Feature detection (also feature testing) is a technique used in web development for handling differences between runtime environments (typically web browsers or user agents), by programmatically testing for clues that the environment may or may not offer certain functionality. This information is then used to make the application adapt in some way to suit the environment: to make use of certain APIs, or tailor for a better user experience  

* What is semantic html?  
Semantic HTML is the use of HTML markup to reinforce the semantics, or meaning, of the information in webpages and web applications rather than merely to define its presentation or look. Semantic HTML is processed by traditional web browsers as well as by many other user agents. CSS is used to suggest its presentation to human users.  

* How would you optimize a website's assets/resources?  
Optimalize images, bundle files, use uglifyjs and minification, use svg, css sprites, serve cdn resources depending on distance and response time from user, cache some files, dont load whole huge libraries if you only use one function from them  

* Why serving resources from many domains is better?  
You can use a lightweight web server that doesn't have to load all the modules/extensions that your dynamic content web server has to load on every single request.
Adding an extra subdomain means you increase the number of parallel downloads that the browser can perform.
If set up properly (e.g. your site is hosted on www.example.com instead of example.com), you can also take advantage of a cookieless subdomain, reducing traffic and roundtrip times. 
http://webmasters.stackexchange.com/a/26757
http://webmasters.stackexchange.com/a/25091  

* How many resources will a browser download from a given domain at a time? 
It depends on a browser, older ones like IE6 - 2, newer ones 6-8.  

* How would you optimize a website's assets/resources?
* How many resources will a browser download from a given domain at a time?
  * What are the exceptions?
* Name 3 ways to decrease page load (perceived or actual load time).  
1. Optimalize images - decrease their amount, use miniatures, svg, css-sprites, preloaders 2.Cache content 3. Reduce amount of http requests  

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

* What tools do you use to check your code performance?  
Chrome Timeline - record and analyze all the activity in your application as it runs, accessible in devTools  
JSPerf - jsPerf aims to provide an easy way to create and share test cases, comparing the performance of different JavaScript snippets by running benchmarks.  
 Dromaeo - Mozilla JavaScript performance test suite currently considered to be a "work in progress."  
https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/timeline-tool  
https://jsperf.com/  
https://wiki.mozilla.org/Dromaeo   

* If you could master one technology this year, what would it be?
I'd love to learn how to create fusion bomb. ...or just pick something trendy, React Native, React Redux, ES7.  

* Explain the importance of standards and standards bodies.  
Standars are super important because apps being written in the same language are compiled by different browsers. Thanks to standards we avoid creating code that would work in half of browsers or only in one of them. Standard creators are: w3c, iso, ansi, unicode consortium, ietf and ecma  

* What is Flash of Unstyled Content? How do you avoid FOUC?  
Flash of unstyled content is displaying unstyled content for user for a while when loading page. Appears when CSS is slow to load or when JS causes multiple page rendering.
To avoid FOUC, you should provide the user with the most optimized CSS (minimized, in one file), and use as little rerendering browser javascript as possible. Use Critical CSS (ie throw the most important inline css rules in the head tag).
Use media queries and serve CSS optimized for lower resolution devices. One can also hide whole page until all styles are loaded.  
https://en.wikipedia.org/wiki/Flash_of_unstyled_content  
http://www.techrepublic.com/blog/web-designer/how-to-prevent-flash-of-unstyled-content-on-your-websites/  

* Explain what ARIA and screenreaders are, and how to make a website accessible.  
ARIA defines ways to make Web content and Web applications (especially those developed with Ajax and JavaScript) more accessible to people with disabilities.
A screen reader is a software application which, rather than presenting web content visually, converts text into 'synthesised speech' allowing user to alternatively listen to content.
The steps to follow to make your Web apps accessible are as follows:

Use native HTML tags wherever possible
Make interactive elements keyboard accessible
Provide extra markup for AT (accessibility technology)
https://www.w3.org/WAI/intro/aria
http://gingertech.net/2012/02/14/a-systematic-approach-to-making-web-applications-accessible/

* Explain some of the pros and cons for CSS animations versus JavaScript animations.  
Cons of CSS animations vs JS:  
- scale/rotation/position control are all crammed into one "transform" property, making them impossible to animate in a truly distinct way on a single element  
- CSS is praised for using GPU instead of CPU for animations, but only transforms and opacity are the primary beneficiaries of this feature, plus in JS we can do that too by setting a transform with a 3D characteristic  
- CSS in theory is able to use a different CPU thread for animation-related calculations, but only properties that don't affect document flow can truly be relegated to a different thread. So again, transforms and opacity are the primary beneficiaries - it's a very little boost on performance  
- on almost every platform animations created with JS GASP are performing better than created with CSS  
- no control over animation flow (you cannot seek to a particular spot in the animation, nor can you smoothly reverse part-way through or alter the time scale or add callbacks at certain spots or bind them to a rich set of playback events)  
- some really old browsers cannot perform css animations (older than IE9)  

Pros of CSS animations vs JS:  
- they perform much better than JQuery animations  
- great for simple sliders and hover effects  

https://developers.google.com/web/fundamentals/design-and-ui/animations/css-vs-javascript  
https://css-tricks.com/myth-busting-css-animations-vs-javascript/  

* What does CORS stand for and what issue does it address?

* What HTTP methods do you know?
* How many requests are there on GET and how many on PUT, and where does the difference come from?
* What's REST? What alternatives do you know?
* What is the difference in logging into SPA app and normal app?
* What threats and attacks are related to SPA apps?


[9:34]  
. co sie dzieje gdy uzywamy new?

#### HTML Questions:

* What does a `doctype` do?  
DOCTYPEs are required for legacy reasons. When omitted, browsers tend to use a different rendering mode that is incompatible with some specifications. Including the DOCTYPE in a document ensures that the browser makes a best-effort attempt at following the relevant specifications. Examples:  

```
html 5: <!DOCTYPE html>
HTML 4.01 Strict <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
XHTML 1.0 Strict <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

* What's the difference between full standards mode, almost standards mode and quirks mode?  
Full standards mode renders page according to modern web standards of html and css. Quirks mode is rendering mode for very old browsers - IE 5 and Navigator 4. Almost standards mode renders page with a small amount of quirks.    
https://developer.mozilla.org/pl/docs/Quirks_Mode_and_Standards_Mode  

* What's the difference between HTML and XHTML?  
XHTML is HTML written as XML. They are almost identical. Most important differences are: XHTML is stricter and is supported by all major browsers. Doctype is mandatory, also xmlns attribute in <html> and <html>, <head>, <title>, and <body> are mandatory. XHTML elements must be properly nested, always be closed, always in lowercase, always have one root element.  
https://www.w3schools.com/html/html_xhtml.asp  

* What are the limitations when serving xhtml page?  
Perhaps the biggest issue is the poor browser support XHTML currently enjoys. In typical setups, most browsers simply pretend that your XHTML pages are regular HTML. XHTML source is not necessarily any “cleaner” than HTML source. Plus we have to take care of restrictions like this:  
- all elements must have a start tag.  
- non-void elements with a start tag must have an end tag (p and li, for example).  
- any element may be “self-closed” using />.  
- tags and attributes are case sensitive, typically lowercase.
- attribute values must be enclosed in quotes.  
- empty attributes are forbidden (checked must instead be checked="checked" or checked="true").  
- special characters must be escaped using character entities.  

http://www.webdevout.net/articles/beware-of-xhtml#myths  

* Are there any problems with serving pages as `application/xhtml+xml`?  
When a browser reads XML it uses an XML parser, not an HTML parser. Unfortunately, up to and including version 8, Internet Explorer doesn't support files served as XML, although a number of other browsers do. To get around the fact that not all browsers support content served as XML, many XHTML files are actually served using the text/html MIME type. In this case, the user agent will read the file as if it were HTML, and use the HTML parser. Since the browser considers the XML to actually be HTML, you need to take into account some of the differences between the two formats when writing your XHTML code, to ensure that the differences between XML and HTML syntax do not trip up the browser. This includes different ways of declaring the character encoding or language declarations inside the document.  
In IE8 there would be opened downloading dialogue for such served site. Proxy servers might already have cached xml version of site and they later will send it to browsers that dont support xml. Xml errors will be shown by browser when they occure. 

http://stackoverflow.com/a/351908  
https://www.w3.org/International/articles/serving-xhtml/  

* How do you serve a page with content in multiple languages?  
Always use a language attribute on the html tag to declare the default language of the text in the page. When the page contains content in another language, add a language attribute to an element surrounding that content. Use the lang attribute for pages served as HTML, and the xml:lang attribute for pages served as XML. For XHTML 1.x and HTML5 polyglot documents, use both together.  
https://www.w3.org/International/questions/qa-html-language-declarations  

* What kind of things must you be wary of when design or developing for multilingual sites?  
I have to consider how will users to be directed to their native language? Also I need to remeber about things like: text in images wont translate or scale, colors might be perceived different in different culture, no text should be hardcoded in templates, dates formatting might differ, styling font-size for :lang({language_code}) selectors in CSS, difference in word length for each language.  
https://www.quora.com/What-kind-of-things-one-should-be-wary-of-when-designing-or-developing-for-multilingual-sites  

* What are `data-` attributes good for?
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?  
The main building blocks are centred on HTML 5, CSS3, Javascript and SVG. Where HTML is a language to define the mark-up of a document (titles, headers, body, footer, tables, input forms etc.), CSS is a language to define style (formatting, colours, shades and the like). Javascript is a programming/scripting language and SVG is a language for creating 2D scalable vector graphics and images.  
http://yucianga.info/?p=655  

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.  
Cookie:
Max size of 4093 bytes, can set expiration date, sent on every request  
sessionStorage:
Max size of 2.5MBs+ depending on browser, stored in browser and not sent with every request, if you close a tab using sessionStorage, open a new tab, or exit the browser - you'll lose that specific sessionStorage data. 
localStorage:
Max size of 2.5MBs+ depending on browser, stored in browser and not sent with every request, will persist if browser/tabs are closed.  
http://stackoverflow.com/a/19869560  

* Describe the difference between `<script>`, `<script async>` and `<script defer>`.  
Browser behaviour encountering:  
- script tag: Pause parsing the document. Make a request to fetch the file. Execute the script after it has been downloaded. Resume parsing the document.  
- script tag with async: Make parallel requests to fetch the files. Continue parsing the document as if it was never interrupted. Execute the individual scripts the moment the files are downloaded.  
- script tag with defer: Make parallel requests to fetch the files. Continue parsing the document as if it was never interrupted. Finish parsing the document even if the script files have downloaded. Execute each script in the order they were encountered in the document.  
http://javascript.tutorialhorizon.com/2015/08/11/script-async-defer-attribute/  

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?  
Placing css in header lets us avoid FOUC. Placing script before body tag makes sense for old browsers that stops rendering page when encountered script tag. The browser cannot start downloading the scripts until the entire document is parsed. For larger websites with large scripts & stylesheets, being able to download the script as soon as possible is very important for performance.  
Nowadays browsers have defer and async scripts, also speculative parsing, so modern approach is to just use defer script tags.  
http://stackoverflow.com/a/24070373  

* What is progressive rendering?  
Progressive rendering is the name given to techniques used to render content for display as quickly as possible. Example: lazy loading of images where (typically) some javascript will load an image when it comes into the browsers viewport instead of loading all images at page load.  
http://stackoverflow.com/a/33651444  

* Have you used different HTML templating languages before?  
No, but I'm familiar with Jade, EJS, HandlebarsJs, Underscore Templates, Mustache  

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
  It is the way to reduce HTTP requests by combining images together into one big image. I would use sprite generator, combining all images into one big, usually separated by a pixel. In the css, put the background image on a sprite class that I use for all my image elements. To specify a specific image or icon, I'll set another class with the background positions and sizes of the image.

  https://css-tricks.com/css-sprites/
* What are your favourite image replacement techniques and which do you use when?
  CSS image replacement is a technique of replacing a text element (usually a header tag) with an image. You may want to use a `<h1>` tag and text for this for the accessibility and SEO benefits.
  I use image replacements (depending on the needs), when I want to make my page more accessible for devices like readers etc. Usually I use display none span in header.

  #1: Display none span in header
  ```html
  <h1 id="logo">
    <span>CSS-Tricks</span>
  </h1>
  ```
  ```css
  h1#logo {
    width: 250px;
    height: 25px;
    background-image: url(logo.gif);
  }
  h1#logo span {
    display: none;
  }
  ```
  #2: Text-indent out of sight
  ```html
  <h1 id="logo">
    CSS-Tricks
  </h1>
  ```
  ```css
  h1#logo {
    width: 300px;
    height: 75px;
    background: url(test.png);
    text-indent: -9999px;
  }
  ```
  #3: Invisible Text
  ```html
  <h3 class="leon">
    <span>CSS-Tricks</span>
  </h3>
  ```
  ```css
  h3.leon {
    width: 300px;
    height: 75px;
    background: url(test.png);
  }
  h3.leon span {
    display: block;
    width: 0;
    height: 0;
    overflow: hidden;
  }
  ```
  https://css-tricks.com/css-image-replacement/
* How would you approach fixing browser-specific styling issues?
  - use separate stylesheets that loads when that specific browser is being used.
  - use cross-browsers CSS prefixes (-moz-, -webkit-, etc)
  - resetting or normalizing CSS
* How do you serve your pages for feature-constrained browsers?
  - separate stylesheets that loads when that specific browser is being used
  - create a completely separate layout
  - polyfills (A polyfill is code that detects if a certain "expected" API is missing and manually implements it.)

  * What techniques/processes do you use?
      Graceful Degradation

  https://www.sitepoint.com/progressive-enhancement-graceful-degradation-basics/
* What are the different ways to visually hide content (and make it available only for screen readers)?
  - visibility: hidden
  - width: 0; height: 0;
  - text-indent: -1000px
  - absolute position off the screen
* Have you ever used a grid system, and if so, what do you prefer?
  I used Bootstrap and Angular Material. Additionally I heard about Skeleton and Foundation. I prefer Bootstrap, because creating pages with this grid is very easy. Whether you need a fixed grid or a responsive, its only matter of a few changes. Offsetting and nesting of columns is also possible in both fixed and fluid width layouts.
* Have you used or implemented media queries or mobile specific layouts/CSS?
  Yes, I used media queries after I created a project using Bootstrap grid to learn how Bootstrap and responsive pages works. I used mobile-first method to have a fully-responsive, readable page on any device without unnecessary content.
  Media queries allow you to target CSS rules based on - for instance - screen size, device-orientation or display-density. It allows you to display your page in different way on different devices.

  http://cssmediaqueries.com/
* Are you familiar with styling SVG?
  A bit. I colored some SVG's.
  Generally SVG is resolution independent (scalable, without losing quality), does not add any additional, unneccesary HTTP requests and is very easy to script. You can use SVG to make road maps, graphs, complex UI elements, logos and simple games. You are able to use CSS and style SVG what you like. Also you can use animations which will move your whole SVG or just paths (parts of SVG).

  https://www.smashingmagazine.com/2014/11/styling-and-animating-svgs-with-css/
  https://code.tutsplus.com/articles/why-arent-you-using-svg--net-25414
* How do you optimize your webpages for print?
  - create a stylesheet for print
  - avoid unnecessary HTML tables
  - know which portions of the page do not have any print value (give him class .no-print with display:none)
  - use page breaks in places where page should break (.page-break { page-break-before: always; display: none; })
  - size page for print (width in inches or centimeters(both recommended))

  https://davidwalsh.name/optimizing-structure-print-css
* What are some of the "gotchas" for writing efficient CSS?
  - avoid key selectors that match large numbers of elements (tag and universal selectors)
  - prefer class and ID selectors over tag selectors
  - avoid redundant selectors
  - try group and reuse common properties

  https://css-tricks.com/efficiently-rendering-css/
* What are the advantages/disadvantages of using CSS preprocessors?
  Advantages
    - better organization from nesting selectors
    - ability to define variables and mixins
    - have mathematical functions
    - joining multiple files
    - in some cases, cleaner syntaxes
  Disadvantages
    - mainly for designers - not comfortable on the command line or programming concepts
  * Describe what you like and dislike about the CSS preprocessors you have used.
    I used SASS and I really like nesting, variables and mathematical functions which help a lot in styling. There were no things I did not like, maybe my knowledge about SASS is not enough deep.

  http://nosleepforsheep.com/using-a-css-preprocessor/
* How would you implement a web design comp that uses non-standard fonts?
  - use '@font-face' to render a font (uses 'src' for hard resources)
  - link to a webfont as a stylesheet, use @import or javascript (link from e.g. google fonts)
* Explain how a browser determines what elements match a CSS selector.
  Browsers read selectors from right-to-left. First looks for all elements matching the key selector (the right-most). Then checks if it matches or is under the next (left-most) element.
* Describe pseudo-elements and discuss what they are used for.
  Pseudo-elements starts with '::' and are used to style specified parts of and element.
    Syntax: 'selector::pseudo-element {}'
    We distinguish the following pseudo-elements:
     - ::after - add additional layer/content after the element
     - ::before - add additional layer/content before element
     - ::first-letter - selects the first letter
     - ::first-line - selects the first line
     - ::selection - selects the portion of and element that is selected by user
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
  For display purpose, every element in the page is considered a box. The box model refers to the specification of the box attributes such as the width, padding, border and margin.
  You can change the box model by setting the box-sizing property. Some values are: content-box (default), padding-box, and border-box)
  Content-box: width & height includes content but not padding/border/margin
  Padding-box: include up to padding
  Border-box: include up to border, but not margin
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
  It’s the IE6 Quirks mode: if you set a width, and add paddings and borders, the total width won’t change. It’s the inner width that will adapt.

  Advantage: You can play with the paddings and border values without worrying about expanding your box. Very convenient for column layouts. And you can mix percentage and pixel values, so you do not have to rely on a child element for the padding.
* List as many values for the display property that you can remember.
  display: value; - displays an element as...
  - inline - an inline element, default value
  - block -  a block element
  - inline-block - an inline-level block container
  - flex - an block-level flex container
  - inline-flex - an inline-level flex container
  - inline-table - an inline-level table
  - run-in - either block or inline, depending on context
  Let the element behave like...
  - list-item - ``<li>``
  - table - ``<table>``
  - table-caption - ``<caption>``
  - table-column-group - ``<colgroup>``
  - table-header-group - ``<thead>``
  - table-footer-group - ``<tfoot>``
  - table-row-group - ``<tbody>``
  - table-cell - ``<td>``
  - table-column - ``<col>``
  - table-row - ``<tr>``
  - none - the element will not be displayed
  - initial - sets this property to its default value
  - inherit - inherits this property from its parent

  https://www.w3schools.com/cssref/pr_class_display.asp
* What's the difference between inline and inline-block?
  Elements with display:inline-block are like display:inline elements, but they can have a width and a height. That means that you can use an inline-block element as a block while flowing it within text or other elements.

  Difference of supported styles:
    inline: only margin-left, margin-right, padding-left, padding-right
    inline-block: margin, padding, height, width
* The 'C' in CSS stands for Cascading. How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
  CSS priority is determined by specificity and inheritance.
  Ascending order of importance:
    1. User agent declarations,
    2. User declarations,
    3. Author declarations,
    4. Author !important declarations,
    5. User !important declarations.

  Specificity: ID > class, pseudo-class > element, pseudo-element
  Inheritence: specified value → computed value → used value → actual value

  Knowing that I can define how to plan my code using specificity and inheritance, so they cause only minimal (or no) problems.

  https://www.smashingmagazine.com/2010/04/css-specificity-and-inheritance/
* What's the difference between a relative, fixed, absolute and statically positioned element?
  Static is the default type of positioning. When elements don’t have a position specifically set, they default to static. These elements will stack in a standard one-after-another order.

  Relative Position
  You can set its position using one of the following top: XXX ; bottom: XXX; left: XXX; right: XXX;. Element will move off from the side specified, so if you wrote top:50px; the element will move 50px off from the top, or basically down. When you do this though, it doesn’t effect any other static elements around it, so they can overlap.

  An absolutely positioned element is actually removed from the DOM and positioned based on its nearest relatively positioned parent element. Unlike a relatively positioned element which doesn’t effect other static elements, when you give an element position:absolute its like it no longer exists. This means that other static elements will move up to fill in the space where the absolute element would have been. The position of the absolute element is determined by its parent elements. If all of the parent elements are either static, or there are none, then the element is positioned based on the <body>. 

  Fixed elements are completely independent of everything else on the web page. Regardless of any parents, a fixed position element will always be positioned based on the browser window. The interesting thing about fixed position elements is that when the page is scrolled, the element stays “fixed” and is always visible.
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
  Bootstrap and Angular Material. Bootstrap is great for small pages, but for bigger projects there is too much to change. Every framework impose its own style of page, so a lot of pages looks the same, just with different colors. It is what I would change in CSS frameworks - more freedom and adjusting to create pages which don't look like a milion others.
* Have you played around with the new CSS Flexbox or Grid specs?
  Yes, I use flexbox in my projects. It is very simple and comfortable in use and giving great effects. Grid seems to be supported by all major browsers (except Edge, which has old syntax), so it is worthy to learn it.

  http://caniuse.com/#feat=css-grid
  https://css-tricks.com/snippets/css/a-guide-to-flexbox/
  https://css-tricks.com/snippets/css/complete-guide-grid/
* How is responsive design different from adaptive design?
  Responsive: There is one basic layout, and it changes responsively to screen changes
  Adaptive: For each possible screen size, there is a distinct layout
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
  Retina has double density pixel screen, it allows to create sharper images on smaller screens. You need to provide suitable images for these screens.

  Resizing Images
    - Using alternate high resolution pixels
    - Using @face-fonts instead of images icon
    - Using SVG images instead of Bitmap images
    - Using JavaScript to replace all the images with double sized image
  Working with high resolution favicons

  https://www.sitepoint.com/css-techniques-for-retina-displays/
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?
  Yes, translate do not cause the browser to repaint when it is used, which if you're looking for the best performance is undoubtly better.

  https://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/

#### REACT Questions:

* What is React? How is it different from other JS frameworks?
    React is a library that allows you to create composite user interfaces.
    It has a virtual DOM tree, and when you change some data, only those elements are rendered,
    those that have changed. Compared by layer V (View) in MVC. The main assumption is
    creating reusable components.

    Difference:
      - Virtual DOM tree
      - Re-render only those elements that have changed
      - Uses JSX - javascript and html combination
      - It needs libraries like Flux or Redux to implement full architectures

* What happens during the lifecycle of a React component?
    React.Component has three main life cycles, allowing them to manage
    Component before adding it to the DOM tree, during its life
    and when it was removed. These are:
    1. mount - Methods created when adding to a DOM tree:
      - constructor()
      - componentWillMount()
      - render()
      - componentDidMount()
    2. update - Methods invoked when changing the state of a component or variable in this.props object:
      - componentWillReceiveProps()
      - shouldComponentUpdate()
      - componentWillUpdate()
      - render()
      - componentDidUpdate()
    3. unmount - Method invoked when a component is removed from a DOM tree:
      - componentWillUnmount()

* What can you tell me about JSX?
    This is the so-called. Syntax sugar for function
    React.createElement (component, props, ... children).
    It allows you to write code that is a combination of javascript and html
    within the render function of the component. JSX syntax can be used to
    render both regular HTML elements as well as other React components,
    these must start with a capital letter.

* Are you familiar with Flux?
    With Flux no. On the other hand, I have experience with Redux, which comes from Flux.
    The simplest saying Redux middleware provides a third-party extension point
    between dispatching an action, and the moment it reaches the reducer.
    Redux can be described in three fundamental principles:
    - Single source of truth - The state of your whole application is stored
      in an object tree within a single store.
    - State is read-only - The only way to change the state is to emit an action,
      an object describing what happened.
    - Changes are made with pure functions - To specify how the state tree
      is transformed by actions, you write pure reducers.
      
* What are stateless components?
  Stateless components are components that do not have `this.state` inside them.
  Other names are pure or dumb. You can declare them using the const and
  arrow functions as well as all its internal functions. So we do not have to worry
  about `this` inside the component.
  
* Explain this Code:

  ```

  class MyComponent extends React.Component {
      constructor(props) {
          // set the default internal state
          this.state = {
              clicks: 0
          };
      }

      componentDidMount() {
          this.refs.myComponentDiv.addEventListener(
              ‘click’,
              this.clickHandler
          );
      }

      componentWillUnmount() {
          this.refs.myComponentDiv.removeEventListener(
              ‘click’,
              this.clickHandler
          );
      }

      clickHandler() {
          this.setState({
              clicks: this.clicks + 1
          });
      }

      render() {
          let children = this.props.children;

          return (
              <div className=”my-component” ref=”myComponentDiv”>
                  <h2>My Component ({this.state.clicks} clicks})</h2>
                  <h3>{this.props.headerText}</h3>
                  {children}
              </div>
          );
      }
  }

  ```
  After mounting the `MyComponent` component in the DOM tree, a `clickHandler()`
  event is assigned to the` myComponentDiv`. This feature increases one click
  count by updating component state. The default/initial number of clicks is stored
  in the component state, and is 0. In render() via JSX, we display html elements,
  page content, values from the component state or other properties assigned
  to that component by framing them in parentheses {}.
  When a component is unmounted in the `componentWillUnmount ()` function,
  it is removed an event that listens for clicks.

  * What happens when you call setState?
    I change the value in the component state what is captured by React
    And it leads to re-rendering of the component with child elements in the virtual DOM.

    http://lucybain.com/blog/2017/react-js-when-to-rerender/
    
*  What’s the difference between an Element and a Component in React?
    Element:
    - Describes the DOM tree
    - They do not have their own methods
    - This is a syntax sugar for React.createElement (element)
    - Element can be created without defined
    - Within the component, you can create multiple elements and package them into another element
    - They are not an instance of a component and describe how a component instance should look

    Component:
    - May have his state
    - The component must be defined eg by React.Component
    - The render () function returns the DOM element tree
    - Has access to life cycle methods

* When would you use a Class Component over a Functional Component?
    The class component should be used when I know that the class will have its own state.
    And when I want to use lifecycle methods.
    The function component can be used when the component has no state,
    I can use eg. const, arrow function or other ES6 syntax features.
    
* What are refs in React and why are they important?
    Used to return a reference to an element. They are useful to manipulating
    the DOM tree and adding methods to components. They are  recommend as a last resort.

 * What are keys in React and why are they important?
    When we render repetitive elements eg. a list with .map each <li> element
    must have its own unique key in the DOM tree. So we give such an element
    property <li key = {key}>.
    This is important because in React not everything has its mapping in the virtual DOM,
    Some changes, without assigning unique keys, may remain unnoticed.

    https://coderwall.com/p/jdybeq/the-importance-of-component-keys-in-react-js


#### JS Questions:

* Explain event delegation
    Event delegation consists in bundling an event handler into a parent rather than an element that we want to handle.
    When we click on an interior element, the event bubbles up to the item assigned to the handler.
    Then, with event.target, we can see where the event occurred and execute it on the corresponding element.
    This allows us to handle events occurring on multiple items with one handler.

    http://www.crimsteam.site90.net/crimsteam/dom/dom_zdarzenia_delegacja.html
    https://davidwalsh.name/event-delegate

* Explain how `this` works in JavaScript
    `this` points to an object depending on the function context in which it was declared.
    Context, ie the way and place of the call.

    Global context:
    console.log(this === window); // true
    this.a = 37;
    console.log(window.a); // 37
    As an object method:
    var o = {  prop: 37, f: function() { return this.prop; }};
    console.log(o.f()); // logs 37

    https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/Operatory/this
    http://stackoverflow.com/questions/3127429/how-does-the-this-keyword-work

* Explain how prototypal inheritance works
    Prototypal inheritance means prototypes of objects are linked,
    which means, that when some property is used it is first searched at the object,
    then (when not found) on its prototype and so on

* What do you think of AMD vs CommonJS?
    Both specifications describe the format and manner in which modules and their dependencies should be defined.
    The main difference between AMD (Asynchronous Module Definition) and CommonJS is the asynchronous loading of modules in AMD.

    AMD:
     - Used in browsers, asynchronous loading of modules
     - define('module', [dependencies], function module() { return contents });
    CommonJS:
     - On backend - Formerly used in NodeJS, nowadays less popular.
     - exports / module.exports | require

     https://auth0.com/blog/javascript-module-systems-showdown/

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
    - Callbacks
    - IIFE's
    - Closures
    
* How do you organize your code? (module pattern, classical inheritance?)
  Eg. Module pattern, IIFE, Atomic design.

* What's the difference between host objects and native objects?
    Host objects are objects provided by the host environment. They may be different between environments, examples:
    - window, document, location
    Native objects are the ones described and fully defined in the ECMAScript specification, examples:
    - Date, Math, parseInt.
    http://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects

* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
  - A Function Declaration defines a named function variable without requiring variable assignment.
  - Assigns to the person variable the value returned by the person function, in this case undefined
  - Assigns a Person object to person variable, with this assigned to the person object
  https://javascriptweblog.wordpress.com/2010/07/06/function-declarations-vs-function-expressions/

* How you can achieve inheritance in JavaScript (new + Object.create)

- With a constructor

A "constructor" in JavaScript is "just" a function that happens to be called with the new operator.
In constructor functions, the newly created object inherits from the constructor's prototype.
In the new Function() form the declared properties/functions do not form the prototype.

- With Object.create

ECMAScript 5 introduced a new method: Object.create(). Calling this method creates a new object. The prototype of this object is the first argument of the function
Object.create builds an object that inherits directly from the one passed as its first argument. Object.create doesn't execute the constructor function.

- With the class keyword

ECMAScript 2015 introduced a new set of keywords implementing classes. Although these constructs look like those familiar to developers of class-based languages, they are not the same. JavaScript remains prototype-based. Classes are just a syntactic sugar for creating object using constructor.

Difference new vs Object.create![Difference new vs Object.create](http://stackoverflow.com/questions/4166616/understanding-the-difference-between-object-create-and-new-somefunction)

* What's the difference between `.call` and `.apply`?
    You can use `.call` and` .apply` to assign another object when calling an existing function.
   `This` refers to the current object.
    So you can write the method once and then inherit it in another object, without rewriting the method for the new object.
    Call accepts `this` and single arguments, and apply as an array.
    theFunction.apply(valueForThis, arrayOfArgs)
    theFunction.call(valueForThis, arg1, arg2, ...)
    http://stackoverflow.com/questions/1986896/what-is-the-difference-between-call-and-apply
    https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/Obiekty/Function/apply
    https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Function/call

* Explain `Function.prototype.bind`.
    Bind creates a new function that allows `this` to be assigned to the context we want.
    Because in callback the value of the current object `this` may not be what we expect.
    It also allows you to assign default arguments to the returned function:
      var Person = function (name) { this.name = name; };
      Person.prototype.speak = function (volume) {return this.name +  volume };
      var person = new Person("John");
      var f = person.speak.bind(person, "loudly");
      // "John loudly"
      http://www.kurshtml.edu.pl/js/bind,function-prototype.html

* When would you use `document.write()`?
  Document.write() is always available, it is a good choice for third party vendors to use it to add their scripts.
  Many generated ads use `document.write ()` although it is not welcome.

* What's the difference between feature detection, feature inference, and using the UA string?
    Feature detection is the detection of whether a feature / functionality is available in an executable environment
    eg: return !!document.createElement('canvas').getContext; // return true or false

    Feauture inference is based on the assumption that if a given functionality is available in a given browser version, then the rest of the functionality also. They are then used without checking if they exist, which can lead to errors.

    UA string defaults return the version of the browser that executes the query that runs the js script. UA string can be changed by the client.

    http://lucybain.com/blog/2014/feature-detection-vs-inference/

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
    JavaScript Object Notation with Padding - remote AJAX outside the domain.
    Allows you to retrieve data from servers located in another domain,
    Than the domain where script.js is started. Helps to bypass Same-origin policy.
    JSONP allows you to retrieve JSON data by wrapping data into a JS function,
    This makes it possible to run an external js script by adding it using a script tag.
    In order to start the JSON return function we need to specify a callback in the url like the JSON wrapper function.
    - `http://www.example.net/sample.aspx?callback=mycallback`
    - Can only be used with GET queries

    http://stackoverflow.com/questions/2067472/what-is-jsonp-all-about

* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
    I only used Handlebars for simple scripts that needed to fill a lot of data in a loop.
    Popular templates:
    - Mustache
    - Underscore
    - Embedded JS

* Explain "hoisting".
    Hoisting is the lifting of variables with assigned value and functions
    up to the very top (to global reach or function coverage).
    Which allows them to be used before they are declared.
    x = 5; // Assign 5 to x
    elem = document.getElementById("demo"); // Find an element
    elem.innerHTML = x; // Display x in the element
    var x; // Declare x

* Describe event bubbling.
    Bubbling is an event passing up of the DOM tree.
    When an event occurs in an element inside another element,
    and both elements have registered a handle for that event.
    With bubbling, the event is first captured and handled by the innermost element
    and then propagated to outer elements.

    http://stackoverflow.com/questions/4616694/what-is-event-bubbling-and-capturing

* What's the difference between an "attribute" and a "property"?
    Attribute is a value in HTML itself, which is always a string
    JS DOM objects have properties. These properties are kind of
    like instance variables for the particular element.
    As such, a property can be different types (boolean, string, etc.).

    http://lucybain.com/blog/2014/attribute-vs-property/

* What does second parameter in Object.create do?

It specify property descriptors to be added to the newly-created object, with the corresponding property names. These properties correspond to the second argument of Object.defineProperties().

Object.create![Object.create](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Object/create)


* Why is extending built-in JavaScript objects not a good idea?

    Because these objects were created according to some well-documented
    and well-thought-out specifications. If we add our methods to the built-in object,
    they can be overwritten by an unknowable developer using our code,
    developers may implement a method with the same name.

* Does extending built-in objects have good part?
    You can use features that are not normally available for a given method.
    For example, reverse the string using the `reverse` method from the Array.
    String.prototype.reverse = function() {
      return Array.prototype.reverse.apply(this.split('')).join('');
    };
    https://code.tutsplus.com/tutorials/quick-tip-how-to-extend-built-in-objects-in-javascript--net-9168

* Does JavaScript have private methods?

Yes, private methods are made by the constructor. Every function definition or function expression (not bound with this) will become private method.
Private methods cannot be called by public methods.

Private members![Crockford on private members](http://javascript.crockford.com/private.html)

* Difference between document load event and document DOMContentLoaded event?
    The DOMContentLoaded event is fired when the document has been completely loaded and parsed the DOM tree,
    the load event will do it when all the images and sub-frames have finished loading.
    http://stackoverflow.com/questions/2414750/difference-between-domcontentloaded-and-load-events

* What is the difference between `==` and `===`?
`==` Compares values by making coerces if the types of variables are not the same
`===` Compares the values and types of variables without making coercion

* Whats a function declaration and function expression? What are the differences?

The function declaration defines a function with the specified name and parameters.
Function expression is almost identical, but i allows to omit function name, thus creating annonymous function. Function expressions can be used as an IIFE. Function expressions (not like function declartion) arent hoisted.

Function delcaration![Function delcaration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)
Function expression![Function expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function)
Function declaration vs function expression![Function declaration vs function expression](https://www.sitepoint.com/function-expressions-vs-declarations/)

* Are the functions hoisted?
    In JS, functions can be declared in two ways: by function definition and function expression.
    Function definition are hoisted, whereas function expressions do not.
    Function hoisting![Function hoisting](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)
    
* Explain the same-origin policy with regards to JavaScript.
  This is a fundamental security mechanism of the browser.
  This mechanism prevents js scripts from accessing the DOM trees of different origins.
  The same origin occurs when the port protocol and the host
  of the pages that trigger the scripts are compatible.

* Describe inheritance patterns in JavaScript.
  - Pseudoclassical pattern - Constructors/classes are created by `new`,
    inheriting all methods and properties of the parent.
    By creating an instance with `new` we bind it to` this`.
    Class methods refer to `this` instance.
  - Functional pattern - It contains all the methods and properties within the constructor function.
  - Prototypal pattern - Expands the class/constructor to successive subclasses inheriting all parent methods and properties.

  http://wes.is/2014/12/14/why-i-prefer-the-pseudoclassical-pattern-for-creating-classes-in-javascript-and-why-you-should-too/

* Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
  ```javascript
  function duplicate(arr) {
    return arr.concat(arr);
  }
  ```
  Reference: [Array.prototype.concat](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)
* Why is it called a Ternary expression, what does the word "Ternary" indicate?

  The word "Ternary" indicates that a Ternary expression takes three operands.
  It's the only JavaScript operator that takes three operands.
  Reference: [Conditional (ternary) Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

* What is `"use strict";`? what are the advantages and disadvantages to using it?

  "use strict" turns on more restricted variant of JavaScript.
  It has different semantics than a normal code.

  Advantages:
    - Eliminates some JavaScript silent errors by changing them to throw errors.
    - Fixes mistakes that make it difficult for JavaScript engines to perform optimizations (strict mode version might be slightly faster than a normal version).
    - Prohibits some syntax that is likely to be defined in the future versions of ECMAScript.

  Disadvantages:
    - Browsers not supporting strict mode will run strict mode code with different behavior from browsers that do.
  
  Reference: [Strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode)

* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`

```javascript
  for(let i = 1; i <= 100; i += 1) console.log((i % 3 === 0 ? 'fizz' : '') + (i % 5 === 0 ? 'buzz' : ''));
```

* Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?

It is generally a good idea to leave the global scope untouched, because all code share a single global namespace.
Relying too much on global variables can result in collisions between various scripts on the same page.
The best solution for avoiding global space pollution is IIFE.

Reference: [Global variables disscusion](http://stackoverflow.com/questions/2613310/ive-heard-global-variables-are-bad-what-alternative-solution-should-i-use)

* What is a callback?

Callback is a function that is passed to the other function as an argument. Function that gets callback as argument can invoke it in its body. This execution may be immediate as in a synchronous callback, or it might happen at a later time as in an asynchronous callback.

[Callback](https://en.wikipedia.org/wiki/Callback_(computer_programming))

* Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?

The `load` event is fired when a resource and its dependent resources have finished loading.
It can be used to check when a page is ready to use (fully-loaded page).
One of disadvantages is that the `load` event waits for everything to be ready - even stylesheets and images.
The most recommended alternative is `DOMContentLoaded` event which is fired when the initial HTML document has been completely loaded and parsed.

* Which JavaScript patterns do you know?

- Guard pattern
In computer programming, a guard is a boolean expression that must evaluate to true if the program execution is to continue in the branch in question. Regardless of which programming language is used, guard code or a guard clause is a check of integrity preconditions used to avoid errors during execution.

- Constructor pattern
Object constructors are used to create specific types of objects - both preparing the object for use and accepting arguments which a constructor can use to set the values of member properties and methods when the object is first created.

- Module pattern
In JavaScript, the Module pattern is used to further emulate the concept of classes in such a way that we're able to include both public/private methods and variables inside a single object, thus shielding particular parts from the global scope. What this results in is a reduction in the likelihood of our function names conflicting with other functions defined in additional scripts on the page.

- Singleton pattern
The Singleton pattern is thus known because it restricts instantiation of a class to a single object. Classically, the Singleton pattern can be implemented by creating a class with a method that creates a new instance of the class if one doesn't exist. In the event of an instance already existing, it simply returns a reference to that object.

In JavaScript, Singletons serve as a shared resource namespace which isolate implementation code from the global namespace so as to provide a single point of access for functions.

Participants

- Singleton:
  - defines getInstance() which returns the unique instance.
  - responsible for creating and managing the instance object.

- Observer pattern
The Observer is a design pattern where an object (known as a subject) maintains a list of objects depending on it (observers), automatically notifying them of any changes to state.

When a subject needs to notify observers about something interesting happening, it broadcasts a notification to the observers (which can include specific data related to the topic of the notification).

When we no longer wish for a particular observer to be notified of changes by the subject they are registered with, the subject can remove them from the list of observers.

  Participants

  - Subject:
    - maintains list of observers. Any number of Observer objects may observe a Subject
    - implements an interface that lets observer objects subscribe or unsubscribe
    - sends a notification to its observers when its state changes
  - Observers - has a function signature that can be invoked when Subject changes (i.e. event occurs)


- Strategy
The Strategy pattern encapsulates alternative algorithms (or strategies) for a particular task. It allows a method to be swapped out at runtime by any other method (strategy) without the client realizing it. Essentially, Strategy is a group of algorithms that are interchangeable.

  Participants: 
  - Context:
    - maintains a reference to the current Strategy object
    - supports interface to allow clients to request Strategy calculations
    - allows clients to change Strategy
  - Strategy - implements the algorithm using the Strategy interface

DotFactory patterns![DotFactory patterns](http://www.dofactory.com/javascript/design-patterns)
JavaScript Design Patterns![JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)

* Explain what a single page app is and how to make one SEO-friendly.

A single-page application (SPA) is a web application or web site that fits on a single web page with the goal of providing a user experience similiar to that of a desktop application. In an SPA, either all necessary code - HTML, JavaScript and CSS - is retrieved with a single page load, or dynamically loaded and added to the page as necessary.
The page does not reload at any point in the process, although the `location hash` or the `HTML5 History API` can be used to provide the perception and navigabillity of separate logical pages in the application.
The page can be SEO-friendly by enabling server-side rendering and using HTML5 semantics.

[Single-page application](https://en.wikipedia.org/wiki/Single-page_application)

* What is the extent of your experience with `Promises` and/or their polyfills?

I've been using `Promises` for some time now, probably about half of a year.
Thanks to `Promises` my asynchronous code looks better and I dont get stuck in a callback hell.
The only polyfill I've used is `Bluebird`.

* Whats a Promise ?

The Promise object is used for asynchronous computations. A Promise represents a value which may be available now, or in the future, or never.
A Promise is in one of these states:

- pending: initial state, not fulfilled or rejected.
- fulfilled: meaning that the operation completed successfully.
- rejected: meaning that the operation failed.

A pending promise can either be fulfilled with a value, or rejected with a reason (error). When either of these options happen, the associated handlers queued up by a promise's then method are called.

[Promise](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Promise)

* What are the pros and cons of using Promises instead of callbacks?

Pros:
  - Avoiding "callback hell".
  - More flexibility.
  - Rich interface.
  - Error handling.

Cons:
  - The envoirnment needs to support promises.
  - Complexity.

* Variables scope in JS?

In JavaScript, til version ES6, there were only two versions of variables scope - global scope, and local - function scope.
In ES6 there is one more - block scope for variables defined with let and const (scope in {}).

[var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)
[let](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Statements/let)
[const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
[other scopes](http://stackoverflow.com/a/500459)

* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?

Pros:
  - Typos caught at compilation time.
  - Simplier syntax.
  - Better maintainability.

Cons:
  - In order to run the application in a browser, a compile step is required.
  - Debugging can be a pain.
  - Learning new language / syntax.
  - Smaller community, generally less resources avaible.

Reference: [Typescript pros and cons](https://designmodo.com/typescript/),
[Javascript, CoffeScript, Dart and TypeScript](https://smthngsmwhr.wordpress.com/2013/02/25/javascript-and-friends-coffeescript-dart-and-typescript/)

* What tools and techniques do you use debugging JavaScript code?

I'm using Chrome DevTools.
Im using the following techniques:
  - Break on node changes.
  - XHR breakpoints.
  - Pause on exception.
  - Audits (optimization).

Reference: [Tips & tricks](http://www.zsoltnagy.eu/javascript-debugging-tips-and-tricks/)

* What are falsy values

Falsy values are values that evaluate to false when they're converted to boolean:
- 0
- "" - empty string
- null
- undefined
- NaN
- false

Falsy values![MDN falsy values](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)

* Types in Javascript

JS types can be split in two categories - primitives and objects

Primitives are:
- String
- Number
- Boolean
- null
- undefined
- Symbol (from ES6)

Not primitive type is Object type ie:
- Array
- Date
- Function
- Map, WeakMap
- Set, WeakSet

Primitive types are passed by value, objects are passed by reference.

Javascript Types![Javascript Data Types](https://developer.mozilla.org/pl/docs/Web/JavaScript/Data_structures)

* What language constructions do you use for iterating over object properties and array items?

For iterating over object properties I use for... in loop with hasOwnProperty property checking.
For iterationg over array items I use for loop and methods of Array.prototype, for example .forEach, and .map.

Reference: [hasOwnProperty](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty),
[Array.prototype](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype)

* Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?

A mutable object is a object that can be changed.
An immutable object is a object than can't be changed. Instead on every change it returns new object.

Pros:
  - Less complicated in using.
  - Operations can be chained.
  - Can be easily copied.
  - Never changes.
  - Can be shared easily.
  - Easy debugging.

Cons:
  - More memory usage.
  - Sometimes difficult to build.

Immutability can be achieved by using Object.freeze and Object.seal.
Also a library like Immutable.js can be used.

Reference: [Discussion on Quora](https://www.quora.com/What-are-the-advantages-and-disadvantages-of-immutable-data-structures),
[Discussion on Stackoverflow](http://stackoverflow.com/questions/1863515/pros-cons-of-immutability-vs-mutability)

* Explain the difference between synchronous and asynchronous functions.

Synchronous function will be executed and finished before moving on to another task.
Asynchronous function will be executed and whether its finished or not another next task will be executed.

Reference: [Asynchronous vs synchronous](http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean)

* Are functions hoisted in js?

There are two ways of declaring a function in JS: function definition and function expression.
Function definitions are hoisted, function expressions arent.

* What is event loop?
  * What is the difference between call stack and task queue?

The event loop got its name because of how it's usually implemented, which usually resembles:

```javascript
while (queue.waitForMessage()) {
  queue.processNextMessage();
}
```

queue.waitForMessage waits synchronously for a message to arrive if there is none currently.
Each message is processed completely before any other message is processed. 
This offers some nice properties when reasoning about your program, including the fact that whenever a function runs, 
it cannot be pre-empted and will run entirely before any other code runs (and can modify data the function manipulates).

A call stack is a queue of functions that are being executed.
Task queue is a list of messages waiting to be processed. 
A function is associated with each message. When the stack has enough capacity, a message is taken out of the queue and processed.

* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`.

There is a function declaration (first one) and function expression (second one).
The usage is almost the same, except for one thing. 
Calling foo before a declaration (first case) the function will be called, because functions are hoisted.
Calling foo before an expression (second case) will result in throwing error, because, even though, variables are hoisted too, their value is undefined untill the declaration.

```javascript
foo(); // ok
boo(); // TypeError: boo is not a function

function foo() {};
var boo = function () {};
```

* What is inheritance?

Inheritance (in programming) is a mechanism that allow sharing functionality (and code reuse) beetwen classes and/or objects (in classical inheritance) or between objects (in prototypal inheritance - like in JS). Class that inherits (called subclass) gains acess to all shared behaviors and attributes of parent class (called superclass);

Inheritance![Wikipedia - Inheritance](https://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming))

* Whats the difference between inheritance in JS and the classical inheritance?

Classical inheritance inherits the behavior, without any state, from the parent class. It inherits the behavior at the moment the object is instantiated.

Prototypal inheritance inherits behavior and state from the parent object. It inherits the behavior and state at the moment the object is called. When the parent object changes at run-time, the state and behavior of the child objects are affected.

Classical vs Prototypal![Stackoverflow - classical vs prototypal](http://softwareengineering.stackexchange.com/a/99438)

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

* How do you test apps? What kinds of tests do you know? What tools do you use to those types of tests? (please include in response links to videos about those tests types)
* What should you test with unit tests?
* What should you test with e2e tests?
* What's BDD? What's TDD?
* What is code coverage?
* What elements do you test?

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

  * Graphics size should be adjusted to the size of their containers, they should be optimized so as not to take to much bandwidth.
  * Avoid using large amounts of box-shadows and other styles that require more work to draw by the browser.
  * Avoid JavaScript methods/properties that cause reflow/repaint the page, such as elements offsets, container sizes etc.
  * Use debouncing with scrolling events.

* Explain the difference between layout, painting and compositing.

  * layout - in this phase the browser checks how much space each of the page elements need.
  * painting - filling in pixels, drawing elements: text, graphics etc.
  * compositing - showing of elements on the page in the correct order - rendering of the page.

  [source](https://developers.google.com/web/fundamentals/performance/rendering/?hl=en)

#### Network Questions:

* Traditionally, why has it been better to serve site assets from multiple domains?

  Doing so increases page loading speed:
  * Parallelization - it allows to send multiple request at once to many servers, which decreases the loading time of assets overall.
  * Reduced header overhead - usually servers send clients some cookies, which are then attached to every client request in the same domain as the site. Serving static content from different domains than the server allows the client to skip sending the headers.

  [source](https://travishorn.com/why-it-is-better-to-serve-site-assets-from-multiple-domains-972a2bf69d71)

* Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.

  1. Get the servers IP address based on the URL from the DNS.
  2. Send an HTTP request to the server.
  3. Parse the response and render the page.

  [more details](http://stackoverflow.com/a/2092602)

* What are the differences between Long-Polling, Websockets and Server-Sent Events?

  * Long-polling - The client sends a request, and when the server has a new information to report it sends it to the client. This process is one-off.
  * WebSockets - The client connects to the server and the connection is maintained. The client can then exchange information with the server.
  * Server-Sent Events - The client connects to the server by sending a request, this connection is maintained. The server can then send new information to the client as it becomes available. In comparison to WebSockets, the connection is unidirectional.

  [more info](http://stackoverflow.com/a/12855533)

* Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-Since
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options

  * Date - the date when the message was sent.
  * Expires - the date after which the message is considered stale.
  * Age - the number of seconds the object has been in the proxy cache.
  * If-Modified-Since - allows the server to return 304 code when the message wasn't change since the date inside this header.
  * DNT (Do Not Track) - asks the server not to track the user.
  * Cache-Control - controls the options related to caching, eg. for how long should the response be cached.
  * Transfer-Encoding - form of encoding used on the message, eg.: chunked, compress, deflate, gzip, identity.
  * ETag - may be used for versioning of the resource.
  * X-Frame-Options - controls the clickjacking protection.

  [source](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)

* What are HTTP methods? List all HTTP methods that you know, and explain them.

  HTTP methods indicate an action the client wants to be performed on the specified resource.

  * GET - retrieves a resource without changing it.
  * HEAD - same as GET, but doesn't retrieve the actual body. May be useful when only the headers are needed.
  * POST - adds a new resource.
  * PUT - updates the resource.
  * DELETE - deletes the resource.
  * TRACE - echoes data sent in the request back to the client.
  * OPTIONS - returns the methods that the server supports for the specified URL.
  * CONNECT - converts the connection to a TCP/IP tunnel.
  * PATCH - applies partial modifications to the resource.

  [source](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Request_methods)

#### Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

  `1020` (string)

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

  ```javascript
  const add = (a, b) => {
  if (!b) {
    return b => a + b;
  }

  return a + b;
  };
  ```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

  `goh angasal a m'i`

*Question: What is the value of `window.foo`?*
```javascript
( window.foo || ( window.foo = "bar" ) );
```

  If `window.foo` was already set then it retains the previous value, if not then the value is `bar`.

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

  Second alert call will fail because of the `bar` variable being set in a different block-scope.

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

  `2`

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

  `undefined` - after `x` is set in `foo`, the `foo` is assigned a different object that doesn't have `x` set. `x` is still assigned in the previous object, which is now in a variable named `bar`.

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

  ```
  one
  three
  two
  ```
  
### AngularJS Questions:

* What is AngularJS?
  AngularJS is a client side JavaScript MVC framework to develop a dynamic web application. AngularJS was originally started as a project in Google but now, it is open source framework.
  AngularJS is entirely based on HTML and JavaScript, so there is no need to learn another syntax or language.
  AngularJS changes static HTML to dynamic HTML. It extends the ability of HTML by adding built-in attributes and components and also provides an ability to create custom attributes using simple JavaScript. 

  https://docs.angularjs.org/guide/introduction
  http://www.tutorialsteacher.com/angularjs/what-is-angularjs
* Explain ng-controller directive.
  The ng-controller directive attaches a controller class to the view. This is a key aspect of how angular supports the principles behind the Model-View-Controller design pattern. It also creates a new scope.
* Which components can be injected as a dependency in AngularJS?
  - Services, directives, filters, animations
  - Controllers
  - Run method
  - Providers
  - Factories

* What are the differences between service and factory methods?
  - service is a constructor function, factory is not
  - factory returns an object
  - services allow to use ES6 classes

  https://blog.thoughtram.io/angular/2015/07/07/service-vs-factory-once-and-for-all.html
* What is scope hierarchy in AngularJS?
  The $scope object used by views in AngularJS are organized into a hierarchy. There is a root scope, and the $rootScope can has one or more child scopes. Each controller has its own $scope (which is a child of the $rootScope), so whatever variables you create on $scope within controller, these variables are accessible by the view based on this controller.

  http://www.dotnettricks.com/learn/angularjs/understanding-scope-inheritance-in-angularjs
  
* What is $rootScope?
  $rootScope refers to an object which is accessible from everywhere of the application. You can think $rootScope as global variable and $scope as local variables.

* What is use of $routeProvider in AngularJS?
  $routeProvider is used for configuring routes in app.

  https://docs.angularjs.org/api/ngRoute/provider/$routeProvider

* Explain ng-include directive.
  It is the way to fetch, compile and include templates/html fragment from external files.

* How to make an ajax call using Angular JS?
  You can make ajax calls using services $http or $https.
  ```
  $http({
    method: 'GET',
    url: '/someUrl'
  }).then(function successCallback(response) {
    // this callback will be called asynchronously
    // when the response is available
  }, function errorCallback(response) {
    // called asynchronously if an error occurs
    // or server returns response with an error status.
  });
  ```

* How to validate data in AngularJS?
  You can use two-way data-binding (ng-model) to validate data. Validation happens in the model, where you have a lot of options to validate data using JavaScript and its methods. 

  AngularJS provides basic implementation for most common HTML5 input types: (text, number, url, email, date, radio, checkbox), as well as some directives for validation (required, pattern, minlength, maxlength, min, max).

* What are the basic steps to unit test an AngularJS filter?
  1. Inject '$filter'
  2. Call it with '$filter(filterName)(input, options)'
  Example:
  ```
  describe('The test filter', function () {
  'use strict'; 

  var $filter;

  beforeEach(function () {
    module('myTestFilterModule');

    inject(function (_$filter_) {
      $filter = _$filter_;
    });
  });

    it('should capitalize a string', function () {
      // Arrange.
      var foo = 'hello world', result;

      // Act.
      result = $filter('testFilter')(foo, 'capitalize');

      // Assert.
      expect(result).toEqual('HELLO WORLD');
    });
  });
  ```
  
  http://stackoverflow.com/questions/21094569/how-to-unit-test-a-filter-in-angularjs-1-x

* What is data binding in AngularJS?
  
  Data-binding in AngularJS apps is the automatic synchronization of data between the model and view components. The way that AngularJS implements data-binding lets you treat the model as the single-source-of-truth in your application. The view is a projection of the model at all times. When the model changes, the view reflects the change, and vice versa.

  https://docs.angularjs.org/guide/databinding

* What is scope in AngularJS?

  Scope is an object that refers to the application model. It is an execution context for expressions. Scopes are arranged in hierarchical structure which mimic the DOM structure of the application. Scopes can watch expressions and propagate events.

  https://docs.angularjs.org/guide/scope

* What are the controllers in AngularJS?

  In AngularJS, a Controller is defined by a JavaScript constructor function that is used to augment the AngularJS Scope.
  When a Controller is attached to the DOM via the ng-controller directive, AngularJS will instantiate a new Controller object, using the specified Controller's constructor function. A new child scope will be created and made available as an injectable parameter to the Controller's constructor function as $scope.
  If the controller has been attached using the controller as syntax then the controller instance will be assigned to a property on the new scope.

  Use controllers to:
    Set up the initial state of the $scope object.
    Add behavior to the $scope object.

  Do not use controllers to:
    Manipulate DOM — Controllers should contain only business logic. Putting any presentation logic into Controllers significantly affects its testability. AngularJS has databinding for most cases and directives to encapsulate manual DOM manipulation.
    Format input — Use AngularJS form controls instead.
    Filter output — Use AngularJS filters instead.
    Share code or state across controllers — Use AngularJS services instead.
    Manage the life-cycle of other components (for example, to create service instances).

  https://docs.angularjs.org/guide/controller

* What are the services in AngularJS?

  AngularJS services are substitutable objects that are wired together using dependency injection (DI). You can use services to organize and share code across your app.
  
  AngularJS services are:
    Lazily instantiated – AngularJS only instantiates a service when an application component depends on it.
    Singletons – Each component dependent on a service gets a reference to the single instance generated by the service factory.

  AngularJS offers several useful services (like $http), but for most applications you'll also want to create your own.

  https://docs.angularjs.org/guide/services

* What are the filters in AngularJS?

  Filters format the value of an expression for display to the user. They can be used in view templates, controllers or services. AngularJS comes with a collection of built-in filters, but it is easy to define your own as well.

  The underlying API is the $filterProvider.

  https://docs.angularjs.org/guide/filter

* Explain directives in AngularJS.

  At a high level, directives are markers on a DOM element (such as an attribute, element name, comment or CSS class) that tell AngularJS's HTML compiler ($compile) to attach a specified behavior to that DOM element (e.g. via event listeners), or even to transform the DOM element and its children.

  https://docs.angularjs.org/guide/directive

* Explain templates in AngularJS.

  In AngularJS, templates are written with HTML that contains AngularJS-specific elements and attributes. AngularJS combines the template with information from the model and controller to render the dynamic view that a user sees in the browser.

  These are the types of AngularJS elements and attributes you can use:
    Directive — An attribute or element that augments an existing DOM element or represents a reusable DOM component.
    Markup — The double curly brace notation {{ }} to bind expressions to elements is built-in AngularJS markup.
    Filter — Formats data for display.
    Form controls — Validates user input.

  https://docs.angularjs.org/guide/templates

* What is routing in AngularJS?

  AngularJS supports SPA using routing module ngRoute. This routing module acts based on the url. When a user requests a specific url, the routing engine captures that url and renders the view based on the defined routing rules.

  https://docs.angularjs.org/api/ngRoute/service/$route
  http://www.tutorialsteacher.com/angularjs/angularjs-routing

* What is deep linking in AngularJS?

  Deep linking is the usage of the URL, which will take to specific page (content) directly without traversing application from home page. It helps in getting indexed so that these links can be easily searchable by search engines like Google, Yahoo.. etc.

  Using Angular, the deep linking is defaut done with the # prefix (when the HTML5 mode is not set).

* What are the advantages of AngularJS?

  Built by Google
    AngularJS has been developed as well as maintained by dedicated Google engineers. This means that there is a huge community out there for you to learn from.
  Great MVC
    Most frameworks require programmers to splitting the app into multiple MVC components. After that, the programmer has to write a code to put them together again. AngularJS, however, strings it together automatically.
  Intuitive
    AngularJS is more intuitive as it makes use of HTML as a declarative language. Moreover, it is less brittle for reorganizing.
  Comprehensive
    AngularJS is a comprehensive solution for rapid front-end development. It does not need any other plugins or frameworks. Moreover, there are a range of other features that include Restful actions, data building, dependency injection, enterprise-level testing, etc.
  Unit Testing Ready
    AngularJS is unit testing ready, and that is one of its most compelling advantages.

* What are the disadvantages of AngularJS?

  Confusion
    There are multiple ways to do the same thing with AngularJS. Sometimes, it can be hard for novices to say which way is better for a task.
  Lagging UI
    If there are more than 2000 watchers, it can get the UI to severely lag. This means that the possible complexity of Angular Forms is limited. This includes big data grids and lists.
  Name Clashes
    With AngularJS, you don’t have the ability to compose many NG-apps on the same page. This can cause name clashes.

* Which are the core directives of AngularJS?

  - ng-app − This directive defines and links an AngularJS application to HTML.
  - ng-model − This directive binds the values of AngularJS application data to HTML input controls.
  - ng-bind − This directive binds the AngularJS Application data to HTML tags.

* Explain ng-model directive.

  The ng-model directive is used for two-way data binding in AngularJS. It binds `<input>`, `<select>` or `<textarea>` elements to a specified property on the $scope object. So, the value of the element will be the value of a property and vice-versa. 

* Explain ng-bind directive.

  The ng-bind directive binds the model property declared via $scope or ng-model directive or the result of an expression to the HTML element. It also updates an element if the value of an expression changes. 

* Explain ng-app directive of AngularJS.

  The ng-app directive is a starting point of AngularJS Application. It initializes the AngularJS framework automatically. AngularJS framework will first check for ng-app directive in a HTML document after the entire document is loaded and if ng-app is found, it bootstraps itself and compiles the HTML template.
  Typically ng-app directives should be placed at the root of an HTML document e.g. `<html>` or `<body>` tag, so that it can control the entire DOM hierarchy. However, you can place it in any DOM element.
  The AngularJS framework will only process the DOM elements and its child elements where the ng-app directive is applied.
  
#### NodeJS questions:

* What is an error-first callback?

  It is a type of callback where the first argument is always an error and other arguments are the result data. The dev can then make sure the function calling the callback executed without troubles by checking whether the error argument is not null.

* How can you avoid callback hells?

  * Keep your code shallow. Don't define callbacks inside callbacks, instead move all callbacks to a single block level and the use them by function name.
  * Modularize. Split your code into smaller pieces that each only have a single task.
  * Handle all errors. This is neccessary so a failed function doesn't pass bad or malformed data down the callback chain and possibly cause other functions to throw errors.

  [source](http://callbackhell.com/)

* What are Promises?

  Promises are used for asynchronous computations. A Promise represents a value which may be available now, in the future, or never.

  [source](https://developer.mozilla.org/pl/docs/Web/JavaScript/Reference/Global_Objects/Promise)

* What tools can be used to assure consistent style? Why is it important?

  So called code style linters (jshint, jslint, eslint, etc.) help you keep a consistent style. It is important because it helps you avoid introducing simple bugs at the stage of writing the code. It assures that code formatting is more consistent between members of the team.

* When would you use npm and when yarn?

  I would use yarn when time is of the essence or when offline installation of modules is required.

  [more info](https://yarnpkg.com/lang/en/)

* What's a stub? Name a use case!

  Stubs are functions used in testing to replace other functions.

  Use cases:

  * Replace problematic pieces of code.
  * Trigger code paths that wouldn't otherwise trigger, such as error handling.
  * Help test asynchronous code more easily.

  [source](https://semaphoreci.com/community/tutorials/best-practices-for-spies-stubs-and-mocks-in-sinon-js)

* What's a test pyramid? Give an example!

  A testing pyramid consists of 3 parts:
  * UI tests test the system just like a real live end user would. They mimic the user's interactions in the form.
  * Integration tests, like UI tests, test various layers of the application, but they don't do it through the UI.
  * Unit tests are tests developers write to prove to themselves, that the code they are writing works. It enables them to make changes, without fear of breaking everything.

  [source](http://www.agilenutshell.com/episodes/41-testing-pyramid)

* What's your favorite HTTP framework and why?

  There's a lot of them. Some of the more popular include Express, Koa and Meteor. My favorite one is Express, because it's simple, powerful and well-supported.

  [more info](http://nodeframework.com/)

* How can you secure your HTTP cookies against XSS attacks?

  Use HTTPOnly cookie flag, which disables access to the cookie from scripts.

  [more info](https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet#Bonus_Rule_.231:_Use_HTTPOnly_cookie_flag)

* How can you make sure your dependencies are safe?

  Use only tested libraries. A good way is to use the most popular ones, as they have a higher chance of errors being detected and fixed by the community. Another way is to freeze a known good version of a library in npm, so it doesn't get updated to an unstable and possibly buggy version, though this requires manual updating in case a newer version contains a bug-fix for the version that's freezed in npm.

* How does Node.js handle child threads?

  Every Node.JS process is single-threaded, therefore to get multiple threads one must use multiple processes. Node.JS provides a `child_process` module that helps with this.

  [more info](https://nodejs.org/api/child_process.html)

* What is the preferred method of resolving unhandled exceptions in Node.js?

  By adding a listener for the `uncaughtException` process-level event:

  ```javascript
  process.on('uncaughtException', function(err) {
    // Handle error
    console.log(err);
  });
  ```

* How does Node.js support multi-processor platforms, and does it fully utilize all processor resources?

  Node.JS is a single-threaded application, and as such it will run only on a single core of a system. Node.JS provides a way to create multiple instances in the form of `cluster` module, which aids in fully utilizing system resources.

  [more info](https://nodejs.org/api/cluster.html)

* What is typically the first argument passed to a Node.js callback handler?

  First argument in a callback is usually an error object if the function failed, or null if the function succeeded.

* Consider the following JavaScript code:
```javascript
console.log("first");
setTimeout(function() {
    console.log("second");
}, 0);
console.log("third");
```

  The output will be:
  ```
  first
  third
  second
  ```

  Assuming that this is the desired behavior, and that we are using Node.js version 0.10 or higher, how else might we write this code?

  Answer:

  Instead of using `setTimeout`, we can use `setImmediate` (behind all I/O events) or `process.nextTick` (ahead all I/O events)

* What is Event Loop?

  The event loop allows Node.JS to offload operations to system kernel, which in turn allows Node to handle multiple background operations at the same time. When the operation completes, the kernel tells Node.JS so that it can add appropriate callbacks to the poll queue.

  [more info](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

* What is the purpose of Buffer object in Node?

  Buffers allow devs to manipulate and temporarily store binary data, as well to act as buffers for streams.

  [more info](https://nodejs.org/api/buffer.html)

* Which types of streams are present in Node?

  * writable
  * readable
  * duplex - implements both writable and readable streams.
  * transform - similar to duplex, but also allows transformation of passing data.
  * passthrough - similar to duplex, but the writable and readable parts are connected, everything that comes in on the writable side will come out unchanged on the readable side.

  [source](https://nodejs.org/api/stream.html)

* Name some of the events fired by streams in Node

  error, close, end, finish, data, pipe, unpipe, readable

  [source](https://nodejs.org/api/stream.html)

* What is Chaining in Node?

  Chaining methods allows devs to use the result of a function call without assigning it to a variable first, for example:

  ```javascript
  const result =
    [1,2,3,4,5]
      .filter(val => val > 1)
      .map(val => val * val)
      .reduce((a, b) => a + b);

  console.log(result); // 55
  ```

* What is the purpose of process object?

  Process object is a global object that gives information about the underlying Node.JS process, such as: arguments passed to the process, environmental variables, memory usage etc.

  [more info](https://nodejs.org/api/process.html)

* What is MVC?
  MVC is a software architecture - the structure of the system - that separates domain/application/business logic from the rest of the user interface. It does this by separating the application into three parts: the model, the view, and the controller.

  The model manages fundamental behaviors and data of the application. It can respond to requests for information, respond to instructions to change the state of its information etc. This could be a database, or any number of data structures or storage systems. In short, it is the data and data-management of the application.

  The view effectively provides the user interface element of the application. It'll render data from the model into a form that is suitable for the user interface.

  The controller receives user input and makes calls to model objects and the view to perform appropriate actions.

  All in all, these three components work together to create the three basic components of MVC.

  http://softwareengineering.stackexchange.com/questions/127624/what-is-mvc-really

#### Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Who inspires you in the front-end community?
* Do you have any pet projects? What kind?
* What's your favorite feature of Internet Explorer?
* How do you like your coffee?


#### React Questions

* If you created a React element like Twitter below, what would the component definition of Twitter look like?

```jsx
<Twitter username='tylermcginnis33'>
 {(user) => user === null
   ? <Loading />
   : <Badge info={user} />}
</Twitter>
```

props.children works just like any other prop in that it can pass any sort of data, not just the sorts that React knows how to render. Children passed to a custom component can be anything, as long as that component transforms them into something React can understand before rendering.

```jsx
import React, { Component, PropTypes } from 'react'
import fetchUser from 'twitter'
// fetchUser take in a username returns a promise
// which will resolve with that username's data.

class Twitter extends Component {
  state = {
    user: null,
  }

  componentDidMount () {
    fetchUser(this.props.username)
      .then((user) => this.setState({user}))
  }
  render () {
    return this.props.children(this.state.user)
  }
}

Twitter.propTypes = {
  username: PropTypes.String.isRequired,
};
```

Functions as children![Functions as children](https://facebook.github.io/react/docs/jsx-in-depth.html#functions-as-children)

* What is the difference between a controlled component and an uncontrolled component?

A controlled component is a component where React is in control and is the single source of truth for the form data. In those components value of the element is based on component state, not the DOM.

In uncontrolled components data is handled directly by the DOM. To access data you can use an event handler or a ref to get form values from the DOM.

Controlled components![Controlled components](https://facebook.github.io/react/docs/forms.html#controlled-components)
Uncontrolled components![Uncontrolled components](https://facebook.github.io/react/docs/uncontrolled-components.html)

* In which lifecycle event do you make AJAX requests and why?

AJAX request should be done in componentDidMount event lifecycle. It's because after AJAX call returns some data, in most cases we want to assign that date to the state of the component, and this can be done only on mounted components.

State and lifecycle![State and lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

* What does shouldComponentUpdate do and why is it important?

shouldComponentUpdate is important because of performance reasons.
If we know that a certain section of our UI isn’t going to change, there’s no reason to have React go through the trouble of trying to figure out if it should update it. By returning false from shouldComponentUpdate, React will assume that the current component, and all its child components, will stay the same as they currently are.

Optimizing performance![Optimizing performance](https://facebook.github.io/react/docs/optimizing-performance.html)

* How do you tell React to build in Production mode and what will that do?

Typically you’d use Webpack’s DefinePlugin method to set NODE_ENV to production. This will strip out things like propType validation and extra warnings.

Development and production![Development and production](https://facebook.github.io/react/docs/installation.html#development-and-production-versions)

* Why would you use React.Children.map(props.children, () => ) instead of props.children.map(() => )

Because props.children can be an array but also a single component. If you'll pass single component then native map method will fail. React.Children.map handles both arrays of components and single components.

React.Children.map![React.Children.map](https://facebook.github.io/react/docs/react-api.html#react.children.map)

* Describe how events are handled in React.

In React native events are wrapped in SyntheticEvent instances, which solves cross browser compatibility issues. SyntheticEvent have the same interface as native events.
React doesn’t actually attach events to the child nodes themselves. React will listen to all events at the top level using a single event listener (due performance reasons).

Handling events![Handling events](https://facebook.github.io/react/docs/handling-events.html)

* What is the difference between createElement and cloneElement?

createElement is what JSX gets transpiled to and is what React uses to create React Elements (object representations of some UI). cloneElement is used in order to clone an element and pass it new props.

Create Element![Create Element](https://facebook.github.io/react/docs/react-api.html#createelement)
Clone Element![Clone Element](https://facebook.github.io/react/docs/react-api.html#cloneelement)

* What is the second argument that can be passed to setState and what is its purpose?

The setState is asynchronous so it takes also a callback function as the second argument. This function is invoked when setState has finished and the component is re-rendered.

setState![setState](https://facebook.github.io/react/docs/react-component.html#setstate)

* What is wrong with this code?

```jsx
this.setState((prevState, props) => {
 return {
   streak: prevState.streak + props.count
 }
})
```

Nothing. setState can also take a function as an argument. That function allows to set current state, based on previus state.

setState![setState](https://facebook.github.io/react/docs/react-component.html#setstate)

* How would you specify that a scope variable should have one-time binding only?

By using “::” in front of it.

#### Contributors:

This document started in 2009 as a collaboration of [@paul_irish](https://twitter.com/paul_irish) [@bentruyman](https://twitter.com/bentruyman) [@cowboy](https://twitter.com/cowboy) [@ajpiano](https://twitter.com/ajpiano)  [@SlexAxton](https://twitter.com/slexaxton) [@boazsender](https://twitter.com/boazsender) [@miketaylr](https://twitter.com/miketaylr) [@vladikoff](https://twitter.com/vladikoff) [@gf3](https://twitter.com/gf3) [@jon_neal](https://twitter.com/jon_neal) [@sambreed](https://twitter.com/sambreed) and [@iansym](https://twitter.com/iansym).

It has since received contributions from over [100 developers](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors).

* Is AngularJS extensible?  
Yes, in Angular we can create custom directive to extend AngularJS existing functionalities.  
https://docs.angularjs.org/guide/directive  

* What should be the maximum number of concurrent “watches”? Bonus: How would you keep an eye on that number?  
To reduce memory consumption and improve performance it is a good idea to limit the number of watches on a page to 2,000. A utility called ng-stats can help track your watch count and digest cycles.  
https://github.com/kentcdodds/ng-stats  

* How do you share data between controllers?  
Create an AngularJS service that will hold the data and inject it inside of the controllers. Using a service is the cleanest, fastest and easiest way to test. However, there are couple of other ways to implement data sharing between controllers, like: using events, usng $parent, nextSibling, controllerAs, etc. to directly access the controllers, using the $rootScope to add the data on (not a good practice).  
The methods above are all correct, but are not the most efficient and easy to test.  
https://daveceddia.com/sharing-data-between-controllers-best-practice-use-a-service/  
http://stackoverflow.com/a/21920241 
* Where should we implement the DOM manipulation in AngularJS?
Dom Manipulations theoretically should not exist in controllers, services or anywhere else but in directives. The currently suggested best practice is to use "components" (which can be realized via directives), where basically all the directive logic leaves in the controller. In that context, I believe it is perfectly fine to manipulate the DOM in a directive's template from within the directive's controller.  
http://ng-learn.org/2014/01/Dom-Manipulations/  
http://stackoverflow.com/questions/37480150/manipulating-dom-in-angularjs-best-practice  

* If you were to migrate from Angular 1.4 to Angular 1.5, what is the main thing that would need refactoring?  
Refactor code to use components.  
https://www.sitepoint.com/upgrade-to-angular-components/  

* What is the difference between ng-show/ng-hide and ng-if directives?  
The ngIf directive removes or recreates a portion of the DOM tree based on an expression. When an element is removed using ngIf its scope is destroyed and a new scope is created when the element is restored.  
The ngShow directive shows or hides the given HTML element based on the expression provided to the ngShow attribute. The element is shown or hidden by removing or adding the ng-hide CSS class onto the element. The .ng-hide CSS class is predefined in AngularJS and sets the display style to none (using an !important flag).  
http://stackoverflow.com/a/19177773  
* What is the difference between one-way binding and two-way binding?  
With two-way binding, if I change the reference Object and Primitive in the parent and the isolate Component, you’ll see both values continue to update. With one way data binding  You’ll be able to change the isolate bindings without affecting the parent scope. However, the $watch is setup on the parent data source, so when changes occur, it’ll propagate down and flow into the Component to update it with new data   
https://toddmotto.com/one-way-data-binding-in-angular-1-5/  
* Explain how $scope.$apply() works  
$scope.$apply() takes a function or an Angular expression string, and executes it, then calls $scope.$digest() to update any bindings or watchers.  
So, when do you need to call $apply()? Very rarely, actually. AngularJS actually calls almost all of your code within an $apply call. Events like ng-click, controller initialization, $http callbacks are all wrapped in $scope.$apply(). So you don’t need to call it yourself, in fact you can’t. Calling $apply inside $apply will throw an error.  
You do need to use it if you are going to run code in a new turn. And only if that turn isn’t being created from a method in the AngularJS library. Inside that new turn, you should wrap your code in $scope.$apply(). Here is an example. We are using setTimeout, which will execute a function in a new turn after a delay. Since Angular doesn’t know about that new turn, the update will not be reflected.  
http://jimhoskins.com/2012/12/17/angularjs-and-apply.html  

* How would you make an Angular service return a promise? Write a code snippet as an example  
To add promise functionality to a service, we inject the “$q” dependency in the service, and then use it like so:

```
angular.factory('testService', function($q){
 return {
  getName: function(){
   var deferred = $q.defer();

   //API call here that returns data
   testAPI.getName().then(function(name){
    deferred.resolve(name)
   })

   return deferred.promise;
  }
 }
})
```

https://docs.angularjs.org/api/ng/service/$q  

* When creating a directive, it can be used in several different ways in the view. Which ways for using a directive do you know? How do you define the way your directive will be used?  
When you create a directive, it can be used as an attribute, element or class name. To define which way to use, you need to set the restrict option in your directive declaration.  
The restrict option is typically set to:  
‘A’ – only matches attribute name  
‘E’ – only matches element name  
‘C’ – only matches class name  
'M' - only matches comment  
These restrictions can all be combined as needed:  
‘AEC’ – matches either attribute or element or class name  

* What makes the angular.copy() method so powerful?  
It creates a deep copy of the variable. A deep copy of a variable means it doesn’t point to the same memory reference as that variable. Usually assigning one variable to another creates a “shallow copy”, which makes the two variables point to the same memory reference. Therefore if we change one, the other changes as well.  
https://docs.angularjs.org/api/ng/function/angular.copy  

* When should you use an attribute directive versus an element?  
Use an element when you are creating a component that is in control of the template. Use an attribute when you are decorating an existing element with new functionality.   
https://docs.angularjs.org/guide/directive  

* How do you reset a $timeout, $interval(), and disable a $watch()?  
To reset a timeout and/or $interval, assign the result of the function to a variable and then call the .cancel() function on this variable. To disable $watch(), we call it.  

```
var customTimeout = $timeout(function () {
// arbitrary code 
}, 55);
$timeout.cancel(customTimeout);
var deregisterWatchFn = $rootScope.$watch(‘someGloballyAvailableProperty’, function (newVal) {
if (newVal) {
// we invoke that deregistration function, to disable the watch
deregisterWatchFn();
...
}
});
```
* Explain what is a $scope in AngularJS  
Scope is an object that refers to the application model. It is an execution context for expressions. Scopes are arranged in hierarchical structure which mimic the DOM structure of the application. Scopes can watch expressions and propagate events.  
https://docs.angularjs.org/guide/scope  

* What are Directives?  
Directives are markers on a DOM element (such as an attribute, element name, comment or CSS class) that tell AngularJS’s HTML compiler to attach a specified behavior to that DOM element (e.g. via event listeners), or even to transform the DOM element and its children.  
https://docs.angularjs.org/guide/directive  
* What is a singleton pattern and where we can find it in Angularjs?  
Is a great pattern that restricts the use of a class more than once. We can find singleton pattern in angular in dependency injection and in the services. If you do 2 times ‘new Object()‘ without this pattern, you will be allocating 2 pieces of memory for the same object. With singleton pattern, if the object exists, you reuse it.  
http://joelhooks.com/blog/2013/05/01/when-is-a-singleton-not-a-singleton/  

* What is an interceptor? What are common uses of it?  
An interceptor is a middleware code where all the $http requests go through. The interceptors are service factories that are registered with the $httpProvider by adding them to the $httpProvider.interceptorsarray.  You have 2 types of requests that go through the interceptor, request and response (and their errors respectively). This piece of code is very useful for error handling, authentication or middleware in all the requests/responses.  
https://docs.angularjs.org/api/ng/service/$http  

* How do you hide an HTML element via a button click in AngularJS?  
You can do this by using the ng-hide directive in conjunction with a controller.  

* How do you disable a button depending on a checkbox’s state?  
We can use the ng-disabled directive and bind its condition to the checkbox’s state.  

* How would you implement application-wide exception handling in your Angular app?  
Angular has a built-in error handler service called $exceptionHandler which can easily be overriden as seen below:  

```
angular.
  module('exceptionOverwrite', []).
  factory('$exceptionHandler', ['$log', 'logErrorsToBackend', function($log, logErrorsToBackend) {
    return function myExceptionHandler(exception, cause) {
      logErrorsToBackend(exception, cause);
      $log.warn(exception, cause);
    };
  }]);
```

This is very useful for sending errors to third party error logging services or helpdesk applications. Errors trapped inside of event callbacks are not propagated to this handler, but can manually be relayed to this handler by calling $exceptionHandler(e) from within a try catch block.  
https://docs.angularjs.org/api/ng/service/$exceptionHandler  

* On which types of component can we create a custom directive?  
AngularJS provides support to create custom directives for following type of elements (one or many):  
Element directives − Directive activates when a matching element is encountered.  
Attribute − Directive activates when a matching attribute is encountered.  
CSS − Directive activates when a matching css style is encountered.  
Comment − Directive activates when a matching comment is encountered.  
https://docs.angularjs.org/guide/directive  

* Is it a good or bad practice to use AngularJS together with jQuery?
Its rather bad. JQuery directly manipulates the DOM, and in Angular it is the model that drives the view and most of the times direct DOM manipulation is not required. Usually things that we want to accomplish using jQuery plugins can be done with Angular directives. One of the most important parts in Angular development is: you shouldn't manipulate the DOM from your controllers, ever. This is fine in jQuery, but in Angular, you should modify your model and let Angular render it. Angular has a templating mechanism built in which you should use to load HTML fragments. If you need to create HTML dynamically, you should do so in a directive. Everything else violates the "separation of concerns" principle.  
http://ng-learn.org/2014/01/Dom-Manipulations/  
http://stackoverflow.com/a/29505812  

* What is DDO (Directive Definition Object)?  
The directive definition object provides instructions to the compiler. Instructions provide a lot of informations about directive behaviour, eg. template to use (or template url to load), restric which restricts the directive to a specific directive declaration style, controller constructor function, controllerAs identifier name for a reference to the controller in the directive's scope and many more.  

https://docs.angularjs.org/api/ng/service/$compile#directive-definition-object 

* How would you programatically change or adapt the template of a directive before it is executed and transformed?  
I would use the compile function. The compile function gives us access to the directive’s template before transclusion occurs and templates are transformed, so changes can safely be made to DOM elements. This is very useful for cases where the DOM needs to be constructed based on runtime directive parameters.  
https://docs.angularjs.org/api/ng/service/$compile

* How would you validate a text input field for a twitter username, including the @ symbol?  
I would use the ngPattern directive to perform a regex match that matches Twitter usernames.
https://docs.angularjs.org/api/ng/directive/ngPattern  

* What is a digest cycle in AngularJS?  
The $digest cycle is a loop through all registered bindings chceking if some of them changed and rerendering any value changes. The digest process is kicked-in when any of the following occur as part of angular context: DOM Events (like ng-click etc.), Ajax with callbacks ($http etc.), Timers with callbacks ($timeout etc.), calling $apply, $digest, etc. It is important to note that the normal browser related DOM events (onclick etc.) and setTimeout would not trigger a digest process as they work out of "Angular Context".  
https://www.ng-book.com/p/The-Digest-Loop-and-apply/  
