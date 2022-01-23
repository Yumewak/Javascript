# JavaScript

## Javascript Alerts
```javascript
alert("Hello");
```

## Data types
```
String: "Hello"
Numbers: 123
Boolean: true false
```
```
typeof() Tells you what is the data type of whatever it is that you put within these round brackets
```
```javascript
typeof()
```

## Javascript Variables
```javascript
var myName = "Angela";
var yourName = prompt("What is your name?")
```
```
Exercise
```
```javascript
function test() {
    var a = "3";
    var b = "8";
    
/***********Do not change the code above 👆*******/
//Write your code on lines 7 - 9:



/***********Do not change the code below 👇*******/

    console.log("a is " + a);
    console.log("b is " + b);
}
```

## Naming conventions
```
1.- Give your variables meaningful names so that anybody can figure out quite easily
what is the data that's likely to be stored inside it.
```
```javascript
var myName = "Socratic"
```
```
2.- You can't give your variable a keyword name but you can modify to contain keyword.
```
```javascript
var var= "abc" NOT ALLOWED
var myvar = "abc" ALLOWED
```
```
3.- Your variable name cannot begin with a number, but like keywords your variable name
can contain numbers.
```
```javascript
var 123 = 123 NOT ALLOWED
var my123 = 123 ALLOWED
```
```
4.- Your variable name can't contain spaces
```
```javascript
var my name = "Socratic" NOT ALLOWED
var myName = "Socratic" ALLOWED
```
```
5.- Names can only contain letters, numbers, the dollar sign, and an underscore
```
```javascript
var abc123$_ = "Value"
```
```
A good practice is using camel casing, this means that you will start out the name with
a lowercase word and then every subsequent word will be capitalized
```
```javascript
var userScoreFinal = "Value"
```

## Strings
```
Concatenation: "a" + " " + "b" = a b
```
```javascript
var messege = "Hello"
var name = "Mario"

// Create an alert that says "Hello Mario"
// Write your code below this line:
```

## Length and Retrieving
```javascript
var name = "Mario"
name.length
```
```
// Create a prompt where the user can enter a long string of text and you will tell them how many characters they have written and how many characters they have remaining out of either 140 or 280 characters
//Expected output: You have written 182 characters, you have -42 characters left.
```

## Slicing and Extracting
```javascript
var name = "Mario"
name.slice (0,1)
//Expected output "M"
//Write a code that creates a prompt, and when you paste in a large text it should give you an alert that cuts your text down to only 140 characters.
```

## toUpperCase() and toLowerCase()
```javascript
var name = "Angela"
name = name.toUpperCase()
name = name.toLowerCase()
//Create a prompt that asks the use for their name, if is uppercase or lowercase, send them an alert that says "Hello, Name", the "Name" must be capitalized but only for the first character and non of the rest of the characters
```

## Basic Arithmetic and the Modulo Operator
```javascript
//Addition
var a = 2+3; //5

//Subtraction
var b = 10-2; //8

//Multiplication
var c = 3*3; //9

//Division
var d = 6/2; //3

//Modulo gives the remainder of the division 9/6=1 and you get a remainder of 3
var e = 9%6; //3

//Code that find if a number that you have is odd or even
//Code that convert a dog age to human age, Formula: humanAge=(dogAge-2)*4+21
```

## Increment and Decrement expressions
```
var x = 5;
x = x+1; // this is the same has x++
x++
x--
x+=2 // 7
//You can also use += to increase by the value of another variable
var x=5;
var y=3;
x+=y; //8
+=
-=
*=
/=
```

## Functions
```javascript
//Vanilla version
//Create the function
function getMilk() {}

//Call the function
Calling the function
getMilk();
```

## Functions parameters and arguments
```javascript
//Chocolate flavor
//Creating the function
function getMilk(bottles){
  var cost= bottles*1.5;
  //Do something with cost
}

//Calling the function
getMilk(2);

//Example
    function getMilk(money) {   // getMilk(money) "money" is a parameter
      var numberBottles = Math.floor(money/1.5)
      console.log("buy " + numberBottles + " Milk")
    }
getMilk(5); //getMilk(5) "5" is an argument
```

## Functions Outputs & Return Values
```javascript
//Strawberry flavor
function getMilk(money, costPerBottle) {
  //var numBottles = Math.floor (money / 1.5);
  console.log("Buy " + calcBottles(money,costPerBottle) + " Bottles of Milk");
  return calcChange(money, costPerBottle)
}

function calcBottles(startingMoney, costPerBottle) {
  var numberOfBottles = Math.floor (startingMoney / costPerBottle);
  return numberOfBottles;
}

function calcChange(startingAmount, costPerBottle) {
  var change = startingAmount % costPerBottle;
  return change;
}

console.log("Hello master, here is your " + getMilk(5, 1.5) + " change:")
```
```
Every time you see this "function name() {}" we are creating a function.
If the parenthesis contain some inputs like "function name(num1, num2) {}" this variables "num1,num2" are called parameters
and only exist inside the function

Every time you see this "name()" is called a function invocation
And if there is nothing inside the parenthesis, then just execute the code inside the function that is being invoked
But if the parenthesis contain some inputs like "name(2,5)" it pass this imputs to the function, this imputs are called arguments
```

## Random Number Generator
```javascript
var n = Math.random(); // Example of a number with 16 decimal places generated: 0.3653767653458296
Math.random() generates a number between 0 - 0.9999999999999999 it never reaches 1
```
```javascript
//Dice generator
var n = Math.random();
n = n*6;
n = Math.floor(n+1);
```
```javascript
//Love calculator
prompt("Whats the first name?")
prompt("Whats the second name?")

var loveScore = Math.floor(Math.random()*101)
alert(loveScore)
```
