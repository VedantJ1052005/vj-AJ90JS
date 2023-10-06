
# My JavaScript Learning Journey #AJ90JS

## Variables in JS

In JavaScript, variables are used to store data that can be manipulated or referenced later in your code. Think of them as named containers for storing information. Here are some key concepts about variables:

### Declaring Variables

To declare a variable in JavaScript, you can use the `let`, `const`, or `var` keyword:

- `let`: Used for variables that can be reassigned.
- `const`: Used for variables that should not be reassigned (constant values).
- `var`: Similar to `let`, but has different scoping rules.

Example:
```javascript 
let Name = "Vedant";
const age = 18;
```

### Variable Scope

Variable scope defines where a variable is accessible or visible within your code. In JavaScript, there are two main types of variable scope:

- **Global Scope**: Variables declared outside of any function or block are considered global and can be accessed from anywhere in your code.

- **Local Scope**: Variables declared inside a function or block have local scope and are only accessible within that function or block.

Example:
```javascript
let globalVariable = "I'm a global variable";

function myFunction() {
  let localVariable = "I'm a local variable";
  console.log(localVariable); // Accessible within the function
  console.log(globalVariable); // Accessible within the function
}

console.log(globalVariable); // Accessible globally
console.log(localVariable); // Error: localVariable is not defined
```

### Data Types

JavaScript has several data types for storing different kinds of information:

- **Primitive Data Types**: These are basic data types and include `number`, `string`, `boolean`, `null`, `undefined`, and `symbol`. They are immutable.

- **Complex Data Types**: These are more advanced data types and include `object`, `array`, and `function`. They can hold multiple values.

Example:
```javascript
let num = 42; // Number
let text = "Hello, world!"; // String
let isTrue = true; // Boolean
let empty = null; // Null
let notDefined; // Undefined

let person = { name: "Alice", age: 30 }; // Object
let colors = ["red", "green", "blue"]; // Array
function greet() { console.log("Hello!"); } // Function
```
