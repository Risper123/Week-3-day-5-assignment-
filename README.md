Tasks:
Part 1: JavaScript Basics
Variables and Data Types:

Declare variables of different types: string, number, boolean, array, and object.
Use console.log() to print their values and types in the browser console.
Example Output:

Name: John Doe (Type: string)  
Age: 25 (Type: number)  
Is student: true (Type: boolean)  
Operators:

Write a simple calculator function that performs addition, subtraction, multiplication, and division using two numbers provided by the user (use prompt() for input).
Use arithmetic and comparison operators to validate user input and display appropriate messages.
Example Output:

Enter the first number: 10  
Enter the second number: 2  
Choose an operation (+, -, *, /): *  
Result: 20
Functions:

Create a function named greetUser that takes a name as a parameter and returns a greeting message. Display the message in an HTML element.
Part 2: JavaScript Control Structures
If Statements:

Ask the user for their age using prompt(). Use an if statement to check if they are eligible to vote (age >= 18). Display a message indicating their eligibility in an HTML element.
Loops:

Write a loop to display numbers from 1 to 10 on the webpage. Use an ordered list (<ol>) to present the numbers.
Part 3: Introduction to the DOM
Creating HTML Structure:

Add the following HTML elements to your webpage:
A heading (<h1>) with the text "JavaScript Assignment".
A paragraph (<p>) with the text "Learning JavaScript is fun!".
A <div> with an id of dynamic-content.
Selecting and Modifying HTML Elements:

Use JavaScript to:
Change the text of the <h1> element to "JavaScript in Action!".
Add a new <p> inside the dynamic-content <div> with the text "This content was added dynamically using JavaScript.".


# Week-3-day-5-assignment-
My assignment for week 3day 5
Variables and Data Types

// Declaring variables of different types
let name = "John Doe"; // string
let age = 25; // number
let isStudent = true; // boolean
let hobbies = ["reading", "coding", "hiking"]; // array
let person = { firstName: "John", lastName: "Doe" }; // object

// Displaying values and types using console.log
console.log("Name:", name, "(Type:", typeof name, ")");
console.log("Age:", age, "(Type:", typeof age, ")");
console.log("Is student:", isStudent, "(Type:", typeof isStudent, ")");
console.log("Hobbies:", hobbies, "(Type:", typeof hobbies, ")");
console.log("Person:", person, "(Type:", typeof person, ")");

Operators

// Simple calculator function
function calculator(a, b, operation) {
    let result;
    if (operation === '+') {
        result = a + b;
    } else if (operation === '-') {
        result = a - b;
    } else if (operation === '*') {
        result = a * b;
    } else if (operation === '/') {
        result = a / b;
    } else {
        return "Invalid operation!";
    }
    return result;
}

// Get user input
let num1 = parseFloat(prompt("Enter the first number:"));
let num2 = parseFloat(prompt("Enter the second number:"));
let operation = prompt("Choose an operation (+, -, *, /):");

let result = calculator(num1, num2, operation);
console.log("Result:", result

Functions

// Function to greet user
function greetUser(name) {
    return "Hello, " + name + "! Welcome to JavaScript.";
}

// Display greeting message
let greetingMessage = greetUser(prompt("Enter your name:"));
document.getElementById("dynamic-content").innerHTML = greetingMessage;


If Statements

let age = parseInt(prompt("Enter your age:"));

if (age >= 18) {
    document.getElementById("dynamic-content").innerHTML = "You are eligible to vote.";
} else {
    document.getElementById("dynamic-content").innerHTML = "You are not eligible to vote.";
}


Loops

// Display numbers from 1 to 10
let output = "<ol>";
for (let i = 1; i <= 10; i++) {
    output += "<li>" + i + "</li>";
}
output += "</ol>";
document.getElementById("dynamic-content").innerHTML += output;


Creating HTML Structure

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Assignment</title>
</head>
<body>
    <h1 id="main-heading">JavaScript Assignment</h1>
    <p>Learning JavaScript is fun!</p>
    <div id="dynamic-content"></div>

    <script src="script.js"></script>
</body>
</html>

Selecting and Modifying HTML Elements

// Changing the h1 text
document.getElementById("main-heading").innerText = "JavaScript in Action!";

// Adding a new p inside dynamic-content
let newParagraph = document.createElement("p");
newParagraph.innerText = "This content was added dynamically using JavaScript.";
document.getElementById("dynamic-content").appendChild(newParagraph);

