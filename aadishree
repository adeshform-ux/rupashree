```html id="cinematic-pro"
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>For You ❤️</title>
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>

*{margin:0;padding:0;box-sizing:border-box;}

body{
font-family: 'Segoe UI', sans-serif;
background:black;
color:white;
overflow:hidden;
}

/* screens */

.screen{
position:absolute;
width:100%;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
transition:1.2s;
}

.hidden{
opacity:0;
pointer-events:none;
}

/* video */

video{
position:absolute;
width:100%;
height:100%;
object-fit:cover;
z-index:-2;
}

/* dark overlay */

.overlay{
position:absolute;
width:100%;
height:100%;
background:rgba(0,0,0,0.5);
z-index:-1;
}

/* glass card */

.card{
backdrop-filter:blur(15px);
background:rgba(255,255,255,0.1);
padding:30px;
border-radius:20px;
max-width:420px;
text-align:center;
box-shadow:0 10px 40px rgba(0,0,0,0.5);
transition:0.3s;
}

.card:hover{
transform:scale(1.05) rotateX(5deg);
}

/* buttons */

button{
padding:12px 25px;
border:none;
border-radius:30px;
background:linear-gradient(45deg,#ff4d6d,#ff758c);
color:white;
font-size:18px;
margin-top:15px;
cursor:pointer;
transition:0.3s;
}

button:hover{
transform:scale(1.1);
}

/* cinematic text */

.big-text{
font-size:40px;
letter-spacing:2px;
animation:fadeIn 3s;
}

@keyframes fadeIn{
from{opacity:0; transform:translateY(40px);}
to{opacity:1;}
}

/* particles */

.particle{
position:absolute;
font-size:20px;
animation:float 10s linear infinite;
}

@keyframes float{
0%{transform:translateY(100vh);}
100%{transform:translateY(-10vh);}
}

#typing{
min-height:80px;
font-size:18px;
}

</style>
</head>

<body>

<!-- MUSIC -->
<audio autoplay loop>
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3">
</audio>

<!-- INTRO -->

<div class="screen" id="intro">

<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4">
</video>

<div class="overlay"></div>

<div class="big-text">
💭 I Need To Tell You Something...
</div>

<button onclick="next('story')">Start ❤️</button>

</div>

<!-- STORY -->

<div class="screen hidden" id="story">

<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4">
</video>

<div class="overlay"></div>

<div class="card">

<h1>I'm Sorry 💔</h1>

<p id="typing"></p>

<button onclick="next('letter')">Continue 💌</button>

</div>

</div>

<!-- LETTER -->

<div class="screen hidden" id="letter">

<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4">
</video>

<div class="overlay"></div>

<div class="card">

<h2>💌 From My Heart</h2>

<p>
I know I irritated you 😅  
But I never meant to hurt you 🥺  
You are very important to me ❤️  
And I miss your smile every day 😊  
</p>

<button onclick="next('question')">One Last Thing... 🥺</button>

</div>

</div>

<!-- QUESTION -->

<div class="screen hidden" id="question">

<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4">
</video>

<div class="overlay"></div>

<div class="card">

<h2>🥺 Will You Forgive Me?</h2>

<button onclick="next('final')">Yes ❤️</button>
<button id="noBtn" onmouseover="moveNo()">No 😤</button>

</div>

</div>

<!-- FINAL -->

<div class="screen hidden" id="final">

<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4">
</video>

<div class="overlay"></div>

<div class="card">

<h1>💍 Thank You ❤️</h1>

<p>
You mean everything to me ❤️  
I promise I’ll be better...  
But I’ll always love you more 💖  
</p>

</div>

</div>

<script>

/* navigation */

function next(id){
document.querySelectorAll(".screen").forEach(s=>s.classList.add("hidden"))
document.getElementById(id).classList.remove("hidden")
}

/* typing */

let text="I know I irritated you... 😅 But I never wanted to hurt you 🥺 You mean everything to me ❤️"

let i=0

function type(){
if(i<text.length){
document.getElementById("typing").innerHTML+=text.charAt(i)
i++
setTimeout(type,40)
}
}

setTimeout(type,1500)

/* no button */

function moveNo(){
let btn=document.getElementById("noBtn")
btn.style.position="absolute"
btn.style.left=Math.random()*80+"vw"
btn.style.top=Math.random()*80+"vh"
}

/* particles */

let emojis=["✨","💖","❤️","🌸"]

setInterval(()=>{

let p=document.createElement("div")
p.className="particle"
p.innerHTML=emojis[Math.floor(Math.random()*emojis.length)]
p.style.left=Math.random()*100+"vw"

document.body.appendChild(p)

setTimeout(()=>p.remove(),10000)

},300)

</script>

</body>
</html>
```
<source src="https://www.w3schools.com/howto/rain.mp4">
<source src="your-video.mp4">
SoundHelix-Song-2.mp3
