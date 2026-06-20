<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sorry Bunny 💐</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&family=Great+Vibes&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
}

body{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
overflow:hidden;
background:linear-gradient(135deg,#ffe6f0,#fff,#ffeaf5);
}

.container{
max-width:700px;
background:rgba(255,255,255,.92);
padding:40px;
border-radius:25px;
text-align:center;
box-shadow:0 15px 40px rgba(255,105,180,.25);
z-index:2;
}

h1{
font-family:'Great Vibes',cursive;
font-size:70px;
color:#ff4f8f;
margin-bottom:10px;
}

h2{
color:#ff6699;
margin-bottom:20px;
}

p{
font-size:18px;
line-height:1.8;
color:#555;
margin-bottom:20px;
}

button{
padding:15px 35px;
font-size:18px;
border:none;
border-radius:40px;
background:#ff4f8f;
color:white;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.08);
background:#ff1f6d;
}

#reply{
display:none;
margin-top:25px;
font-size:24px;
color:#e91e63;
font-weight:bold;
}

.flower{
position:absolute;
font-size:28px;
animation:fall linear infinite;
opacity:.9;
}

@keyframes fall{
0%{
transform:translateY(-100px) rotate(0deg);
}
100%{
transform:translateY(110vh) rotate(360deg);
}
}
</style>
</head>

<body>

<div class="container">
<h1>I'm Sorry 💐</h1>

<h2>Dear Bunny 🐰</h2>

<p>
I hope you know that I truly respect and care about you.
You are like my sister, and it hurts me knowing that I made you upset.
</p>

<p>
If my words or actions hurt you, I sincerely apologize.
It was never my intention.
Your happiness and trust mean a lot to me.
</p>

<p>
I hope you'll forgive me, and I promise to always treat you with kindness, respect, and care.
</p>

<button onclick="showMessage()">🌸 Forgive Me 🌸</button>

<div id="reply">
😊 Thank you, Bunny.<br>
You'll always be someone I respect and care about. 💖
</div>

</div>

<script>
for(let i=0;i<40;i++){
const flower=document.createElement("div");
flower.className="flower";
flower.innerHTML=["🌸","🌷","🌹","💮","🌺"][Math.floor(Math.random()*5)];
flower.style.left=Math.random()*100+"vw";
flower.style.animationDuration=(5+Math.random()*5)+"s";
flower.style.animationDelay=Math.random()*5+"s";
document.body.appendChild(flower);
}

function showMessage(){
document.getElementById("reply").style.display="block";
}
</script>

</body>
</html>
