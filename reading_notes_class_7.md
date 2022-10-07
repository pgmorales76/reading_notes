[Home](https://pgmorales76.github.io/reading_notes/)

# Class 7 Reading Notes

## Control Flow

### - The control flow is the order in which the computer executes statements in a script

### - Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops

### - For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or `if...else`, so that different code executes depending on whether the form is complete or not

    if (isEmpty(field)) {
        promptUser();
    } else {
        submitForm();
    }

### - The above excerpt might be inside a function that runs when the user clicks the Submit button for the form

### - Control flow means that when you read a script, you must not only read from start to finish, but also look at program structure and how it affects order of execution

[MDN Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)

## JavaScript Functions

### - A JavaScript function is a block of code designed to perform a particular task

### - A JavaScript function is executed when "something" invokes it (calls it)

    // Function to compute the product of p1 and p2
    function myFunction(p1, p2) {
        return p1 * p2;
    }

### JavaScript Function Syntax

#### - A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**

#### - Function names can contain letters, digits, underscores, and dollar signs (same rules as variables)

#### - The parentheses may include parameter names separated by commas: **(parameter1, parameter2, ...)**

#### - The code to be executed, by the function, is placed inside curly brackets: **{}**

    function name(parameter1, parameter2, parameter3) {
        // code to be executed
    }

#### - Function **parameters** are listed inside the parentheses () in the function definition

#### - Function **arguments** are the **values** received by the function when it is invoked

#### - Inside the function, the arguments (the parameters) behave as local variables

### Function Invocation

#### - The code inside the function will execute when "something" **invokes** (calls) the function

#### - When an event occurs (when a user clicks a button)

#### - When it is invoked (called) from JavaScript code

#### - Automatically (self invoked)

### Function Return

#### - When JavaScript reaches a `return` statement, the function will stop executing

#### - If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement

#### - Functions often compute a **return value**. The return value is "returned" back to the "caller"

    let x = myFunction(4, 3);   // Function is called, return value will end up in x

    function myFunction(a, b) {
        return a * b;             // Function returns the product of a and b
    }

### Why Functions?

#### - You can reuse code: Define the code once, and use it many times

#### - You can use the same code many times with different arguments, to produce different results

### The () Operator Invokes the Function

#### - `toCelsius` refers to the function object, and `toCelsius()` refers to the function result

#### - Accessing a function without () will return the function object instead of the function result

### Functions Used as Variable Values

#### - Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations

#### - Instead of using a variable to store the return value of a function

    let x = toCelsius(77);
    let text = "The temperature is " + x + " Celsius";

#### - You can use the function directly, as a variable value

    let text = "The temperature is " + toCelsius(77) + " Celsius";

### Local Variables

#### - Variables declared within a JavaScript function, become **LOCAL** to the function

#### - Local variables can only be accessed from within the function

    // code here can NOT use carName

    function myFunction() {
        let carName = "Volvo";
      // code here CAN use carName
    }

    // code here can NOT use carName

#### - Since local variables are only recognized inside their functions, variables with the same name can be used in different functions

#### - Local variables are created when a function starts, and deleted when the function is completed

[JavaScript Functions](https://www.w3schools.com/js/js_functions.asp)

## JavaScript Operators

### Types of JavaScript Operators

#### - There are different types of JavaScript operators

#### - Aritmetic Operators

#### - Assignment Operators

#### - Comparison Operators

#### - Logical Operators

#### - Conditional Operators

#### - Type Operators

### Assignment

#### - The assignment operator (`=`) assigns a value to a variable

    let x = 10;

### Adding

#### - The addition operator (`+`) adds numbers

    let x = 5;
    let y = 2;
    let z = x + y;

### Multiplying

#### - The multiplication operator (`*`) multiplies numbers

    let x = 5;
    let y = 2;
    let z = x * y;

[JavaScript Operators](https://www.w3schools.com/js/js_operators.asp)

[Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

[MDN Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
