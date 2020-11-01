# Javascript

## DAY 16 OF PROGRAMMING 11/2/20

---

# Javascript

---

### Things we worked on:

---

1.
2.
3.

### Data Types

---

-   String - "Hello World"
-   Number - 42
-   Boolean - True
-   Date - new Date(10, 21, 2015)
-   Null - null
-   Array - [1,2,3]
-   Object - { name: "Sarah" }
-   Function - function greetUser(){}

### Concatenating Strings

---

```
Using the '+' operator

console.log("Hello" + " world"); // logs "Hello world"

```

```
Using the  \$\{\} syntax.

var name = "Harry";
console.log(`Hello ${name}`); // logs "Hello Harry"

```

### Variables

---

Basic variables are declared using the var keyword. You can declare variables and set variables using the = symbol. This can be done in one line or a variable that is declared can be set and even overwritten again at any point.

```
var favoriteColor; // declaration
favoriteColor = "Blue"; // assignment
var age = 30; // shorthand for declaration and assignment

```

```
What about "let" and "const"?
Both let and const are keywords in JavaScript for setting variables.
let is limited by scope and const is similar but can't be reassigned. Y
ou can learn more here

```

## Operators

---

## Operator Meaning

---

Assignment =
Addition +
Subtraction -
Increment ++
Decrement --
Multiplication \*
Division /
Modulus (Division Remainder) %
Loose Comparison ==
Strict Comparison ===
Not !
And &&
Or ||

## Functions

---

```
 function allows you to write a block of code that performs specific functionality.
 It is written like this:

function userGreeting() {
  return "Hello user!";
}

// Calling a function
userGreeting();

```

## Parameters

```

Functions can also accept parameters. They are defined between the
parenthesis and separated by a comma. Note: a function can accept any
number of parameters.

function greetUserByName(name) {
  return `Hello ${name}`;
}

greetUserByName("Johnny"); // returns "Hello Johnny"

```

## Return Value

---

```

```

## Conditionals

---

### Conditionals are a central piece in programming.

### JavaScript offers a couple of tools for checking expressions

### and conditionally running code.

```
"If" Statement
For writing conditional statements, the if, else if, else keywords are used and the comparison logic is wrapped in parenthesis:

if (age < 18) {
  console.log("You are not an adults and don't have access");
} else if (age < 21) {
  console.log("You are an adult, but have limited access");
} else {
  console.log("You have full access");
}

```

```
"Switch Case" Statement
A switch case is for making a single comparison again multiple pieces of data. This can be done with an "if" statement, but is more concise and better legibility.

You provide an expression by passing data into the switch, then the case presents a piece of data to compare to the switch expression. If the switch expression matches the case the code block is executed, if the comparison doesn't match the code block is skipped.

var day;
switch (new Date().getDay()) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
    day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case 6:
    day = "Saturday";
    break;
  default:
    console.log("Can't figure out day");
}

console.log(`Today is ${day}`);

```

## Loops

---

Another central piece to programming is the ability to loop through
the same code over and over to reduce repeating yourself and iterating through data.

```
### For Loop ###

To create an iterative loop, you have to set a base number and increment
through it until the expression is false:

// Set variable value, expression, iteration
var x;
for (x = 0; x < 10; x++) {
  console.log(x);
}

```

```
### While Loop ###

The while loop is another common iterative tool for programming.
You use the while keyword followed by an expression. While the expression is true,
the code will continue to loop through the code.

var x = 0;
while (x < 10) {
  console.log(x);
  x++;
}

```

## DAY 17 OF PROGRAMMING 11/3/20

---

### Things we worked on:

1.
2.
3.

---

## DAY 18 OF PROGRAMMING 11/4/20

---

### Things we worked on:

1.
2.
3.

---

## DAY 19 OF PROGRAMMING 11/5/20

---

### Things we worked on:

1.
2.
3.

---

## DAY 20 OF PROGRAMMING 11/6/20

---

### Things we worked on:

1.
2.
3.

---
