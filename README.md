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

##React.DOM.(htmlTagName)
These elements are used in the form React.DOM.h1(attrObject, child) where ```attrObject``` is an element which contains the desired element attributes in a key/value form (or ```null``` if not needed) and ```child``` is the content that will enclosed in the tag. 

```child``` can be simple, such as plaintext, or another React.DOM element:
```
ReactDOM.render(
  React.DOM.h1({id:"myTitle"}, 
     React.DOM.span(null, "A span within an h1")
     )//end h1
   )//end render
```
###Special cases
The are a few restrictions in place for the ```attrObject```
- *class* and *for* cannot be used. Use *className* and *htmlFor* instead
- *style* doesn't take a string, it takes a js object instead.
```
React.DOM.p({className:"my-outline logo", style{text-align:"center", font-weight:"300"}}, "My Title");
```
