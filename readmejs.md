# Introduction to java script
- alert("hello");


## Data types
- typeof(123);
  - "number"

- typeof(Binod); 
   - "String"
- typeof(true/false);
   - "Boolean"

## Javascript variables
- var myName = "Binod";
- var name prompt("What is your name?");

```
var myName = "Binod";
var yourName = prompt("What is your name");
alert("My name is" + myName + "welcome" + yourName + "!");

```
<img src="./img/Screenshot 2025-06-10 125322.png" alt="example">


## Exercise
```
function test() {
    var a = "3";
    var b = "8";
    
var c = a;
a = b ;
b = c ;


alert("a");
alert("b");
    console.log("a is " + a);
    console.log("b is " + b);
}
 
```
## String length
```
var tweet = prompt("compose your tewwt");
alert("You have written " + tweet.length + " characters, you have" + (140 - tweet.length) + "characters remaining");
```
<img src="./img/Screenshot 2025-06-10 151319.png" alt="string.length example">
<img src="./img/Screenshot 2025-06-10 151457.png" alt="string.length example">


## Slicing and Extracting Parts of String
```
var tweet = prompt("Compose your tweet");
var tweetUnder140 = tweet.slice(0,140);
alert(tweetUnder140);
```
<img src="./img/Screenshot 2025-06-10 151319.png" alt="slicing example">
<img src="./img/Screenshot 2025-06-10 151511.png" alt="dogAge example">

## Changing casing in text
```
char.toUpperCase();
```
## Basic Arthemaatic and the Modulo Operator in javascript
```
var dogAge = prompt("How old is your dog?");
var humanAge = ((dogAge -2) * 4) + 21;
alert("Your dog is " + humanAge + " years old in human yeras");

``` 
<img src="./img/Screenshot 2025-06-10 145310.png" alt="dogAge example">
<img src="./img/Screenshot 2025-06-10 145339.png" alt="dogAge example">

## Increment and Decrement Expressions
```
- Increment
var x = 5;
x++
console.log(x);

- Decrement
var x = 5;
x--
console.log(x);

- To increaase the value by more than one
var x = 5;
x += 2;
```

## Creating and Calling Functions
```
- Creating The Function
function turnOnLight(){

    - alert(instrucions);
}

-Calling The Function
  turnOnLight();
  ```

  ## Output & Return Values
  ```
  function getMilk(money, costPerBottle) {   
  console.log("leaveHouse");
  console.log("moveRight");
  console.log("moveRight");
  console.log("moveUp");
  console.log("moveUp");
  console.log("moveUp");
  console.log("moveUp");
  console.log("moveRight");
  console.log("moveRight");


 
  console.log("buy " + calcBottle(money, costPerBottle) + "bottles of milk");

  
  console.log("moveLeft");
  console.log("moveLeft");
  console.log("moveDown");
  console.log("moveDown");
  console.log("moveDown");
  console.log("moveDown");
  console.log("moveLeft");
  console.log("moveLeft");
  console.log("enterHouse");

  return calcChange(money, costPerBottle);
}

 function calcBottle(startingMoney , costPerBottle){
   var numberOfBottles = Math.floor(startingMoney / costPerBottle);
   return numberOfBottles;
 }
function calcChange(startingAmount, costPerBottle){
  var change = startingAmount % costPerBottle;
  return change;
}
console.log ("hello sir, here is your " + getMilk(10,3) + "change") ;
```

## BMI Calculator
```
function bmiCalculator(weight, height){
 var bmi = weight / (height*height);
    return Math.round(bmi);
}

var bmi = bmiCalculator(65,1.8);
console.log(bmi);
```

## Love Calculator
```
var name = prompt("Name of first person.");
var name = prompt("Name of second person.");

var n = Math.random() ;
n = n*100;
n = Math.floor(n) + 1;
alert( "Your love score is " + n + "%❤️");
```

## Using If-Else Conditionals & Logics  
```

alert("Calculate your love❤️💕 percentage");
var name = prompt("Name of first person.");
var name = prompt("Name of second person.");

var n = Math.random() ;
n = n*100;
n = Math.floor(n) + 1;
if (n > 70){
alert( "Your love score is " + n + "%❤️");
} else {
    alert ("Your love score is " + n)
}
```
## Working With Javascrips Arrays
```

var guestlist = ("Binod" + "pratyush" + "ashok" + "lakesh");
var guestName = prompt("What is your name?");

if (guestlist.includes(guestName)){
    alert("Welcome");
}else{
    alert("Sorry, may be next time");
}
```
##  Adding Elements and Intermediate Array Techniques
```
var output = [];
var count = 1;
function fizzBuzz() {
   

  if (count % 3 ===0 && count % 5 === 0){
   output.push("fizzBuzz");
  }
 
   else if (count % 3 === 0){
    output.push("fizz");
   }else if (count % 5 ===0){
    output.push("buzz");
   }
   else{
    output.push(count);
   }
   count++;
console.log(output);
}
```
![alt text](image.png)
![alt text](image-1.png)

## Who's Buying Lunch? Code Challenge
```
function whosPaying(names) {
  
        var numberOfPeople = names.length;
        var randomPersonPosition = Math.floor(Math.random() * numberOfPeople);
        var randomPerson = names[randomPersonPosition];
        return randomPerson + " is going to buy lunch today!"
   
    }
    
    whosPaying(["Angela", "Ben", "Jenny", "Michael", "Chloe"]);

```
output

![alt text](image-2.png)

## while loop
```
var i=1;
while(i < 2){
  console.log(i);
  i++
}
```
```
var numberOfBottles = 99
while (numberOfBottles >= 89)          {
    var bottleWord = "bottle";
    if (numberOfBottles === 89) {
        bottleWord = "bottles";
    } 
    console.log(numberOfBottles + " " + bottleWord + " of beer on the wall");
    console.log(numberOfBottles + " " + bottleWord + " of beer,");
    console.log("Take one down, pass it around,");
	numberOfBottles--;
    console.log(numberOfBottles + " " + bottleWord + " of beer on the wall.");
}
```
output

![alt text](image-5.png)
![alt text](image-6.png)

## For loop
```
for(var i=1; i < 2; i++){
  console.log(i);
}
```
```
var output = [];

function fizzBuzz() {
   
for (var count = 1; count < 101; count++){
  if (count % 3 ===0 && count % 5 === 0){
   output.push("fizzBuzz");
  }
 
   else if (count % 3 === 0){
    output.push("fizz");
   }else if (count % 5 ===0){
    output.push("buzz");
   }
   else{
    output.push(count);
   }
 }
  
console.log(output);
}
```
output
![alt text](image-4.png)