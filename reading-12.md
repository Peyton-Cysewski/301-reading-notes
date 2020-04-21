# Reading Notes 12

## EJS Partials
Partials in EJS are the things that act as templates. Depending on the application, this can massively reduce the amount of code needed to be written. If a website has many pages that are different but use a similar structure, a template can be used to create the pages with minimal things having to be written more than once. Nav bars and footers are common things that are perfect examples of partials. To use partials, the following delimiter of ejs syntax is used: `<%- include('relative/file/path') %>`. That relative file path is usually a directory called 'views' that holds .ejs files that hold the specific bits of html to be inserted into the specified templates.



#### [Home](README.md)