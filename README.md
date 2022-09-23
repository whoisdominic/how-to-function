# Functions in javascript
## Objective: Define and call functions in JS

### Pre requisetes
Javascript variables, loops, comparison operators

### Eniornment setup
Node 12+, Vscode

Alternative: repl.it, codesandbox

### What is a function?
A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

```javascript
function myFirstFunction() {
	console.log("Wow! I did something?")
}
myFirstFunction()
```
A JavaScript function is defined with the  `function`  keyword, followed by a  **name**, followed by parentheses  **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:  
**(_parameter1, parameter2, ..._)**

The code to be executed, by the function, is placed inside curly brackets:  **{}**

#### Arguements
```javascript
function mySecondFunction(name, age) {
	console.log("My name is ", name, " and I am ", age , " years old")
}
mySecondFunction()
```

#### Return statements

When JavaScript reaches a  `return`  statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a  **return value**. The return value is "returned" back to the "caller":

**Example 1:**
```javascript
function anotherFunction(x) {
	var cheese = "gouda"
	console.log(cheese)
	return x * x 
	console.log(cheese)
}
anotherFunction()
```
**Example 2:**
```javascript
function canWeGoSurfing(weather) {
	if (weather === "cloudy" || weather === "monsoon") {
		return false
	}
	if (weather === "thunderstorm") {
		return false
	}
	if (weather === "sunny") {
		return true
	}
	return false 
}
canWeGoSurfing()
```
#### Functions as variables

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

```javascript
let activityOption = canWeGoSurfing("cloudy")
```

### Exercise

 1. Define a function called "sayHello" that takes one arguement called "name" and prints a greeting to the console. If the name arguement is equal to your name, then customize the greeting.
 2. Define a function that takes in an array of numbers, log all of the numbers to the console
 3. Define a function called "canVote" that takes one arguement called "age". If age is greater than 18 return true. Otherwise return false
 4. How would you assign your  "canVote" function to a variable?

