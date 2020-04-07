# Reading Notes 02

## jQuery Intro

jQuery is a versatile part of JavaScript that allows code to be written cleanly and succinctly. The first thing it is good at is finding elements using CSS-style selectors. For example `$('li.hot')` would find all `<li>` elements with the class of 'hot'. These are in essence performing the same functionality as traditional DOM queries, but the syntax is much simpler and shorter to write. There is also a vast library of methods that can be used to manipulate or change CSS-style selectors. Continuing with the sentiment, these are very simple. Adding classes to items, animations, and clicking events can often be handled in short one-liners.

Note: Javascript can be used to do all the same tasks, but it is easier to write, thus saving time in both creation and ease use/readability.

## Specific Notes on jQuery

- Selecting Elements - `$('ul')` may return a single element in its object, but it can also return multiple items in its object.
- Get and Set Methods - `var content = $('li').html()` would return all of content of the first item of a list, but `var content = $('li').html('Example Text')` would update all of the list items with the string 'Example Text'.
- jQuery objects do not store the actual DOM elements, instead they store references to them.
- Caching jQuery objects is when a reference is stored in a variable.
- Looping - selector functions inherently loop through all of the items they can select.
- Chaining - using the dot notation, multiple methods can be applied to selector by chaining them one after the other.
- Checking the Page - `$(document).ready(function() { // Code Block });` will wait until the page is fully loaded before running any javascript. `$(function() { // Code Block });` is a shorthand way of writing the same thing.
- Changing Elements - `.html()`, `.text()`, `.replaceWith()`, and `.remove()` are the ways of directly getting at the content on a page.
- Inserting Elements - `.before()`, `.after()`, `.prepend()`, `.append()`, `.prependToO()`. and `.appendto()` all are ways of inserting elements to a page.
- Attributes - `.attr()`, `.removeAtrr()`, `.addClass()`, and `.removeClass()` are used with obtaining or changing attributes and their values of elements.
- CSS Properties - `.css('property', 'value')` is how specific CSS styles can be changed or obtained. Many can be changed in one method by putting all of the property-value pairs in `{}` brackets.
- Each Method - `.each()` allows one or more statements to be performed on each of the items of a selection. `$(this)` creates a jQuery object that refers to itself in the loop.
- Event Methods - `.on()` is what handles ALL events. The type of event that is listened for is specified and then a function is ran.
- Event Objects - all events form objects which contain useful information regarding the event. The list of properties is long and in-depth, which makes these objects very versatile. The 'on' method contains the properties: `events`, `[, selector]`, `[, data]`, and `function(e)` where 'selector' refers to which subset of elements of which the event will respond to and 'data' where extra data is passed in to the function when the event is triggered.

## Including jQuery on a Page

jQuert can be hosted by another company, however, a fallback option should always be included. jQuery can be loaded from a CDN. A source property of a script tag is url, but the address starts with two forward slashes `//` to signify that this is a relative URL so that it will used the https protocal that the main page is using.
Note: Having the script tag at the top of the page like in the head can cause the page to loader slower, so it is now the bset practice to put it at the bottom of the page as the very last thing inside the closing body tag.



#### [Home](README.md)