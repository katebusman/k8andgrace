<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title> Jonny Boy </title>
<style>
body{background-color:lightskyblue}
#quiz{text-align:center}
#test{text-align:center}
.head{text-align:center;
font-family:comic sans ms}
.button{background-color:#FFB6C1;
border-radius:12px;
border:2px dashed lightcoral;
color:mediumvioletred}
table,tr,td,th{border:2px solid mediumvioletred}
#twilightGif{display: none;
margin-top: 30px;
max-width: 80%;
border: 4px dashed purple;
border-radius: 15px;
box-shadow: 0 0 20px magenta}
.rob {padding: 14px 28px;
font-size: 18px;
background-color: orchid;
border: 2px solid black;
border-radius: 12px;
cursor: pointer;
transition: all 0.3s ease}
.rob:hover {background-color: pink;
transform: scale(1.05)}
.ed{display:flex}
#amazing{margin:auto;
text-align:center}
</style>
</head>
<body onload="checkPassword()">
<p class="head" onclick="showQuiz()"> Click Here to Take a Quiz about the Beautiful Kate Nicole Busman </p>
<div id="quiz">
</div>
<p class="head" onclick="showGrace()"> Click Here to Take a Quiz about the Gorgeous Grace Elizabeth Campbell </p>
<div id="test">
</div>
<table style="margin:auto">
<tr>
<th colspan="2" style="font-family:comic sans MS, cursive"> Click on the images of Kate and Grace to see their furry friends</th>
</tr>
<td>
<img src="goggles.jpg" alt="Kate with goggles on" id="goggles" height="300" width="300" onclick="swapKate()">
</td>
<td>
<img src="grace_1D.jpeg" alt="Grace with 1D Shrine" id="one" height="300" width="350" onclick="swapGrape()">
</td>
</tr>
</table>
<br><br><br>
<div id="amazing">
<h1 style="text-align:center"> Summon the Power of Edward Cullen </h1>
<button class="rob" onclick="sparkleTime()">Click for Sparkle</button>
</div>
<br><br>
<div class="ed">
<img id="twilightGif" src="twilight.gif" alt="Edward Cullen Sparkle Time">
</div>
<script>
function checkPassword() 
{
	var password = prompt("Enter the secret password:");
	if (password !== "bella hadid") {
	alert("WRONG! Access denied.");
	document.body.innerHTML = "<h2 style='text-align:center;'>Unauthorized Access</h2>";
	}
}
function showQuiz()
{
	document.getElementById("quiz").innerHTML=`
	<p> 1. What is Kate's favorite color?</p>
	<input type="radio" name="cool" id="q1a"> A. Yellow<br>
	<input type="radio" name="cool" id="q1b"> B. Green<br>
	<input type="radio" name="cool" id="q1c"> C. Black<br>
	<input type="radio" name="cool" id="q1d"> D. Blue<br>
	<input type="radio" name="cool" id="q1e"> E. Pink<br>

	<p> 2. What kind of car was Kate's first car?</p>
	<input type="radio" name="bean" id="q2a"> A. Subaru Forester<br>
	<input type="radio" name="bean" id="q2b"> B. Subaru WRX STI<br>
	<input type="radio" name="bean" id="q2c"> C. Subaru Outback<br>
	<input type="radio" name="bean" id="q2d"> D. Subaru BRZ<br>

	<p> 3. What was Kate's favorite show when she was a child? </p>
	<input type="radio" name="toast" id="q3a"> A. Doc McStuffins<br>
	<input type="radio" name="toast" id="q3b"> B. Mickey Mouse Clubhouse<br>
	<input type="radio" name="toast" id="q3c"> C. Wonder Pets <br>
	<input type="radio" name="toast" id="q3d"> D. Dora the Explorer<br>
	
	<p> 4. How old was Kate when she broke her ankle the first time? </p>
	<input type="radio" name="rob" id="q4a"> A. 12 years old <br>
	<input type="radio" name="rob" id="q4b"> B. 13 years old <br>
	<input type="radio" name="rob" id="q4c"> C. 7 years old <br>
	<input type="radio" name="rob" id="q4d"> D. 8 years old <br>

	<p> 5. Aside from Robert Pattinson, who is Kate's biggest celebrity crush? </p>
	<input type="radio" name="pore" id="q5a"> A. Zac Efron<br>
	<input type="radio" name="pore" id="q5b"> B. Michael B. Jordan<br>
	<input type="radio" name="pore" id="q5c"> C. Pedro Pascal<br>
	<input type="radio" name="pore" id="q5d"> D. Jacob Elordi<br><br>
	
	<input type="button" value="Submit" class="button" onclick="calculateScore()">`;
}

function calculateScore()
{
	var score=0;

	//Question 1 - C
	if(document.getElementById("q1c").checked)
	{
		score+=20;
	}

	//Question 2 - C

	if(document.getElementById("q2c").checked)
	{
		score+=20;
	}

	//Question 3 - A
	if(document.getElementById("q3a").checked)
	{
		score+=20;
	}

	//Question 4 - A
	if(document.getElementById("q4a").checked)
	{
		score+=20;
	}

	//Question 5 - D
	if(document.getElementById("q5d").checked)
	{
		score+=20;
	}

	alert("Your score is: " + score + "/100");
}

function showGrace()
{
	document.getElementById("test").innerHTML=`
	<p> 1. What was the primary name of Grace's most beloved guinea  pig?</p>
	<input type="radio" name="thank" id="t1a"> A. Pants<br>
	<input type="radio" name="thank" id="t1b"> B. Colin<br>
	<input type="radio" name="thank" id="t1c"> C. Lala<br>
	<input type="radio" name="thank" id="t1d"> D. Bangs<br>
	<input type="radio" name="thank" id="t1e"> E. Rooster<br>

	<p> 2. In what grade did Grace stop learning math?</p>
	<input type="radio" name="math" id="t2a"> A. First Grade<br>
	<input type="radio" name="math" id="t2b"> B. Fourth Grade<br>
	<input type="radio" name="math" id="t2c"> C. Third Grade<br>
	<input type="radio" name="math" id="t2d"> D. Fifth Grade<br>

	<p> 3. Who is Grace's least favorite of all of the following people? </p>
	<input type="radio" name="ppl" id="t3a"> A. Jayde Irlbeck<br>
	<input type="radio" name="ppl" id="t3b"> B. Alivia Vasil<br>
	<input type="radio" name="ppl" id="t3c"> C. Hinano Tomlinson <br>
	<input type="radio" name="ppl" id="t3d"> D. Angie (Lucas)<br>
	
	<p> 4. Who was Grace's first crush? </p>
	<input type="radio" name="jm" id="t4a"> A. J.M. Berry <br>
	<input type="radio" name="jm" id="t4b"> B. Andy Kuipers <br>
	<input type="radio" name="jm" id="t4c"> C. Jacob Abell <br>
	<input type="radio" name="jm" id="t4d"> D. Logan Elliott <br>

	<p> 5. What has Grace nicknamed her car? </p>
	<input type="radio" name="car" id="t5a"> A. Little Slut<br>
	<input type="radio" name="car" id="t5b"> B. Trashcan<br>
	<input type="radio" name="car" id="t5c"> C. Sandy<br>
	<input type="radio" name="car" id="t5d"> D. Mutt<br><br>
	
	<input type="button" value="Submit" class="button" onclick="calculateGrade()">`;
}

function calculateGrade()
{
	var score=0;

	//Question 1 - C
	if(document.getElementById("t1c").checked)
	{
		score+=20;
	}

	//Question 2 - C

	if(document.getElementById("t2c").checked)
	{
		score+=20;
	}

	//Question 3 - A
	if(document.getElementById("t3a").checked)
	{
		score+=20;
	}

	//Question 4 - A
	if(document.getElementById("t4a").checked)
	{
		score+=20;
	}

	//Question 5 - D
	if(document.getElementById("t5d").checked)
	{
		score+=20;
	}

	alert("Your score is: " + score + "/100");
}

function swapKate()
{
	var img=document.getElementById("goggles");
	img.src="subear.jpg";
	img.style.width="300px";
	img.style.height="500px";
}

function swapGrape()
{
	var img=document.getElementById("one");
	img.src="pigs.jpeg";
	img.style.width="400px";
	img.style.width="300px";
}

function sparkleTime()
{
	document.body.style.backgroundColor="hotpink";
	document.getElementById("twilightGif").style.display="block";
}	
</script>
</body>
</html>
