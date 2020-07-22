# Cascading Style Sheets - Notes

- RGB
  - expresses color based on how much red green and blue is present in color 
  - ` rgb(100,100,100)`
- HSL
  - Assigning colors by Hue Saturation and Lightness
  - Hugh is assigned between 0 and 360 degrees
  - Saturation is assigned by percentage
  - Lightness is also expressed as a percentage 0 being white and 100 being black
- Hex codes
 - hex codes express color by their assigned hexidecimal value
 - `#00ff00` green
- Layout

## Anatomy

- Rule - 

- background color assigns a color to the background of the box it is set to.

> be sure to have a decent amount of contrast between your background color and text color

![CSS syntax example](sel.gif) 

### Selectors

- `*{}` is a universal selctor
- type selectors match element names
- class selectors matches an element whos class matches 
  - `.note` will select all emementsof class `.note`
  - `p.note` will select only paragraph of class `.note`
- id selectorws only select element with corresponding ID
  - `#id `
- child selector will select element that are children of specified element
  - `li>a{}`

- Decendant selector matches an element that is a decendant 
  - ` p a {} `
- Adacent sibling selector will target the next sibling
  - ` h1+p {} `
- General sibling collector
  - ` h1~p `


  - conditionals
  - if
  - else
- operators ( + - = *)
- data types
  - string
  - boolean
  - number
- variable` var` `x = 42`, `UserName = Brandon`

## Objects and methods

- the document object represents the entire page
- write() method allows new conent wherever the `<Script>` element sits
- parameters go inside methods

<img src ="js example.jpg">

- java script will run where it is found in the html
- comment are done like C++ with a `//`
- store variable into strings bye using  ' string here'

``` 
var today = new Date();
var hourNow = today.getHours();
var greeting;


if (hourNow > 18) {
    greeting = 'Good Evening G!';
} else if ( hourNow > 12){
    greeting = 'Good Afternoon Playa!';
} else if (hourNow > 0){
    greeting = ' Good Morning Sunshine!';
} else {
    gretting = ' Welcome Sir ...';
}

document.write('<h3>'+ greeting + '</h3>')
```

## Loops adn decisions.



# Operators and Loops Notes
## Comparison Operators Evaluating Conditions
- Is Equal to (==)
    - compares two values to see if they're the same
- Is Not Equal to (!=)
    - Compares two values to see if they are not the same.
- Strict Equal to (===)
    - Compares two values to check that both the data type and value are the same.
- Strict Not Equal to (!==)
    - Compares two values to check that both the data type and value are not the same.
- Greater Than (<)
    - Checks number on the left is greater than the number on the right.
- Less Than (<)
    - Checks if number on the left is less than number on the right.
- Greater Than or Equal to (>=)
    - Checks number on the left is greater than or equal to the number on the right.
- Less Than or Equal to (<=)
    - Checks number on left is less than or eual to  the number on the right
## Comparison Operator Anatomy
(score >= pass)
- "score" = operand
- "pass" = operand
- ">=" = comparison operator
- "()" = enclosing brackets

## Logical Operators
- && = logical and
    - tests more than one condition
    - ((2<5) && (3>=2)) returns true
- || = logical or
    - tests at least one condition
    - ((2<5) || (2>1)) returns true
- ! = logical not
    - operator takes a single Boolean value and inverts it.
    - !(2<1) returns true
<br>

((5 < 2) && (2 >= 3))
- (5<2) = expression 1
- (2 >= 3) = expression 2
- && = logical operator
- ((5 < 2) && (2 >= 3)) = expression 3

## Loops
> Loops check a condition. If it returns true, a code block will run. The condition will be checked again and if still true, the code block will run again. It repeats until the condition returns false.
### Common Types of Loops
- For
    - Runs code specific amount of times. The condition is usually a counter which is used to tell how many times the loop should run.
- While
    - Don't know how many times loop should run. Condition doesnt have to be a counter, and code will continue to loop for as long as the condition is true.
- Do While
    - Similar to while loop but it will always run the statements in curly braces at least once, even if condition is false.

<pre>
for (var i = 0; i < 10; i++) {
    document.write(i);
}
</pre>

- "for" = keyword
- "{}" = curly bracket
- "document.write(i);" = code to execute during loop
- "for (var i = 0; i < 10; i++) = condition(counter)

## Loop Counters
> A "for" loop uses a counter as a condition. This tells the code to run a specified amount of times. Below you'll see the condition is made up of three statements:
- Initialization
    - var i = 0;
    - Create a variable and set it to 0. This variable is called i, and acts as the counter.
- Condition
    - i < 10
    - The will run until it hits a specified number.
- Update
    - i++
    - Every time the loop runs the content in the curly brackets it adds one to the counter.

## While Loops
<pre>

- var i = 1;     //Set counter to 1
- var msg = '';  //Message
// Store 5x table in a variable
while (i < 10) {
    msg += i + ' x 5 = ' + (i * 5) + '<br>';
    i++;
}
document.getElementById('answer').innerHTML = msg;