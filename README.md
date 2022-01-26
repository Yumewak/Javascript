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

## Control statements: Using If-Else Conditionals & Logic
```javascript
if (track === "clear) {goStraight();}
else {turnRight();}

//Love Calculator
prompt("Whats the first name?")
prompt("Whats the second name?")

var loveScore = Math.floor(Math.random()*101)

if (loveScore > 70) {
  alert("Your love score is " + loveScore + "%" + " You love each other like Kanye loves Kanye")
} else {
  alert("Your love score is " + loveScore + "%")
}
```

## Comparators and Equality
```
==  Is equal to //It doesn't look for data type match
=== Is equal to //Data type also match
!== Is not equal to
>   Is greater than
<   Is lesser than
>=  Is greater or equal to 
<=  Is lesser or equal to 
```
```javascript
var a = 1;
var b = "1";
console.log(typeof(a));
console.log(typeof(b));
if (a === b) {
  console.log("yes")
} else {
  console.log("no")
}
```

## Combining comparators
```
&& AND
|| OR  //alt+124
!  NOT
```
```javascript
prompt("Whats the first name?")
prompt("Whats the second name?")

var loveScore = Math.floor(Math.random()*101)

if (loveScore > 70) {
  alert("Your love score is " + loveScore + "%" + " You love each other like Kanye loves Kanye")
} 

if(loveScore > 30 && loveScore <= 70) {
  alert("Your love score is " + loveScore + "%")
}

if (loveScore <=30) {
  alert("Your love score is " + loveScore + "%" + " You go together like oil and water.")
}
```

## Nested if-else
```javascript
//Leap Year Challenge
function isLeap(year) {
    
/**************Don't change the code above****************/    
    
    //Write your code here.    
if ((year / 4) % 1 === 0){
    if ((year / 100) % 1 === 0){
        if ((year / 400) % 1 === 0){
            return "Leap year."
        }else{
            return "Not leap year."
        }
    }else{
        return "Leap year."
    }
}else{
    return "Not leap year."
}
/**************Don't change the code below****************/    

}
```

## Collections: Working with Javascripts Arrays
```javascript
var eggs = [1,2,3,4,5]
var myEgg = eggs[1] // This will select the number 2 of the eggs array
eggs.length; // This counts the eggs inside the eggs array
eggs.includes(4)//This is to find out if an array includes a particular item
```
```javascript
var guestList = ["Angela", "Jack", "Pam", "James", "Lara", "Jason"];
var guestName = prompt("What is your name?")
if (guestList.includes(guestName)) {
  alert("Welcome")
} else {
  alert("Sorry maybe next time")
}
```

## Adding Elements and Intermediate Array Techniques
```
Write a program that prints the numbers from 1 to 100. But for multiples of three
print "Fizz" instead of the number and for the multiples of five print "Buzz". For numbers
wich are multiples of both three and five print "FizzBuzz"
```
```
eggs.pus()
eggs.pop
```
```javascript
//Fizz Buzz 1
var output = []
var count = 1

function fizzBuzz() {
  //Write code here.
  if (count % 3 === 0 && count % 5 ===0){
    output.push("fizz-buzz")
  }
  else if (count % 3 === 0){
    output.push("fizz")
  }
  else if (count % 5 === 0){
    output.push("buzz")
  }
  else {
    output.push(count)
  }
  count++
  
  console.log(output)
}
//Fizz Buzz 2
var output = []
var count = 1

function fizzBuzz() {
  
  if (count%3===0 && count%5===0) {
    output.push("FizzBuzz")
  } else if (count%3 === 0) {
    output.push("fizz")
  } else if (count%5 === 0) {
    output.push("buzz")
  } else {
    output.push(count)
  }
  
  console.log(output)
  count++
}

fizzBuzz()
```

## Whos buying lunch?
```javascript
function whosPaying(names) {
    
/******Don't change the code above*******/
    
    //Write your code here.
    var guest = names.length
    var random =Math.floor( Math.random()*guest)
    var payer=names[random]
    return payer + " is going to buy lunch today!"


/******Don't change the code below*******/    
}

console.log(whosPaying(["Angela","Ben", "Jenny", "Michael", "Chloe"])) //Don't forget the [] while calling the function with an array argument
```

## Control statements: While loops
```javascript
while (something is true) {
  //Do something
}
```
```javascript
var i = 1;          //i=1

while (1<2) {
  console.log(i);   //1
  i++;              //i=2
}
```
```javascript
var output = []
var count = 1

function fizzBuzz() {
  while (count <= 100) {
  if (count%3===0 && count%5===0) {
    output.push("FizzBuzz")
  } else if (count%3 === 0) {
    output.push("fizz")
  } else if (count%5 === 0) {
    output.push("buzz")
  } else {
    output.push(count)
  }
  
  console.log(output)
  count++ // Remember always put a way of ending the program, otherway it will crash becaus an infinite loop
}
}

fizzBuzz()
```
