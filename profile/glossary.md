# Javascript Glossary

### Argument
The actual value passed to a function when called.

Example:
```javascript
greet("John"); // "John" is the argument
```

Example (multiple arguments):
```javascript
add(5, 10); // 5 and 10 are arguments
```

### Array
A list-like object used to store multiple values.

Example:
```javascript
let fruits = ["Apple", "Banana", "Cherry"];
```

Example (Access an Array item by index):
```javascript
console.log(fruits[0]); // "Apple"
```

### Arrow Function
A shorthand way to write functions.

Example (concise syntax):
```javascript
const add = (a, b) => a + b;
```

Example (block syntax):
```javascript
const greet = (name) => {
  return `Hello, ${name}!`;
};
```

### Boolean
A data type with only two values: `true` or `false`.

Example:
```javascript
let isActive = true;
```

Example:
```javascript
let hasCompleted = false;
```

### Concatenation
A way to put multiple strings together into a new string.

Example (concatenation):
```javascript
let name = "Bob";
let greeting = "Hello, " + name;
console.log(greeting); // prints "Hello, Bob"
```

### Conditional Statement
A way to execute different code based on conditions.

Example (`if` and `else`):
```javascript
if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

### Decrement
To decrease a numeric value by 1.

Example (using `--`):
```javascript
let i = 5;
i--; // i is now 4
```

Example (using `-=`):
```javascript
let count = 10;
count -= 1; // count is now 9
```

### DOM (Document Object Model)
A programming interface for manipulating HTML and CSS using JavaScript.

Example (access element):
```javascript
let header = document.getElementById("header");
```

Example (modify element):
```javascript
header.textContent = "Welcome!";
```

### Event Listener
A way to handle user interactions like clicks.

Example:
```javascript
button.addEventListener("click", () => alert("Clicked!"));
```

Example (separate function):
```javascript
const handleHover = () => { alert("Hover!"); }
button.addEventListener("mouseover", handleHover);
```

### Function
A reusable block of code that performs a specific task.

Example (function declaration):
```javascript
function greet(name) {
  return "Hello, " + name;
}
```

Example (arrow function):
```javascript
const greet = (name) => "Hello, " + name;
```

A function can be passed as an argument to another function.

Example:
```javascript
function handleClick() {
  alert("Click happened!");
}
button.addEventListener("click", handleClick);
```

### Increment
To increase a numeric value by 1.

Example (using `++`):
```javascript
let i = 0;
i++; // i is now 1
```

Example (using `+=`):
```javascript
let count = 5;
count += 1; // count is now 6
```

### JSON (JavaScript Object Notation)
A lightweight data format.

Example:
```javascript
let user = { "name": "Alice", "age": 25 };
```

Example (convert to JSON string):
```javascript
let userJSON = JSON.stringify(user);
```

### Local Storage
A way to store data in the browser persistently.

Example:
```javascript
localStorage.setItem("username", "Alice");
```

Example (retrieve item):
```javascript
let name = localStorage.getItem("username");
```

### Loop
A way to execute a block of code multiple times.

Example (`for` loop):
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

Example (`while` loop):
```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

Example (`forEach` loop):
```js
[0, 1, 2, 3, 4].forEach(function(number) {
  console.log(number);
});
```

### Method
A function that belongs to an object.

Example:
```javascript
let person = {
  name: "John",
  greet: function() {
    return "Hello " + this.name;
  }
};
```

Note that `this` refers to the object itself.

Example (calling method):
```javascript
console.log(person.greet()); // "Hello John"
```

### Null
Represents an intentional absence of value.

Example:
```javascript
let value = null;
```

Example (checking for null):
```javascript
if (value === null) {
  console.log("No value");
}
```

### Number
A data type representing numeric values.

Example (integer):
```javascript
let age = 25;
```

Example (decimal):
```javascript
let price = 9.99;
```

### Object
A collection of key-value pairs.

Example:
```javascript
let person = { name: "John", age: 30 };
```

Example (accessing a property):
```javascript
console.log(person.name); // "John"
```

### Operator
Symbols used to perform operations.

Example (plus operator `+`):
```javascript
let sum = 2 + 3;
```

Example (comparison operator `==`):
```javascript
let isEqual = (age == 18);
```

### Parameter
A variable used in function declarations to accept input values.

Example:
```javascript
function greet(name) {
  console.log(`Hello, ${name}`);
} // name is the parameter

greet("Bob"); // "Bob" is the argument
```

Example (multiple parameters):
```javascript
const add = (x, y) => x + y; // x and y are parameters
```

### Promise
Represents a value that may be available now, in the future, or never.

Example:
```javascript
fetch("url").then(response => response.json());
```

Example (creating promise):
```javascript
const promise = new Promise((resolve, reject) => {
  resolve("Success");
});
```

### Property
A key-value pair that belongs to an object.

Example:
```javascript
let car = { brand: "Toyota", model: "Corolla" };
```

`brand` and `model` are properties, and "Toyota" and "Corolla" are values.

Example (accessing properties):
```javascript
console.log(car.brand); // "Toyota"
console.log(car.year); // undefined
```

### String
A sequence of characters enclosed in quotes (`""` or `''` or ` `` `).

Example:
```javascript
let name = "John";
let city = 'Auckland';
let car = `Mazda Mx-5 Miata`;
```

Example (finding the length of a string):
```
console.log(name.length); // Prints 4
console.log(city.length); // Prints 8
```

### Template Literal
A way to create strings using backticks (`` ` ``) and `${}` for interpolation.

Example:
```javascript
let greeting = `Hello, ${name}!`;
```

Example (multi-line):
```javascript
let multiLine = `This is a string
on multiple lines`;
```

### Undefined
A variable that has been declared but not assigned a value.

Example:
```javascript
let x;
```

### Variable
A container for storing data values. Declared using `let` or `const`.

Example (`let`):
```javascript
let score = 10;
let isFridge = false;
```

Example (`const`):
```javascript
const pi = 3.14;
const birthdayInWords = "3 March 1901";
```
