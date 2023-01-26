---
title: HTML Questions
layout: layouts/page.njk
permalink: /questions/html-questions/index.html
---

* What does a `doctype` do?

My answer : it assert the document type of html to the browser

correct answer : tells the browser what version of HTML the document is written in.

:rage:

---

* How do you serve a page with content in multiple languages?

My answer : to give 'homepage/id' for Indonesian languages and 'homepage/en' for English language, there's basically 2 page for each language that user can toggle or just use library i believe there's one for that.

correct answer : [some answer, i don't find any thing useful. just use library man](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language)

ChatGPT: 

There are several ways to serve a page with content in multiple languages, including:

Using browser or device language settings: The browser or device can send an HTTP header indicating the preferred language, and the server can use that information to serve the appropriate version of the page.

Using subdomains or subdirectories: Each language can have its own subdomain (e.g. fr.example.com) or subdirectory (e.g. example.com/fr)

Using query parameters: A query parameter can be used to indicate the language (e.g. example.com?lang=fr)

Using cookies: The server can set a cookie indicating the preferred language, and use that information to serve the appropriate version of the page.

Implementing a language switcher: A language switcher can be added to the webpage, which allows users to select their preferred language.

It's also important to note that some languages have different scripts like right-to-left(RTL) and it's important to have a proper design to handle that.


---

* What kind of things must you be wary of when designing or developing for multilingual sites?

My answer : SEO, RTL language,  

correct answer : 

1. Character encoding: Different languages use different character sets, and it's important to ensure that the site uses the correct encoding for each language.

2. Text direction: Some languages, like Arabic and Hebrew, are written right-to-left (RTL) instead of left-to-right (LTR). This means that the layout of the site needs to be adjusted to accommodate RTL text and any elements that may be affected by the text direction.

3. Date and time formats: Different languages and cultures use different date and time formats, so it's important to ensure that the site uses the appropriate format for each language.

4. Number formats: Different languages and cultures use different number formats, so it's important to ensure that the site uses the appropriate format for each language.

5. Images and videos: Any images or videos on the site should be captioned or subtitled in all languages to ensure that they are accessible to all users.

6. Search engine optimization (SEO): Each language version of the site should have its own unique content, and it's important to use the correct hreflang tags and other SEO techniques to ensure that the site is properly indexed by search engines.

7. Accessibility: The site should be accessible to users with disabilities in all languages. This includes providing alternative text for images and videos, and providing text transcripts for audio content.

8. Translation: The quality of translation is important, and professional translators should be used to ensure that the content is accurate and appropriate for the target audience.

9. Testing: The site should be tested in all languages to ensure that it functions correctly and is accessible to all users.

---

* What are `data-` attributes good for?

my answer : its for make html hold value, I know the use case of like saving the scroll mouse value to HTML tag so I can animate it nicely.

data- attributes are used to store custom data private to the page or application, for which there are no more appropriate attributes or elements. These attributes are used to store data that is not meant to be seen or edited by the user, but is used by JavaScript or other scripts to perform specific actions on the page.

Here are a few examples of how data- attributes can be used:

Storing metadata: data- attributes can be used to store metadata about an element, such as the element's position in a list, or a unique identifier.

Tracking user interactions: data- attributes can be used to track user interactions with an element, such as whether a button has been clicked or a form has been submitted.

Enhancing accessibility: data- attributes can be used to provide additional information to assistive technology, such as providing a description of an image for users with visual impairments.

Storing state: data- attributes can be used to store state information, such as whether a button is disabled or whether a form field is required.

Enhancing performance: data- attributes can be used to speed up the rendering of complex pages by storing data that is used to update the page after it has loaded.

The data stored in data- attributes is not visible to the user and will not affect the presentation of the page, but it can be accessed and manipulated using JavaScript, CSS or other scripting languages.

---

* Consider HTML5 as an open web platform. What are the building blocks of HTML5?

my answer : tag

correct answer : 

1. Semantic elements: HTML5 introduces new semantic elements, such as <header>, <footer>, <article>, <section>, and <nav>, which provide more meaningful and accurate information about the structure and content of a web page.

2. Form controls: HTML5 provides new form controls, such as <search>, <tel>, <email>, <url>, and <date>, which can be used to create more interactive and user-friendly forms.

3. Canvas: The <canvas> element is a new feature in HTML5 that allows developers to create and manipulate graphics and animations in a web page, using JavaScript.

4. Audio and Video: HTML5 introduces new elements <audio> and <video> that can be used to embed multimedia content directly into a web page, without the need for additional plug-ins.

5. Local storage: HTML5 provides new storage options, such as local storage, which allows web applications to store data on the client-side, and make it available even when the user is offline.

6. WebSockets: HTML5 introduced WebSockets, a new protocol for real-time communication between the client and the server.

7. Microdata: HTML5 provides a way to embed structured data in web pages, using the itemscope and itemprop attributes, which can be used to help search engines and other applications understand the content of a web page.

8. Geolocation: HTML5 introduced an API which allows the user's device to share their location with the browser, which allows web pages to provide location-aware features and services.

9. Web workers: HTML5 introduced the concept of web workers, which allow long-running scripts to run in the background, without blocking the user interface.

10. Drag and drop: HTML5 introduced the drag-and-drop API, which allows users to drag elements from one place to another on a web page, and allows web developers to create more interactive and user-friendly interfaces.

---

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.

my answer :

cookie : when user visit the webpage it saves the users behavior and we can use it later to make the web performance faster because it doesn't has to re render everything

sessionStorage : idk

localStorage : save data on client side

correct answer : 

Cookies: Cookies are small text files that are stored on the user's computer by the web browser. They are sent back to the server with every request, which allows the server to maintain state between requests. Cookies have a size limit of 4KB and can also have an expiration date, which determines how long they will be stored on the user's computer.

sessionStorage: sessionStorage is an HTML5 feature that allows web developers to store data on the client-side, but unlike cookies, the data is only stored for the duration of the current browser session. This means that when the user closes the browser, the data stored in sessionStorage is deleted. sessionStorage objects are specific to the origin of the web page and the browser tab.

localStorage: localStorage is similar to sessionStorage, but the data stored in localStorage is not deleted when the browser is closed. The data will persist until it is explicitly deleted by the web application or the user. The data stored in localStorage is also specific to the origin of the web page, and it has a larger storage limit than cookies, usually around 5MB.

In summary, cookies are mainly used for maintaining state between requests, sessionStorage is mainly used for temporary data that needs to persist across a single browser session and localStorage is mainly used for persistent data that needs to persist across multiple browser sessions.

---

* Describe the difference between `<script>`, `<script async>` and `<script defer>`.

my asnwer : 

adding script to the html and with added attribute will result in vary ways of how the script run

script : will load cascadingly

script async : will run asynchronously with other file

script defer : will run last after everything else done

correct answer : 

The script element is used to include a script within an HTML or XHTML document.

The async attribute tells the browser to download the script in the background and execute it as soon as it's finished downloading. This allows the rest of the page to continue to load while the script is downloading, which can improve the overall performance of the page. However, the script will execute as soon as it finishes downloading, regardless of where it is located in the HTML.

The defer attribute tells the browser to download the script in the background and execute it only after the page has finished parsing. This can also improve the performance of the page, and it ensures that the script will execute in the order in which it appears in the HTML.

In short, async allows the script to be downloaded and executed as soon as it is available, while defer waits until the page has finished parsing before executing the script.

---

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

my answer : 

for css style link so it will executed immediatly 

fot script so it will be executed after the body of page finished parsing

correct answer :

It is generally a good idea to position CSS <link>s between <head></head> and JS scripts just before </body> because it allows the browser to load and apply the CSS first, ensuring that the page is rendered correctly and consistently before any JavaScript is executed. This can improve the perceived performance of the page, as the user can start interacting with the page sooner.

One exception to this might be if a script is required to make the page usable, such as a script that sets up the layout or makes the navigation functional. In this case, it may be necessary to include the script higher up in the page to make sure that the page is usable as soon as possible.

Another exception is if you are using the async or defer attributes for script loading, as that can change the loading and execution order of the scripts regardless of where they are placed in the DOM.

---

* What is progressive rendering?  *it's literally lazy loading*

my answer : tbh idk but i'll try, it's the protocol about how the page rendered from downloading, executing and displayed for user.

correct answer : 

Progressive rendering is a technique used to improve the perceived performance of a website by gradually displaying content to the user as it becomes available, rather than waiting for all content to be fully loaded before displaying anything.

With progressive rendering, the browser can start rendering the page as soon as the HTML document is received, even if some resources such as images and scripts have not yet been fully loaded. This allows the user to start interacting with the page sooner, and can improve the overall user experience.

There are several ways to achieve progressive rendering, such as using lazy-loading to only load images as they come into view, or using a technique called "time-to-first-paint" to measure and improve the time it takes for the browser to start rendering the page.

Progressive rendering is a best practice, and it's commonly used by many websites, especially on mobile devices where the network may be slower.

---

* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.

my answer : idk what's a srcset.

correct answer : 

The srcset attribute is used in an img tag to provide a list of different image files for the browser to choose from, based on the device's screen resolution and available network bandwidth. The browser can then select the most appropriate image for the current device and network conditions, rather than always loading the same image file.

When the browser encounters an img tag with a srcset attribute, it evaluates the content of the attribute to determine the best image to load. The srcset attribute should contain a list of image URLs, each followed by a comma and a descriptor indicating the size and density of the image. The browser will use the descriptor to determine the best image to use, based on the device's screen resolution and available network bandwidth.


* Have you used different HTML templating languages before?

my answer : no, i only use vanilla or react. i encounter some like pug on codepen

open answer :

Mustache: A simple, logic-less template language that can be used with a variety of programming languages.

Handlebars: An extension of Mustache that adds support for more advanced features such as block expressions and helper functions.

Jade: A high-performance template engine for Node.js that uses a simplified syntax for generating HTML.

EJS: A simple templating language for JavaScript that is similar to ERB templates in Ruby on Rails.

Twig: A flexible, fast, and secure template engine for PHP.

Blade: A simple and elegant templating engine for PHP which is provided by Laravel framework.

Jinja: A modern and designer-friendly templating language for Python, modelled after Django templates.

Smarty: A popular templating engine for PHP that is widely used in content management systems and e-commerce platforms.

---

* What is the difference between `canvas` and `svg`?

my answer : canvas for 3d, svg for 2d

correct answer :

Canvas and SVG are both technologies used to create graphics and visualizations in web pages, but they have some key differences in terms of how they work and the types of graphics they are best suited for.

The canvas element is an HTML element that creates a fixed-size drawing surface on a web page. It allows you to draw shapes, lines, and images using JavaScript, and it also provides a number of built-in tools for manipulating the graphics, such as rotating, scaling, and compositing. Canvas is best used for creating graphics that need to be updated frequently, such as animations and games.

The svg element, on the other hand, is an XML-based vector image format that is used to create graphics that can be scalable and maintain their quality when resized. SVG graphics are defined using a set of instructions, rather than pixels, which means that they can be resized without losing quality. SVG graphics are best used for creating logos, icons, charts, and other types of graphics that need to be scalable, and also can be animated.

In summary, Canvas is best for dynamic, interactive graphics and animations, while SVG is best for vector-based graphics that need to be scalable and maintain their quality when resized.

---

* What are empty elements in HTML ?

my asnwer : element that doesnt has a content?

correct answer :

In HTML, an empty element is an element that does not have a closing tag. Empty elements are also known as self-closing or void elements. These elements are used to create elements that don't have any content, but may still have attributes. Empty elements are represented by a single tag, with a forward slash before the closing angle bracket.

An example of an empty element is the br element, which is used to create a line break in the text. The <br> element doesn't have any content, so it doesn't require a closing tag.

Here is a list of some common empty elements in HTML:

br: Creates a line break in text

hr: Creates a horizontal rule (a line)

img Displays an image

input: Creates an input field for user input

link: Links to an external resource

meta: Provides metadata about the HTML document

param: Defines parameters for an object element

source: Specifies the source of a media element (audio or video)
It's worth noting that some of these elements are not empty in XML, because they need a closing tag.

Empty elements are a important part of HTML and they are used to create simple and lightweight HTML documents, but they should be used with care to make sure that the elements are used correctly and that the HTML is semantically correct.
