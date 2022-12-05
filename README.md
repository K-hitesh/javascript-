# javascript-
#calucalter by using java script
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="icon" href="https://cdn2.iconfinder.com/data/icons/ios7-inspired-mac-icon-set/512/Calculator_512.png">
<title>Calculator</title>
<style>
body{
background-image: url(/hand-painted-watercolor-background-with-sky-clouds-shape_24972-1095.jpg.webp);
}
input{
background-color: rgb(255, 255, 255);
color: rgb(0, 0, 0);
font-family: monospace;
border: 1px solid lime;
text-align: center;
}
div{
background-color: black;
text-align: center;
border: 1px solid white;
padding-bottom: 10px;
}
h1{
color: white;
font-family: monospace;
}
p{
color: white;
font-family: monospace;
}

</style>
</head>
<body>
<div>
<h1 id="heading">Arithmetic Calculator</h1>
<p>It calculates basic arithmetic operations</p>
<form>
<input type="text" id="bt1" placeholder="Enter first number"><br><br>
<input type="text" id="bt2" placeholder="Enter second number"><br><br>
<input type="number" id="bt3" placeholder="Result"><br><br>
<input type="button" value="Add" id="bt4" onclick="addNum()">
<input type="button" value="Subtract" id="bt4" onclick="subNum()">
<input type="button" value="Multiply" id="bt5" onclick="mulNum()">
<input type="button" value="Divide" id="bt6" onclick="divNum()">
<input type="button" value="Modulus" id="bt7" onclick="modNum()">
<input type="reset">
<hr>

</form>
<script>
function addNum()
{let no1 = parseInt(document.getElementById('bt1').value);
let no2 = parseInt(document.getElementById('bt2').value);
let no3 = no1+no2;
document.getElementById('bt3').value = no3;
}

function subNum()
{let no1 = parseInt(document.getElementById('bt1').value);
let no2 = parseInt(document.getElementById('bt2').value);
let no3 = no1-no2;
document.getElementById('bt3').value = no3;
}

function mulNum()
{let no1 = parseInt(document.getElementById('bt1').value);
let no2 = parseInt(document.getElementById('bt2').value);
let no3 = no1*no2;
document.getElementById('bt3').value = no3;
}

function divNum()
{let no1 = parseInt(document.getElementById('bt1').value);
let no2 = parseInt(document.getElementById('bt2').value);
let no3 = no1/no2;
document.getElementById('bt3').value = no3;
}

function modNum()
{let no1 = parseInt(document.getElementById('bt1').value);
let no2 = parseInt(document.getElementById('bt2').value);
let no3 = no1%no2;
document.getElementById('bt3').value = no3;
}
function ageCheck(){
let x = document.getElementById('btage').value;
if(x>=18){
alert('Congratulations! You are eligible to vote')

}
else{
alert('Sorry you are ineligible to vote')
}


}
function day(){
let y = document.getElementById('week1'.value);
if(y=1){
document.getElementById('week-day-display').innerText='It is a Monday'
}
else if(y=2){
document.getElementById('week-day-display').innerText='It is a Tuesday'
}
else if(y=3){
document.getElementById('week-day-display').innerText='It is a Wednesday'
}
else if(y=4){
document.getElementById('week-day-display').innerText='It is a Thursday'
}
else if(y=5){
document.getElementById('week-day-display').innerText='It is a Friday'
}
else if(y=6){
document.getElementById('week-day-display').innerText='It is a Saturday'
}
else{
document.getElementById('week-day-display').innerText='It is a Sunday'
}

}



</script>
</div>

<div class="eligibility-calculator">
<h1>Eligibilty Calculator</h1>
<p>It calculates whether you are eligible to vote or not</p>
<input type="text" id="btage" placeholder="Enter your age"><br><br>
<input id="btage1"type="button" value="Check Eligibility" onclick="ageCheck()" >

</div>
<div>
<h1>Week Day Calculator</h1>
<p id="week-day-display">It calculates the week of the day!</p>
<input type="text" id="week1" placeholder="Enter the number of weekday"><br><br>
<input type="button" onclick="day()" value="Check Day">
</div>
</body>
</html>



#output
design calculator as we use in daily life(casino)
