## writeCode

### Read the questions and do what is asked.

```js
/**
 Write a function named calculator that accepts three parameter
 - operation ('add', 'sub', 'mul','divide')
 - num1 (number)
 - num2 (number)
 and if operation is
    - 'add' returns num1 + num2.
    - 'sub' returns num1 - num2 (if num1 is smaller than num2 alert "First number should not be smaller than second number.)
    - 'mul' return num1 * num2
    - 'div' return num1 / num2 (if num1 is smaller than num2 alert "First number should not be smaller than second number.)

  also print the operation in alert after operation like if 'add' => 5 + 66 = 71 etc
 */
//1. Write a Function Decleration
function calculator(num1,num2, operation){
  if(operation == 'add'){
    return num1 + num2;
  }
  if(operaton == 'sub'){
    if(num1>num2){
      return num1 - num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
  if(operation == 'mul'){
    return num1 * num2;
  }
  if(operaton == 'div'){
    if(num1>num2){
      return num1 / num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
}

//2. Write an anonymous Function Expression

(function (num1,num2, operation){
  if(operation == 'add'){
    return num1 + num2;
  }
  if(operaton == 'sub'){
    if(num1>num2){
      return num1 - num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
  if(operation == 'mul'){
    return num1 * num2;
  }
  if(operaton == 'div'){
    if(num1>num2){
      return num1 / num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
})(5,3,'sub');

//3. Write an named Function Expression
let calculator = function (num1,num2, operation){
  if(operation == 'add'){
    return num1 + num2;
  }
  if(operaton == 'sub'){
    if(num1>num2){
      return num1 - num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
  if(operation == 'mul'){
    return num1 * num2;
  }
  if(operaton == 'div'){
    if(num1>num2){
      return num1 / num2;
    }else {
      return 'First number should not be smaller than second number';
    }
  }
}

//4. Write an Arrow Function

let calculator = (num1, num2,operation) => (operation == 'add')? num1 + num2 : ((operation == 'sub')?  num1-num2 : 'first number should be larger than second number')? : (operation == 'mul')? num1 * num2 : ((operation == 'div')? num1 / num2 : 'first number should be larger than second number');

//5. Write an Arrow Function with curly brackets (if possible)

//6. Execute the function
calculator(5,3,'add');

//7. Execute the function and store the return value in a variable.
let store = calculator (5,3,'mul');

//8. What is the typeof returnValue
```

## writeTextAnswer

```js
function add(var a = 0,var b = 0){
  return a + b;
}
add(21, 23);
```

- Is the code above valid or not?
invalid
- Explain the reason.
in placeholder we cannot declare a variable.

## writeQuiz

```js
function add(a = 0; b) {
  return a + b;
}
add(21);
```

What will be the output of the above code?

- [x] 21
- [x] 0
- [x] 210
- [x] NaN

error inside parameter we cannot use semicolon
## writeQuiz

```js
function add(a = 0, b = 0) {
  return a + b;
}
add(undefined, 21);
```

What will be the output of the above code?

- [x] 21
- [ ] 0
- [ ] 210
- [ ] NaN

## writeTextAnswer

```js
function knowWhy(value) {
  return if(value === 21){
    return "Yes"
  } else {
    return "No"
  }
}
knowWhy(211);
```

- Output of the above code 
error
- Is the code above valid or not?
invalid
- Explain the reason.
in return statement we cannot write any condition .i.e it should be an expression which has some value

## writeTextAnswer

```js
function isItIf(ifElse) {
  return ifElse;
}
isItIf(if(true){console.log('Testing')});
```

- Output of the above code 
error
- Is the code above valid or not?
invalid
- Explain the reason.
we cannot write condition in function call . i.e it should contain an expression having some value
