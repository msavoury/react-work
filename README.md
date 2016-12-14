# react-work
Jumping on the React Hype Train

Using react in the browser requires the inclusion of 2 files:
- react.js
- react-dom.js

Simplest react code: (Will place an h1 inside of an element of id "app1")
```
 ReactDOM.render(
            React.DOM.h1(null, "Hello world!"),
            document.getElementById("app1")
        );
```
###ReactDOM
This file will render the file in the browser
###React.DOM
A collection of ready made elements to be used such as ```React.DOM.span```

##React.DOM.<whatever>
These elements are used in the form React.DOM.h1(attrObject, text) where ```attrObject``` is an element which contains the desired element attributes in a key/value form and ```text``` is the text that will enclosed in the tag.
