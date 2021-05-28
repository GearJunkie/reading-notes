# Programming with JavaScript

Control flow
 - The control flow is the order in which the computer executes         statements in a script. Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution. Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:
if (field==empty) {
    promptUser(“you need to fill this field”);
} else {
    submitForm();
}
The above excerpt might be inside a function that runs when the user clicks the Submit button for the form. The function could also include a loop, which iterates through all of the fields in the form, checking each one in turn. Looking back at the code in the if and else sections, the lines promptUser and submitForm could also be calls to other functions in the script. As you can see, control structures can dictate complex flows of processing even with only a few lines of code.

- JavaScript Functions
A JavaScript function is a block of code designed to perform a particular task. A JavaScript function is executed when "something" invokes it (calls it).

Example
function exampleOne() {
  return p1 * p2;   // The function returns the product of p1 and p2
}

- JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses (). Function names can contain letters, digits, underscores, and dollar signs (same rules as variables). The parentheses may include parameter names separated by commas: (parameter1, parameter2, ...). The code to be executed, by the function, is placed inside curly brackets: {}

function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

- Function parameters are listed inside the parentheses () in the function definition. Function arguments are the values received by the function when it is invoked. Inside the function, the arguments (the parameters) behave as local variables. A Function is much the same as a Procedure or a Subroutine, in other programming languages.

- Function Invocation
The code inside the function will execute when "something" invokes (calls) the function: When an event occurs (when a user clicks a button), When it is invoked (called) from JavaScript code, Automatically (self invoked)

- Function Return
When JavaScript reaches a return statement, the function will stop executing. If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement. Functions often compute a return value. The return value is "returned" back to the "caller":

Example

Calculate the product of two numbers, and return the result:
var x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
The result in x will be: 12

- Why Functions?
You can reuse code: Define the code once, and use it many times. You can use the same code many times with different arguments, to produce different results. The () Operator Invokes the Function. Accessing a function without () will return the function object instead of the function result.

- Functions Used as Variable Values
Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

- Local Variables
Variables declared within a JavaScript function, become LOCAL to the function. Local variables can only be accessed from within the function. Since local variables are only recognized inside their functions, variables with the same name can be used in different functions. Local variables are created when a function starts, and deleted when the function is completed.

Example

// code here can NOT use carName
function myFunction() {
  var carName = "Volvo";
  // code here CAN use carName
}
// code here can NOT use carName

- JavaScript Operators

Example
Assign values to variables and add them together:
var x = 5;         // assign the value 5 to x
var y = 2;         // assign the value 2 to y
var z = x + y;     // assign the value 7 to z (5 + 2)
The assignment operator (=) assigns a value to a variable.

Assignment
var x = 10;
The addition operator (+) adds numbers:

Adding
var x = 5;
var y = 2;
var z = x + y;
The multiplication operator (*) multiplies numbers.

Multiplying
var x = 5;
var y = 2;
var z = x * y;	
JavaScript Arithmetic Operators
Arithmetic operators are used to perform arithmetic on numbers:

Operator	Description
(+)	        Addition
(-)	        Subtraction
(*)	        Multiplication
**	        Exponentiation (ES2016)
/	        Division
%	        Modulus (Division Remainder)
++	        Increment
--	        Decrement

Assignment operators assign values to JavaScript variables.
Operator	Example	Same As
=	x = y	x = y
+=	x += y	x = x + y
-=	x -= y	x = x - y
*=	x *= y	x = x * y
/=	x /= y	x = x / y
%=	x %= y	x = x % y
**=	x **= y	x = x ** y
The addition assignment operator (+=) adds a value to a variable.

Assignment
var x = 10;
x += 5;

JavaScript String Operators
The + operator can also be used to add (concatenate) strings.

Example
var txt1 = "John";
var txt2 = "Doe";
var txt3 = txt1 + " " + txt2;
The result of txt3 will be: John Doe

The += assignment operator can also be used to add (concatenate) strings:

Example
var txt1 = "What a very ";
txt1 += "nice day";
The result of txt1 will be: What a very nice day

When used on strings, the + operator is called the concatenation operator.

Adding two numbers, will return the sum, but adding a number and a string will return a string:

Example
var x = 5 + 5;
var y = "5" + 5;
var z = "Hello" + 5;
The result of x, y, and z will be: 10, 55, "Hello5"


JavaScript Comparison Operators
Operator	Description
==	        equal to
===	        equal value and equal type
!=	        not equal
!==	        not equal value or not equal type
>	        greater than
<	        less than
>=	        greater than or equal to
<=	        less than or equal to
?	        ternary operator

JavaScript Logical Operators
Operator	Description
&&	        logical and
||	        logical or
!	        logical not

JavaScript Type Operators

Operator	Description
typeof	    Returns the type of a variable
instanceof	Returns true if an object is an instance of an object type
