1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes 
let percentage =  function (marks, total) {
  return (marks * 100) / total;
}

let percentage2 =  (marks, total) => {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.



Function definition is an expression because it evaluates to a single value. When you execute the expression, it returns a value. 

```js
function sum(num1, num2) {
  return num1 + num2;
}
```

4. Why is a function call an expression in JavaScript?

Again, since function call evalues to a value, it is an expression in Javascript.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid 
five = add; // invalid - no parameters 
five = five(10, 11); // invalid - five is not defined
five = function () {
  return 'Hello';
}; // valid
```

6. What is the difference between function definition and function call? Explain with an example.
function definition defines the steps in a function,
function call executes the steps contained in a function. 


7. What is the similarities between function definition and function call?

function definition and function call both accepts parameters



8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; //valid - function is an object and object can take properties
```

9. What is higher order function explain with an example.

A function which takes another function as an argument or returns a function is called as a higher order function. 

function isOdd (num) {
  return num % 2 !== 0
}

function filter (arr, isOdd) {
  return arr.map(ele => isOdd(ele))
}

10. Explain what is callback function. Why you can pass a function inside a function?

Callback function is a function that is passed in another function as an argument. 
Since functions are objects, a callback function can be passed inside a function. 


