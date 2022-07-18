Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // `Reference Error username is not defined`

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the variable defined inside a block from outside.

The above code will throw an error `Reference Error username is not defined`.
```

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // `Reference Error username is not defined`
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the variable defined inside a block from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // `Arya`
```


In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block defined by var which we can access.

The above code will output`Arya`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); //  SyntaxError: Identifier 'username' has already been declared

We are looking for the variable username but its already defined by let at the start. So the code will run into an error since we are trying to redeclare it again inside the block scope from which var can bubble out. 
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John

let is block scoped so when you try to access username in the global scope, there is only one username with `John` as the value. 
```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // `John`

Again, here there is only one username in global scope with John as the value. The one inside function scope is limited to the function. 
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0
}
console.log(i, 'Second'); // 10

since var is not block scoped, the final value of i is available outside in the global scope. So first value would be 0 while the Second value would be 10, which is also the final output of i in the for loop.
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0
}
console.log(i, 'Second'); // undefined

since we declare i using let, the variable is not available outside of the block scope. So it will return undefined. 
```
