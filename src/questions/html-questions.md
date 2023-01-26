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
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
* What is progressive rendering?
* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
* Have you used different HTML templating languages before?
* What is the difference between `canvas` and `svg`?
* What are empty elements in HTML ?
