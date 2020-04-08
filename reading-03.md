# Reading Notes 03

## Mustache Templating

Mustache is a logic-less template syntax. This is a logic-less syntax because there are logical statements; only tags are used. These tags will have either a single vallue, series of values, or nothing. `mustache.js` is an implementation of this template system in JavaScript.
Note: Mustache is not a templating engine, but a specification for a templating engine.
- Example from reading: `Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” }); // returns: Hello, Sherlynn`


## Flexbox

The Flexbox display has a whole new set of properties. It's function is based around the flex container and the flex items. The flex container has a 'main size' across the horizontal 'main axis' and a 'cross size' across the vertical 'cross axis'.

### Parent Properties - The Flex Container

- `display: flex` - defines a flex container and enables flex content to all its its children.
- `flex-direction: row | row-reverse | column | column-reverse;` - determines the direction in which the children are placed.
- `flex-wrap: nowrap | wrap | wrap-reverse;` - determines how the children items will be wrapped from one line to another.
- `flex-flow: <‘flex-direction’> || <‘flex-wrap’>` - a shorthand combo property for the two prior properties.
- `justify-content:` - determines the alignment on the main axis and helps deal with leftover space between items horizontally. Its values are: `justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;`.
Note: Some browsers may not support a couple of these property values.
- `align-items:` - determines the alignments on the cross axis. It is very similar to the previous property with its functionality and values: `align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;`.
Note: Some browsers may not support a couple of these property values.
- `align-content:` - determines the alignment on the cross axis and helps deal with leftover space between items vertically. Its values are: ` align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;`.
Note: Some browsers may not support a couple of these property values.

### Child Properties

- `order: <integer>;` - defines the order in which the items appear in a flex container. The default value is 0 and the items should normally appear in the order that they are in on the html unless otherwise specified.
- `flex-grow: <number>;` - allows a flex item to grow (if necessary) to a specifed number that corresponds to a proportion to other items and will take up the appropriate amount of space.
- `flex-shrink: <number>;` - works like `flex-grow` but allows for items to shrink, if necessary.
- `flex-basis: <length> | auto;` - sets a default size of an element before the remaining space is distributed. Takes any length measurements.
- `flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]` - shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`. It is recommended to use this shorthand method instead of all of them individually.
- `align-self:` - allows for the alignment of an item to be individually overridden. Its values are: `align-self: auto | flex-start | flex-end | center | baseline | stretch;`.
Note: `float`, `clear`, and `vertical-align` have no effect here if tried.



#### [Home](README.md)