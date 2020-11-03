# Jquery and Pair programming

-$() is a shorthand for writing Jquery()

>Jquery can be use to select  elements of the dom and has many method of manipulating the forementioned

## Selectors

- `*` all elements
- `element` all elements with specified name
- `#id` elements that specified id
- `.class` will select element with specified class
- `selector1, selector2`  seperation  with a comma allows you to use multiple selectors

## Heirarchy

- standars css heirarchy works * > ~ +
 

 ## filters

 >what you are selecting can be filtered here are some examples

 - :not(selector)
 - :first
 - :last
 - etc

 >you can also filter throught the contents of html elements

 - :contains('whatever')
 - :empty 
 - etc


>you can check the document for if tis ready  using `$(document).ready(function())

## inserting elements

- `.before()` will insert the element before waht was selectet while `.prepend()' puts it right after the parent elements opening tag


>you can also include jquery through a cdn  using a script tag