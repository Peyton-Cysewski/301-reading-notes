# Reading Notes 13

## Sending Form Data
Data sent from an html is most likely done using the http or better yet, the https protocol. When a user enters data into a form, that information is packaged up in that protocol and sent somewhere else. The 'action' attribute of the form decides where that data is sent. This can be an absolute url (includes https://somewhere.com) or a relative path (/this/relative/path). Note, https data can be sent to a http site just fine, but an https site will not work and warn the user of a security risk when sent. The 'method' of a form determines how the data is sent. The most common methods are 'GET' and POST'. A 'GET' request appends data to the url itself while the 'POST' request sends data in the body of the request.

## Receiving Form Data
For us, the javascript express library handles all of the inner workings of processing the response. Almost every server language already has a library that has been developed for this purpose. These transactions can be handled manually, but using these libraries massively increases productivity and ease of use.

## Baseline Protection
Rule number one is to never trust your users. Three basic steps can be taken to be protective with html forms:
- Escape dangerous characters
- Limit the amount of incoming data
- sandbox uploaded files; store them somewhere else so a potenially harmful file can't do extra damage.



#### [Home](README.md)