# 10th
<!DOCTYPE html> 
<html> 
<head> 
<title>Factorial Program</title> 
</head> 
<body> 
<h2>Factorial Program</h2> 
<label for="number">Enter a number:</label> 
<input type="number" id="number"> 
<button onclick="calculateFactorial()">Calculate</button> 
<h2>Result:</h2> 
<div id="result"></div> 
<script> 
function calculateFactorial() { 
var number = parseInt(document.getElementById("number").value); 
var result = 1; 
var ch = prompt("Choose loop type:\n0. For\n1. While\n2. Do While"); 
switch (ch) { 
case "0": 
for (var i = 1; i <= number; i++) { 
result *= i; 
} 
document.getElementById("result").innerText = "The factorial of " + number + " by 
using for loop is " + result; 
break; 
case "1": 
var i = 1; 
while (i <= number) { 
result *= i; 
i++; 
} 
document.getElementById("result").innerText = "The factorial of " + number + " by 
using while loop is " + result; 
break; 
case "2": 
var i = 1; 
do { 
result *= i; 
i++; 
} while (i <= number); 
document.getElementById("result").innerText = "The factorial of " + number + " by 
using do-while loop is " + result; 
break; 
default: 
alert("Invalid choice"); 
return; 
} 
} 
</script> 
</body> 
</html> 
