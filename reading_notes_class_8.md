[Home](https://pgmorales76.github.io/reading_notes/)

# Class 8 Reading Notes

## Expressions and Operators

### An expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely *evaluate*

### Assignment Operators

#### - An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (`=`), which assigns the value of its right operand to its left operand. That is, `x = f()` is an assignment expression that assigns the value of `f()` to `x`

### Assigning to properties

#### - If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression

    const obj = {};

    obj.x = 3;
    console.log(obj.x); // Prints 3.
    console.log(obj); // Prints { x: 3 }.

    const key = "y";
    obj[key] = 5;
    console.log(obj[key]); // Prints 5.
    console.log(obj); // Prints { x: 3, y: 5 }.

#### Assignment  x = f() x = f()

#### Addition assignment x += f() x = x + f()

#### Subtraction assignment x -= f() x = x - f()

#### Multiplication assignment x *= f() x = x* f()

#### Division assignment x /= f() x = x / f()

#### Remainder assignment x %= f() x = x % f()

### Avoid Assignmen Chains

#### - Chaining assignments or nesting assignments in other expressions can result in surprising behavior

#### - In particular, putting a variable chain in a `const`, `let`, or `var` statement often does *not* work. Only the outermost/leftmost variable would get declared; other variables within the assignment chain are *not* declared by the `const`/`let`/`var` statement. For example

    const z = y = x = f();

#### - This statement seemingly declares the variables `x`, `y`, and `z`. However, it only actually declares the variable `z`. `y` and `x` are either invalid references to nonexistent variables (in strict mode) or, worse, would implicitly create global variables for `x` and `y` in sloppy mode

## Comparison Operators

### A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values

#### Equal (`==`) Returns true if the operands are equal

#### Not equal (`!=`) Returns true if the operands are not equal

#### Strict equal (`===`) Returns true if the operands are equal and of the same type

#### Strict not equal (`!==`) Returns true if the operands are of the same type but not equal, or are of different type

#### Greater than (`>`) Returns true if the left operand is greater than the right operand

#### Greater than or equal (`>=`) Returns true if the left operand is greater than or equal to the right operand

#### Less than (`<`) Returns true if the left operand is less than the right operand

#### Less than or equal (`<=`) Returns true if the left operand is less than or equal to the right operand

[Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

## Loops and Iteration

### Loops offer a quick and easy way to do something repeatedly

### You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop

    for (let step = 0; step < 5; step++) {
        // Runs 5 times, with values of step 0 through 4.
        console.log('Walking east one step');
    }

### There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!)

### for statement

#### - A `for` loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop

#### - A `for` statement looks as follows

    for ([initialExpression]; [conditionExpression]; [incrementExpression])
        statement

#### - When a for loop executes, the following occurs

#### 1. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables

#### 2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)

#### 3. The statement executes. To execute multiple statements, use a block statement ({ }) to group those statements

#### 4. If present, the update expression incrementExpression is executed

#### 5.Control returns to Step 2

### while statement

#### - A `while` statement executes its statements as long as a specified condition evaluates to true. A `while` statement looks as follows

    while (condition)
      statement

#### - If the `condition` becomes `false`, `statement` within the loop stops executing and control passes to the statement following the loop

#### - The condition test occurs *before* `statement` in the loop is executed. If the condition returns `true`, `statement` is executed and the `condition` is tested again. If the condition returns `false`, execution stops, and control is passed to the statement following `while`

#### - To execute multiple statements, use a block statement (`{ }`) to group those statements

#### - The following while loop iterates as long as n is less than 3

    let n = 0;
    let x = 0;
    while (n < 3) {
    n++;
    x += n;
    }

#### With each iteration, the loop increments n and adds that value to x. Therefore, x and n take on the following values

#### - After the first pass: n = 1 and x = 1

#### = After the second pass: n = 2 and x = 3

#### - After the third pass: n = 3 and x = 6

#### = After completing the third pass, the condition n < 3 is no longer true, so the loop terminates

#### - Avoid infinite loops. Make sure the condition in a loop eventually becomes `false`—otherwise, the loop will never terminate! The statements in the following `while` loop execute forever because the condition never becomes `false`

    // Infinite loops are bad!
    while (true) {
    console.log('Hello, world!');
    }

[Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
