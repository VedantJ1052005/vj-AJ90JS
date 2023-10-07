# Loops in JavaScript

Loops are essential programming constructs that allow you to execute a block of code repeatedly. In JavaScript, there are several types of loops:

## 1. `for` Loop

The `for` loop is used when you know in advance how many times the loop should run. It consists of three parts: initialization, condition, and iteration.

```javascript
for (let i = 0; i < 5; i++) {
  // Code to be executed
  console.log(`Iteration ${i + 1}`);
}
```

**Output:**

```plaintext
Iteration 1
Iteration 2
Iteration 3
Iteration 4
Iteration 5
```

## 2. `while` Loop

The `while` loop repeatedly executes a block of code as long as a specified condition is true.

```javascript
let count = 0;
while (count < 5) {
  // Code to be executed
  console.log(`Count: ${count}`);
  count++;
}
```

**Output:**

```plaintext
Count: 0
Count: 1
Count: 2
Count: 3
Count: 4
```

## 3. `do...while` Loop

The `do...while` loop is similar to the `while` loop, but it guarantees that the code block is executed at least once before checking the condition.

```javascript
let x = 0;
do {
  // Code to be executed
  console.log(`x: ${x}`);
  x++;
} while (x < 5);
```

**Output:**

```plaintext
x: 0
x: 1
x: 2
x: 3
x: 4
```

## Loop Control Statements

JavaScript provides loop control statements to control the flow within loops:

- `break`: Terminates the loop and transfers control to the next statement after the loop.

- `continue`: Skips the current iteration and proceeds to the next iteration of the loop.

### Example of `break`

```javascript
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break; // Terminate the loop when i is 3
  }
  console.log(`Iteration ${i + 1}`);
}
```

**Output:**

```plaintext
Iteration 1
Iteration 2
```

### Example of `continue`

```javascript
for (let i = 0; i < 5; i++) {
  if (i === 2) {
    continue; // Skip iteration when i is 2
  }
  console.log(`Iteration ${i + 1}`);
}
```

**Output:**

```plaintext
Iteration 1
Iteration 3
Iteration 4
Iteration 5
```

## Iterating Arrays with Loops

Loops are often used to iterate over arrays:

```javascript
const colors = ["red", "green", "blue"];

for (let i = 0; i < colors.length; i++) {
  console.log(`Color: ${colors[i]}`);
}
```

**Output:**

```plaintext
Color: red
Color: green
Color: blue
```

## `for...of` and `for...in` Loops

JavaScript also offers `for...of` and `for...in` loops for iterating through arrays and objects more conveniently.

### Example of `for...of`

```javascript
const fruits = ["apple", "banana", "cherry"];

for (const fruit of fruits) {
  console.log(`Fruit: ${fruit}`);
}
```

**Output:**

```plaintext
Fruit: apple
Fruit: banana
Fruit: cherry
```

### Example of `for...in`

```javascript
const person = { name: "Alice", age: 30 };

for (const key in person) {
  console.log(`${key}: ${person[key]}`);
}
```

**Output:**

```plaintext
name: Alice
age: 30
```

These are the fundamental concepts of loops in JavaScript, which are crucial for creating repetitive tasks and handling data efficiently.
