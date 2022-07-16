1. What does thread of execution means in JavaScript?
Javascript goes through the code line by line and this process is called the thread of execution.

2. Where the JavaScript code gets executed?

Javascript code gets executed in Global execution context and function execution contexts. 

3. What does context means in Global Execution Context?

context means environment

4. When do you create a global execution context.

When Javascript runs the code fo the first time, it creates a global execution context.

5. Execution context consists of what all things?

Execution context contains a memory section and one more section for computation or execution

6. What are the different types of execution context?

Global execution context and function execution context

7. When global and function execution context gets created?

When Javascript starts to run a  code, global execution context is created. Whenever it encounters a code where a function is being executed, it creates a function execution context. 

8. Function execution gets created during function execution or while declaring a function.

only when the function is being executed. 


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.





```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/IMG_9562.HEIC)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}
 
var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/IMG_9564.HEIC)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/IMG_9565.HEIC)