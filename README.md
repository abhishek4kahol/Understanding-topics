# Understanding-topics

1. **[Understanding JavaScript and EcmaScript](#understanding-javascript-and-ecmascript)**
2. **[Server side and Client side rendering](#server-side-and-client-side-rendering])**

## Understanding JavaScript and EcmaScript

* Ecma International : An organization that creates standards for technologies.

### ECMA-262
1. This is a standard published by Ecma International.It contains the specification for a general purpose scripting language.
2. ECMA-262 is a standard that represents a scripting language specification called **ECMAScript**.
3. It is a specification for creating a general purpose scripting language.
4. ECMAScript provides the rules, details, and guidelines that a scripting language must observe to be considered ECMAScript compliant.

### JavaScript
1. A general purpose scripting language that conforms to the ECMAScript specification. It is a dialect of the ECMAScript language.
2. JavaScript is the coffee-flavored language and ECMAScript is the specification it’s based on.
3. By reading the [ECMAScript specification](https://www.ecma-international.org/publications/files/ECMA-ST/Ecma-262.pdf), you learn how to create a scripting language. By reading the [JavaScript documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript), you learn how to use a scripting language.

4. JavaScript mostly implements the ECMAScript specification as described in ECMA-262, but a handful of differences do exist. Mozilla outlines JavaScript’s non-ECMAScript language features [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript/ECMAScript_Next_support_in_Mozilla).

### Differences in browser support

* Even though the JavaScript engines of browsers all understand JavaScript, some browsers have a greater understanding of the language than others. There are differences in the way browsers support the language.

* If you will recall, ECMAScript is a specification for what a scripting language could look like. Releasing a new edition of ECMAScript does not mean that all JavaScript engines in existence suddenly have those new features. It is up to the groups or organizations who are responsible for JavaScript engines to be up-to-date about the latest ECMAScript specification, and to adopt its changes.

* If a new edition of ECMAScript comes out, JavaScript engines do not integrate the entire update at one go. They incorporate the new ECMAScript features incrementally



### ECMAScript 6

* It is the sixth edition of the ECMA-262 standard, and features major changes and improvements to the ECMAScript specification.
* This edition of ECMAScript changed its name from ES6 to ES2015 because in 2015 Ecma International decided to switch to annual releases of ECMAScript.

> whole info is taken from medium article link [here](https://medium.freecodecamp.org/whats-the-difference-between-javascript-and-ecmascript-cba48c73a2b5)

-------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------


## Server side and Client side rendering

### Server-side rendering
* Server-side rendering is the most common method for displaying information onto the screen. It works by converting HTML files in the server into usable information for the browser.
* Whenever you visit a website, your browser makes a request to the server that contains the contents of the website. The request usually only takes a few milliseconds, but that ultimately depends on a multitude of factors:
    1. Your internet speed
    2. the location of the server
    3. how many users are trying to access the site
    4. how optimized the website is, and more.
    
* Once the request is done processing, your browser gets back the fully rendered HTML and displays it on the screen. If you then decide to visit a different page on the website, your browser will once again make another request for the new information. This will occur each and every time you visit a page that your browser does not have a cached version of.

* It doesn’t matter if the new page only has a few items that are different than the current page, the browser will ask for the entire new page and will re-render everything from the ground up.

* On the bright side, server-side rendering is great for SEO. Your content is present before you get it, so search engines are able to index it and crawl it just fine. Something that is not so with client-side rendering. At least not simply.

#### Server-side pros:                                      
* Search engines can crawl the site for better SEO.
* The initial page load is faster.
* Great for static sites.

#### Server-side cons:
* Frequent server requests.
* An overall slow page rendering.
* Full page reloads.
* Non-rich site interactions.


### Client-side rendering
* When developers talk about client-side rendering, they’re talking about rendering content in the browser using JavaScript. So instead of getting all of the content from the HTML document itself, you are getting a bare-bones HTML document with a JavaScript file that will render the rest of the site using the browser.

* This is a relatively new approach to rendering websites, and it didn't really become popular until JavaScript libraries started incorporating it into their style of development. Some notable examples are Vue.js and React.js

* The key difference is that if you were to click on the link the page to load more content, the browser will not make another request to the server. You are rendering items with the browser, so it will instead use JavaScript to load the new content and Vue.js will make sure that only the new content is rendered. Everything else will be left alone.

* This is much faster since you are only loading a very small section of the page to fetch the new content, instead of loading the entire page.

* There are some trade offs with using client-side rendering, though. Since the content is not rendered until the page is loaded on the browser, SEO for the website will take a hit. There are ways to get around this, but it’s not as easy as it is with server-side rendering.

* Another thing to keep in mind is that your website/application won’t be able to load until ALL of the JavaScript is downloaded to the browser. Which makes sense, since it contains all the content that will be needed. If your users are using slow internet connection, it could make their initial loading time a bit long.

#### Client-side pros:
* Rich site interactions
* Fast website rendering after the initial load.
* Great for web applications.
* Robust selection of JavaScript libraries.

#### Client-side cons:
* Low SEO if not implemented correctly.
* Initial load might require more time.
* In most cases, requires an external library.

> whole info is taken from medium article link [here](https://medium.freecodecamp.org/what-exactly-is-client-side-rendering-and-hows-it-different-from-server-side-rendering-bd5c786b340d)


-------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------

