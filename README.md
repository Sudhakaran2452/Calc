# Ex.08 Design of a Standard Calculator
## Date:29.04.2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :

```
calc.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
<center>
<h3>SUDHAKARAN S (212222220051)</h3>
</center>
<div class="calculator">
    <input type="text" id="display" readonly>
    <input type="button" value="(" onclick="addToDisplay('(')">
    <input type="button" value=")" onclick="addToDisplay(')')">
    <input type="button" value="C" onclick="clearDisplay()">
    <input type="button" value="%" onclick="addToDisplay('%')">
    <input type="button" value="7" onclick="addToDisplay('7')">
    <input type="button" value="8" onclick="addToDisplay('8')">
    <input type="button" value="9" onclick="addToDisplay('9')">
    <input type="button" value="*" onclick="addToDisplay('*')">
    <input type="button" value="4" onclick="addToDisplay('4')">
    <input type="button" value="5" onclick="addToDisplay('5')">
    <input type="button" value="6" onclick="addToDisplay('6')">
    <input type="button" value="-" onclick="addToDisplay('-')">
    <input type="button" value="1" onclick="addToDisplay('1')">
    <input type="button" value="2" onclick="addToDisplay('2')">
    <input type="button" value="3" onclick="addToDisplay('3')">
    <input type="button" value="+" onclick="addToDisplay('+')">
    <input type="button" value="0" onclick="addToDisplay('0')">
    <input type="button" value="." onclick="addToDisplay('.')">
    <input type="button" value="/" onclick="addToDisplay('/')">
    <input type="button" value="=" onclick="calculate()">
</div>

<script src="calc.js"></script>

</body>
</html>

```
```
styles.css

.calculator 
{
    width: 220px;
    margin: 0 auto;
    border: none;
    border-radius: 15px;
    padding: 10px;
    background-color: #43e013;
    display: grid;
    grid-template-columns: repeat(4, 50px);
    grid-gap: 5px;
}

input[type="button"] 
{
    width: 50px;
    padding: 10px;
    font-size: 18px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    background-color: #546d66;
    color: white;
}

input[type="text"] 
{
    grid-column: span 4;
    padding: 10px;
    font-size: 18px;
    border: 1px solid #0b0b0b;
    border-radius: 15px;
}

```
```
calc.js

function addToDisplay(value) 
{
    document.getElementById('display').value += value;
}

function calculate() 
{
    var expression = document.getElementById('display').value;
    var result = eval(expression);
    document.getElementById('display').value = result;
}

function clearDisplay() 
{
    document.getElementById('display').value = '';
}

```
## OUTPUT:

![alt text](<Screenshot 2024-04-29 132115.png>)
![alt text](<Screenshot 2024-04-29 132128.png>)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
