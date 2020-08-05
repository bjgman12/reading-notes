[Home](README.md)

## object literals 


> **Objects**
- group together variables and they become properties of that object
- instead of variable objects have named key with a data type as a value
- object are access the same way as in c++ with dot notation


## document object model DOM

> when a browser loads a page it created a model of the page stored in the browsers memory called a **DOM** tree

- **Four node types**
  - document node  over arching term for all nodes
  - element nodes describe structture of html page
  - attribute nodes carry attributes of elements
  - text nodes can be access once you have acessed an element node

## Working with the DOM tree

- `getElementbyId()`  uses the value of an elements ID attribute tp select
- `getElementByClassName()` select all elements by their class
- `getElementByTagName()` selects  all elements that have specific tag name


- `nodeValue()` lets you access contents of text node.
- `innerHTML`  gets the nodes html including any markup


> you can created new elements with `createElement()` along with `createTextNode()`

