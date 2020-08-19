# Chapter 10 Error handling and debugging


## Order of Execution

>knowing the order of how your js app executes is important in finding errors and debuging problems

- **Execution Contexts** correspong to variable scopes there is a global one and one for each function
 - global context  is code in the script but not in a function
 - function context is what it sounds like

 -

 ## The Stack

 > The js interpreter processes one line of code at a time and if the statement needs data from a function it pushes that function to the top of the stack

 ## Hoisting
 > each time a script enters a new execution context there are two phases

 - Prepare
   - scope is created variables functions andarements are created as well

 - Execute
   - assugns values to variables
   - reference functions and run their code
   - execute statements

## lexical scope

> if variables arent found in the local scope of code it can look to parent scopes but is resource intensive

## Error Objects
 > when creating an error object it should include 

  - name
  - message
  - fileNumber
  - lineNumber

### Types of errors

- syntax
- refference
- type
- range
- uri
- eval

