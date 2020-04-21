## writeCode

### 1. Read the questions and do what is asked.

```js
/**
 Write a function named calculator that accepts three parameter
 - operation ('add', 'sub', 'mul','divide')
 - num1 (number)
 - num2 (number)
 and if operation is
    - 'add' returns num1 + num2.
    - 'sub' returns num1 - num2
    - 'mul' return num1 * num2
    - 'div' return num1 / num2
 */
//1. Write a Function Decleration
function calculator(num1,num2,operation){
   if(operation == 'add'){
      return num1 + num2;
   }else if(operation == 'sub'){
      return num1 - num2;
   }else if(operation == 'mul'){
      return num1 * num2;
   }else if(operation == 'div'){
      return num1 / num2;
   } else {
      return 'invalid operator';
   }

}

//2. Write an anonymous Function Expression
(function(num1,num2,operation){
   if(operation == 'add'){
      return num1 + num2;
   }else if(operation == 'sub'){
      return num1 - num2;
   }else if(operation == 'mul'){
      return num1 * num2;
   }else if(operation == 'div'){
      return num1 / num2;
   } else {
      return 'invalid operator';
   }
})(5,3,'add');

//3. Write an named Function Expression

let calculator = function (num1,num2,operation){
   if(operation == 'add'){
      return num1 + num2;
   }else if(operation == 'sub'){
      return num1 - num2;
   }else if(operation == 'mul'){
      return num1 * num2;
   }else if(operation == 'div'){
      return num1 / num2;
   } else {
      return 'invalid operator';
   }

}

//4. Write an Arrow Function  
let calculator = (num1,num2,operation) => (operation == 'add')? num1 + num2 : (operation == 'sub')? num1 - num2 : (operation == 'mul')? num1 * num2 :(operation == 'div') ? num1/num2 :'invalid operation';

//5. Write an Arrow Function with curly brackets (if possible)

let calculator = (num1,num2,operation) => {
   (operation == 'add')? num1 + num2 : (operation == 'sub')? num1 - num2 : (operation == 'mul')? num1 * num2 :(operation == 'div') ? num1/num2 :'invalid operation'; 
}

//6. Execute the function
calculator(5,3,'mul');

//7. Execute the function and store the return value in a variable.
let store =calculator (5,3,'sub');

//8. What is the typeof returnValue
//typeof store is number
```

### 2. Read the questions and do what is asked.

```js
/**
 Write a function named calculator that accepts three parameter
 - operation ('add', 'sub', 'mul','divide')
 - num1 (number)
 - num2 (number)
 and if operation is
    - 'add' returns num1 + num2.
    - 'sub' returns num1 - num2
    - 'mul' return num1 * num2
    - 'div' return num1 / num2
 */
//1. Write a Function Decleration

//2. Write an anonymous Function Expression

//3. Write an named Function Expression

//4. Write an Arrow Function

//5. Write an Arrow Function with curly brackets (if possible)

//6. Execute the function

//7. Execute the function and store the return value in a variable.

//8. What is the typeof returnValue
```
//FEEDBACK: Question repeated

### 3. Read the questions and do what is asked.

```js
/**
 Write a function named grade that accepts a number (marks below 500) calculates the percentage out of (500) and returns the grade as following
 * "A": 90-100%
 * "B": 80-89%
 * "C": 70-79%
 * "D": 60-69%
 * "F": 0-59%
 */
//1. Write a Function Decleration
function grade(n){
   var per=(n/500)*100;
   if(per >= 90 && per <=100){
      return 'A';
   }else if (per >=80 && per <90){
      return 'B';
   }else if(per >=70 && per <80){
      return 'C';
   }else if(per >=60 && per <70){
      return 'D';
   }else if(per < 60){
      return 'F';
   }
}

//2. Write an anonymous Function Expression

(function (n){
   var per=(n/500)*100;
   if(per >= 90 && per <=100){
      return 'A';
   }else if (per >=80 && per <90){
      return 'B';
   }else if(per >=70 && per <80){
      return 'C';
   }else if(per >=60 && per <70){
      return 'D';
   }else if(per < 60){
      return 'F';
   }
})(333);

//3. Write an named Function Expression

let grade = function (n){
   var per=(n/500)*100;
   if(per >= 90 && per <=100){
      return 'A';
   }else if (per >=80 && per <90){
      return 'B';
   }else if(per >=70 && per <80){
      return 'C';
   }else if(per >=60 && per <70){
      return 'D';
   }else if(per < 60){
      return 'F';
   }
}

//4. Write an Arrow Function

let grade = (n) => ((((n/500)*100) >= 90) && ((n/500)*100) <=100) ?
   'A': ((((n/500)*100) >= 80) && ((n/500)*100) <90) ?
   'B': ((((n/500)*100) >= 70) && ((n/500)*100) <80) ?
   'C': ((((n/500)*100) >= 60) && ((n/500)*100) <70) ?
   'D':'F';
//5. Execute the function

grade(333);

//6. Execute the function and store the return value in a variable.
let store = grade(333);

//7. What is the typeof returnValue
typeof store is string
```

### 4. Read the questions and do what is asked.

```js
/**
 Write a function named fullName that accepts two strings (firstName, lastName) and return the full name with an space between firstName and lastName
 */
//1. Write a Function Decleration
function fullName(firstName,lastName){
   return (firstName + ' ' +lastName);
}

//2. Write an anonymous Function Expression
(function(firstName,lastName){
   return (firstname + ' ' +lastName);
}) ('sudhanshu','shekhar');

//3. Write an named Function Expression
let fullName =function(firstName,lastName){
   return (firstName + ' ' +lastName);
}

//4. Write an Arrow Function

let fullName = (firstName,lastName) => (firstName + ' ' +lastName);

//5. Execute the function
fullName('sudhanshu','shekhar');

//6. Execute the function and store the return value in a variable.
let store = fullName('sudhanshu','shekhar');

//7. What is the typeof returnValue
//typeof store is string
```

### 5. Write a function `toCelsius` which converts temperature from Fahrenheit to Celsius:

```js
function toCelsius(farhenheit) {
   var fToc = ((farhenheit -32)*5)/9;
    return (farhenheit + "°F is " + fToc + "°C");
}
toCelsius(100);
```
