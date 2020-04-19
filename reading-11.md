# Reading Notes 11

## EJS

EJS or Embedded Javascript allows html to be written concurrently with javascript. It looks a bit odd and functions similarly to a template. After installing ejs with npm, a .ejs file can be created. The primary syntax for its features is when things are wrapped in `<% %>`. It functions and looks like a normal html file, but js aspects like conditionals can exist intermingled within the ejs file as long as they are wrapped in the according syntax. When `=` is placed in the middle it means that it is evaluating to something and any js syntax can be used within it.

A related library called `express-ejs-layouts` allows express to use ejs in a way that functions as a layout similarly to how mustache or handlebars would. And index.ejs file serves as the building block for how templates would be used. This allows for text to be `re-used` across different pages without needing to copy already-existing code.



#### [Home](README.md)