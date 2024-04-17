# Ex.08 Design of a Standard Calculator
## Date:

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
`````
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colorful Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f5f5f5;
        }
        .calculator {
            
            margin: 50px auto;
            width: 200px;
            height: 400px;
            border: 1px solid #ccc;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            background-color: aquamarine;

        }
        input[type="text"] {
            width: calc(100% - 20px);
            padding: 10px;
            margin-bottom: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
            font-size: 18px;
            
        }
        input[type="button"] {
            width: calc(25% - 10px);
            height: 50px;
            font-size: 18px;
            margin: 5px;
            border: none;
            border-radius: 15px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        input[type="button"]:hover {
            background-color: cadetblue;
        }
        .row {
            display: flex;
            justify-content: space-between;
        }
        .row:last-child {
            margin-top: 10px;
        }
        .result {
            background-color: #007bff;
            color: #fff;
        }
    </style>
</head>
<body>

<div class="calculator">
    <div>

    <h1 style="font-size: 30px;">Abdul Kalam </h1>
    <h2 style="font-size: 20px;">232223230003</h2>
    </div>

    <input type="text" id="display" class="result" readonly>
    <div class="row">
        <input type="button" value="7" onclick="addToDisplay('7')">
        <input type="button" value="8" onclick="addToDisplay('8')">
        <input type="button" value="9" onclick="addToDisplay('9')">
        <input type="button" value="+" onclick="addToDisplay('+')">
    </div>
    <div class="row">
        <input type="button" value="4" onclick="addToDisplay('4')">
        <input type="button" value="5" onclick="addToDisplay('5')">
        <input type="button" value="6" onclick="addToDisplay('6')">
        <input type="button" value="-" onclick="addToDisplay('-')">
    </div>
    <div class="row">
        <input type="button" value="1" onclick="addToDisplay('1')">
        <input type="button" value="2" onclick="addToDisplay('2')">
        <input type="button" value="3" onclick="addToDisplay('3')">
        <input type="button" value="*" onclick="addToDisplay('*')">
    </div>
    <div class="row">
        <input type="button" value="C" onclick="clearDisplay()">
        <input type="button" value="0" onclick="addToDisplay('0')">
        <input type="button" value="=" onclick="calculate()">
        <input type="button" value="/" onclick="addToDisplay('/')">
    </div>
</div>

<script>
    function addToDisplay(value) {
        document.getElementById('display').value += value;
    }

    function clearDisplay() {
        document.getElementById('display').value = '';
    }

    function calculate() {
        try {
            var result = eval(document.getElementById('display').value);
            document.getElementById('display').value = result;
        } catch (error) {
            document.getElementById('display').value = 'Error';
        }
    }
</script>

</body>
</html>
`````

## OUTPUT:
![image](https://github.com/dfghytr/Calc/assets/138970628/643e3bbe-201d-4c4c-b1d7-81616edd5e3f)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
