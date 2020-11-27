# Javascript

## DAY 16 OF PROGRAMMING 11/2/20

---

# Javascript

---

### Things we worked on:

---

1. Variables
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
 let = a;
  let a = "Something" //ending simi-colon not required...
  a = 1
  /* let does not allow you to redeclare inside of a function. It should be used in place of var*/

```

```
const a = 'someintin'
  a = 'something esle'//error cannot re-assign const.

/declare multiple
  let a,b,c
  a = 1;
  b = 2;
  c = 3;

  //declaring and assigning multiple
  let e,f=10,g=12
  //e is undefined f is 10 g is 12


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

1. Arrays
2. Objects
3. Arrays of Objects
4. Objects plus

---

### Creating an Array

```
 //create empty array
  let myArr = []

 //create array with items
  let myArr = ['a','b','c']

  //accessing via index
  console.log(myArr[1]) //b

```

## Modifying an Array

## Objects

## Array of Objects

## OBJECTS PLUS

---

-   typeof
-   instanceof

### TYPEOF

```
Functions are objects. We call them first class objects in javascript.

console.log(typeof 'yes') //string
  console.log(typeof new String('yes')) //object

  'yes' instanceof Object //false
  new String('yes') instanceof Object // true

  function test(){}

  console.log(typeof test) //function
  test instanceof Object //true

```

### Creating instance with new

```
Convention says if it is a object to be instanced you capatalize it.

function Animal() {}
  let rainbow = Animal() //undefined
  //Animal as a function doesn't return anything

  //creating an instance
  rainbow = new Animal()
  console.log(rainbow) //instance of Animal

```

### This

```
this is like self for python, but it is a keyword and not an argument. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new

 function Animal(type,name) {
      this.name = name;
      this.type = type;
  }
  let shadow = new Animal('cat', 'shadow')
  console.log(shadow)

//adding methods
  function Animal(type,name, noise) {
      this.name = name;
      this.type = type;
      this.noise = noise;
      this.makeNoise = function(){
          console.log(this.name+' says '+this.noise)
      }
  }

  let shadow = new Animal('cat', 'shadow', 'meow')
  console.log(shadow)
  shadow.makeNoise()

```

### Prototype

---

```
  function Animal(type,name,noise) {
      this.name = name;
      this.type = type;
      this.noise = noise;
  }

  Animal.prototype.makeNoise = function(){
      console.log(this.name+' says '+this.noise)
  }
```

## DAY 18 OF PROGRAMMING 11/4/20

---

### Things we worked on:

1. DOM 101
2.
3.

---

WHAT IS THE DOM?

The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page. MDN - Document Object Model
The DOM is the primary way that your JavaScript code will interact with a web page. Specifically, the browser provides a document variable that has properties and methods you can use to make changes to the page.

# How is the DOM related to the Browser Object Model?

Whereas the DOM represents the web page, the Browser Object Model (the BOM) represents the window or tab that is showing the page.

In JavaScript, the BOM is accessible through a window variable. This variable has a document property. You could say that the BOM (the window) contains a DOM (the document).

But the window object has other useful properties, such as history, screen, and location.

For example, window.screen object contains information about a user's browser, this includes the width and height properties. window.screen.width give you the current width of the browser's window. It can also be written without the window prefix as screen.width.

#

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
