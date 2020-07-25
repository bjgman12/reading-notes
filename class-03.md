# Lists 
[Home](README.md)

- `<ol>` ordered list
- `<ul>` unordered list
- `<li>` list items

- `<dl>` is a definition list used to list things and their definitions
- `<dt>` is the term to be defined
- `<dd>` is used for teh definition

- You can nest lists if it fits your design for the page

# Boxes

> all elements in a HTML document are placed in boxes , all of these boxed have a width and a height which can be defined by

- px Pixels
- % a percent of the veiw window
- em relative to the size of the text in the box

> % and ems are used to make boxes mutate as teh veiw window changes sizes though this mutation can be limited using 

- min-width/height
- max-width/height

> **overflow** can be used to handle the case when the contents of the box spill out of the defined space for the box this can be set to 

- hidden
- scroll

> **Border** elements work as you expect them to

> **padding** is used to allot space between an element and its broder

>**margin** controls the gap between boxes

> to **center** content set left and right margins to auto

> you can use box shadows to have boxed cast a shadow

>**border radius** can be used to morph boxed into eliptical shapes


## Decisions and Loops
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