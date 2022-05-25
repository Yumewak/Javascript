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
```javascript
    var numberOfBottles = 99
    while (numberOfBottles >= 0) {
        var bottleWord = "bottles";
        if (numberOfBottles <= 1) {
            bottleWord = "bottle";
        } 
        console.log(numberOfBottles + " " + bottleWord + " of beer on the wall");
        console.log(numberOfBottles + " " + bottleWord + " of beer,");
        console.log("Take one down, pass it around,");
    	numberOfBottles--;
        console.log(numberOfBottles + " " + bottleWord + " of beer on the wall.");
    }
    
-------------------------------------------------------------------------------------------------------
var bottles = 5
while (bottles > 1) {
  console.log(bottles + " bottles of beer on the wall, " + bottles + " bottles of beer. Take one down and pass it around, " + (bottles-1) + "bottles of beer on the wall")
  bottles--
}
console.log("1 bottle of beer on the wall, 1 bottle of beer. Take one down and pass it around, no more bottles of beer on the wall")
console.log("No more bottles of beer on the wall, no more bottles of beer. Go to the store and buy some more, 99 bottles of beer on the wall")
---------------------------------------------------------------------------------------------------------
var count = 9;

function beer() {
    while (count > 1) {
        var bottleWord = "bottles"
        console.log(count + " " + bottleWord + " of beer on the wall, " + count + " " + bottleWord + " of beer.")
        if (count === 2){
            bottleWord = "bottle"
        }
        count --
        console.log("Take one down and pass it around, " + count + " " + bottleWord + " of beer on the wall.")
    }
    console.log("1 bottle of beer on the wall, 1 bottle of beer. Take one down and pass it around, no more bottles of beer on the wall.")
    console.log("No more bottles of beer on the wall, no more bottles of beer. Go to the store and buy some more, 99 bottles of beer on the wall.")
}

beer()
```

## Control statements: For loops
```javascript
for (i=0; 1<2; i++) {
//Do something
}
```
```javascript
Difference between While and For
//While loop: checking for a state, so it's while something is true
var i = 1;
while(i<2){
  console.log(i);
  i++;
}
-------------------------------------
//For loop: Trying to iterate, run a piece of code many times
for (i=1; i<2; i++) {
  console.log(i);
}

```
```javascript
var output = [];
function fizzBuzz() {
    for (var i=1; i<100; i++) {
        if (i % 3 === 0 && i % 5 === 0) {
            output.push("Fizz-Buzz");
        } else if (i % 3 === 0) {
            output.push("Fizz");
        } else if (i % 5 === 0) {
            output.push("Buzz");
        } else {
            output.push(i);
        }
    }
    return output;
}
fizzBuzz();
```

## Adding Javascript to websites
```html
//Inline Javascript
<body onload="alert('Hello')">

//Internal Javascript
    <script type="text/javascript">
        alert(`"Hello"`);
    </script>
  
//External Javascript
<script src="./index.js"></script>
  //index.js
  alert("hello");
```

## Introduction to the Document Object Model
```html
<html lang="en">
<head>
    <title>My Website</title>
</head>
<body>
    <button>Alert</button>
</body>
</html>
```
![Sin título](https://user-images.githubusercontent.com/93165649/151464612-50654f1c-b890-40e7-b668-1660722239ef.png)
![16g5gfert](https://user-images.githubusercontent.com/93165649/151465209-5f24c04d-e73c-478b-bff2-8fe82563d382.png)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Website</title>
    <link rel="stylesheet" href="./styles.css">
</head>
<body>
    <h1>Hello </h1>

    <input type="checkbox">

    <button style=":active: color:red;">ClickMe</button>
    <ul>
        <li class="list">
            <a href="https://www.google.com">Google</a>
        </li>
        <li class="list">Second</li>
        <li class="list">Third</li>
    </ul>

    <script src="./index.js"></script>
</body>
</html>
```
```javascript
document.firstElementChild.lastElementChild.firstElementChild //This will select the "<h1>Hello</h1>" tag thats inside the body
var heading = document.firstElementChild.lastElementChild.firstElementChild // This will save it inside the variable "heading" the DOM line of code
heading.innerHTML = "Good Bye" // This modify the innerHTML of the heading
heading.style.color = "red" // Changes the text color of the element that is selected to red
document.querySelector("input").click() // This looks inside our entire document for the object that has the selector of "input" and call a method "click". click simulates a mouse click
```
```
The objects inside the DOM can have properties and methods
Properties: Describe something about the object
.innerHTML
.style
.firstChild

Methods: Are the things that the object can do
click()
appendChild()
setAttribute()

car.color; //get the value of the property         "Get Property
car.numberOfDoors = 0; // set the number of doors  "Set Property" 
car.drive (); // call the method drive             "Call Method"
```
```javascript
//Diferent ways of change a text
document.getElementsByTagName("li").item(2).innerHTML = "Mario"
document.getElementsByTagName("li")[2].innerHTML = "Ulrich"
document.querySelector("ul").lastElementChild.innerHTML = "Ashley"
```

## Selecting HTML Elements with Javascript
```javascript
document.getElementsByTagName("li")[2].style.color = "purple" // It searches for the element with a particular tag name, the result is an array

document.getElementsByTagName("li").length // length property tell how many items are in the array

document.getElementsByClassName("btn")[0] // Returns an array of element with a particular class name

document.getElementById("title").innerHTML = "Good Bye" // Using this method you only get back one item instead of an array

document.querySelector("") // Only returns a single item, the string inside the parentheses is a selector
("body")
(".navbar")
("#title")
//With selectors we can combine different things, for example an id with a class, or a class with an element
document.querySelector("li a")
document.querySelector("li.item") // When you're combining selectors that occur in the same element there are no spaces

document.querySelectorAll("#list .item")[2] //Return an array with all of the objects that match that selector
```

## Manipulating and Changing Styles of HTML Elements with Javascript
```javascript
// Every singles CSS property can be changed in this way using Javascript, but the property names might look different
document.querySelector("h1").style.color = "red" 
//Javascript naming conventions tend to be camel cased, and the values have to be represented as strings
document.querySelector("h1").style.fontSize = "10rem"
```
[HTML DOM Style Object](https://www.w3schools.com/jsref/dom_obj_style.asp)

## The separation of concerns: Structure vs Style vs Behaviour
```javascript
//Class list
//The add method can use to add classes to the "classList"
document.querySelector("button").classList.add("invisible")
document.querySelector("button").classList.remove("invisible")
document.querySelector("button").classList.toggle("invisible")
```

## Text Manipulation and the Text Content Property
```javascript
// Gives you the HTML that's in between the element tags, you can also add HTML code on the fly
document.querySelector("h1").innerHTML = "<em>Good Bye</em>"
//Just show you the text
document.getElementById("title").textContent = "GoodBye"
```

## Manupulating HTML element attributes
```javascript
// Get the list of attributes
document.querySelector("a").attributes;
// Retrieve the current value of that attribute
document.querySelector("a").getAttribute("href")
// Change the attirbute
document.querySelector("a").setAttribute("href", "https://www.bing.com")
```
