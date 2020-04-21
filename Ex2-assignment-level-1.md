## Function Defination-writeCode

1.  Define a function named `sayHello` when called `alert` saying "Hello JavaScript".

    - Call above function.
    - Store the return value in a variable named `one`
    - What is the `typeof` the value in `one`

    function sayHello(){
       return "Hello Javascript";
       
       
    }
     var one =sayHello();


2.  Change function (from Part 1 above) to accept name from user using `prompt` and store it in a variable named `usename` and alert message saying `Hello username`.

    - Call above function.
    - Store the return value in a variable named `two`
    - What is the `typeof` the value in `two`


    function 


3.  Change the function (from Part 2 above) to accept `username` as a parameter not from prompt.

4.  Change (from Part 4 above) return the message `Hello username` instead of alerting it.

    - Call above function.
    - Store the return value in a variable named `four`
    - What is the `typeof` the value in `four`

## writeQuiz

```js
function hello() {
  console.log("Hello World!");
}
let message = hello();
alert(typeof message);
```

What will be the message in alert in above code.

- [ ] Hello World!
- [ ] null
- [x] undefined //output
- [ ] string

## writeQuiz

```js
function hello() {
  return "Hello World!";
}
let message = hello();
alert(typeof message);
```

What will be the message in alert in above code.

- [ ] Hello World!
- [ ] null
- [ ] undefined 
- [x] string  //output

## writeQuiz

```js
function hello() {
  return "Hello World!";
}
let message = hello();
alert(typeof typeof message);
```

What will be the message in alert in above code.

- [ ] Hello World!
- [ ] null
- [ ] undefined
- [x] string //output

## writeTextAnswer

Why you can store function as a value in a variable? Explain with example.

Functions in javascript are objects and objects are values in javascript.So, we can store function as a value in a variable.For example:
                  var add = function sum() {
                    return 21;
                  };

## Different Function Types-writeCode

For the given problems write do the following:

1. Write a Function Declaration
    function hello(){
      alert("hello everyone!");
    }

2. Write a Function Expression

    var hello = function(){
      alert("hello everyone");
    }
3. //FEEDBACK: arrow functions without curly brackets to be added
4. Write a Arrow Function with curly brackets (if possible)

    let sum = (a,b) => a+b;

5. Function Execution

    sum(1,2);

6. Store the value of function execution in a variable

  var store = sum(1,2);

7. Find the `typeof` of the the variable

    typeof(store); //number

```js
/**
 * Write a function named convertToString that accepts a number,
 converts the number into a string (hint: use String()) and return the converted value.
 */
// Do the following for the given problem:
//1. Write a Function Decleration
function convertToString(n) {
  return String(n);
}

//2. Write a Function Expression
let convertToString = function(n) {
  return String(n);
};

//3. Write an Arrow Function
let convertToString = n => String(n);

//4. Write an Arrow Function with curly brackets (if possible)
let convertToString = n => {
  return String(n);
};

//5. Execute the function
convertToString(21);

//6. Execute the function and store the return value in a variable.
let returnValue = convertToString(23);

//7. What is the typeof returnValue
// typeof returnValue is "string"
```

Do the same for the following problems:

### 1. Read the questions and do what is asked.

```js
/**
 Write a function named addOne that accepts a number,
 add one to the given value and return it(hint: use return keyword).
 */
//1. Write a Function Decleration

  function addOne(n){
    return n+1;
  } 

//2. Write a Function Expression

  let addOne = function(n){
    return n+1;
  }

//3. Write an Arrow Function
let addOne = (n) => n+1;

//4. Write an Arrow Function with curly brackets (if possible)
let addOne = (n) => {
  return n+1;
}

//5. Execute the function
addOne(2);

//6. Execute the function and store the return value in a variable.
let store = addOne(2);

//7. What is the typeof returnValue
//typeof store is number. 
```

### 2. Read the questions and do what is asked.

```js
/**
 Write a function named substractOne that accepts a number,
 substract one from the given value and return it. (hint: use return keyword)
 */
//1. Write a Function Decleration
  function substractOne(n){
    return n-1;
  }

//2. Write a Function Expression
  var substractOne = function(n){
    return n-1;
  }

//3. Write an Arrow Function
  var substractOne = (n) => n-1;

//4. Write an Arrow Function with curly brackets (if possible)
var substractOne = (n) => {
  return n-1;
}

//5. Execute the function
substractOne(5);

//6. Execute the function and store the return value in a variable.
var store = subtractOne(5);

//7. What is the typeof returnValue
//typeof store is number
```

### 3. Read the questions and do what is asked.

```js
/**
 Write a function named sum that accepts two numbers,
 returns the sum of the passed value.
 */
//1. Write a Function Decleration
  function sum(a,b){
    return a+b;
  }

//2. Write a Function Expression
  var sum  = function(a,b){
    return a+b;
  }

//3. Write an Arrow Function

  let sum = (a,b) => a+b;

//4. Write an Arrow Function with curly brackets (if possible)
 let sum = (a,b) => {
   return a+b;
 }

//5. Execute the function
 sum(5,6);

//6. Execute the function and store the return value in a variable.
let store = sum(5,6);

//7. What is the typeof returnValue
//typeof store is number
```

### 4. Read the questions and do what is asked.

```js
/**
 Write a function named square that accepts a number,
 returns the number multiplied by itself.
 */
//1. Write a Function Decleration
  function square(n){
    return n*n;
  }

//2. Write a Function Expression
var square = function(n){
  return n*n;
}

//3. Write an Arrow Function
let square = (n) => n*n;

//4. Write an Arrow Function with curly brackets (if possible)
let square = (n) => {
  return n*n;
}

//5. Execute the function
square(7);

//6. Execute the function and store the return value in a variable.
let store = square(7);

//7. What is the typeof returnValue
//typeof store is number
```

### 5. Read the questions and do what is asked.

```js
/**
 Write a function named isGreater that accepts two numbers x and y and returns true if x is greater than y or return false.
 */
//1. Write a Function Decleration
  function isGreater(a,b){
    if(a > b){
      return true;
    }else{
      return false;
    }
  }

//2. Write a Function Expression
let isGreater = function(a,b){
  if(a > b){
    return true;
  }else {
    return false;
  }

}

//3. Write an Arrow Function

let isGreater = (a,b) => (a > b)? true : false;

//4. Write an Arrow Function with curly brackets (if possible)
let isGreater = (a,b) => {
  (a > b)? true : false;
}

//5. Execute the function
isGreater(5,3);

//6. Execute the function and store the return value in a variable.

let store = isGreater(5,3);

//7. What is the typeof returnValue
//typeof store is number
```

### 6. Read the questions and do what is asked.

```js
/**
 Write a function named oddOrEven that accepts a number and returns "Number is odd" for odd number and "Number is even" for even number.
 */
//1. Write a Function Decleration
  function oddOrEven(n){
    if(n % 2 == 1){
      return "Number is odd";
    }
    if(n % 2 == 0){
      return "Number is even";
    }
  }

//2. Write an anonymous Function Expression

(function (n) {
   if(n % 2 == 1){
   return "Number is odd";
   }else {
   return "Number is even";}
})(5);

//3. Write an named Function Expression

let oddOrEven = function(n){
    if(n % 2 == 1){
      return "Number is odd";
    }
    if(n % 2 == 0){
      return "Number is even";
    }
  }

//4. Write an Arrow Function
let oddOrEven = (n) => (n % 2 == 0)? "Number is even" : "Number is odd";

//5. Write an Arrow Function with curly brackets (if possible)

let oddOrEven = (n) => {
  (n % 2 == 0)? "Number is even" : "Number is odd";
}

//6. Execute the function
oddOrEven(4);

//7. Execute the function and store the return value in a variable.
var store = oddOrEven(4);

//8. What is the typeof returnValue
// typeof store is number
```
