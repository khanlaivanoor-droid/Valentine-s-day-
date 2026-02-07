
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For You ❤️</title>

<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Poppins&display=swap" rel="stylesheet">

<style>
body{
margin:0;
font-family:'Poppins',sans-serif;
background:linear-gradient(to bottom,#ffe6f0,#e6f7ff);
text-align:center;
overflow-x:hidden;
}

h1,h2{
font-family:'Dancing Script',cursive;
color:#ff6fa5;
}

section{
padding:60px 20px;
}

button{
padding:12px 20px;
border:none;
border-radius:20px;
background:#ffb6d9;
cursor:pointer;
font-size:16px;
transition:0.3s;
}

button:hover{
background:#ff8cc4;
transform:scale(1.1);
}

/* Floating Hearts */
.heart{
position:fixed;
color:pink;
animation:float 6s infinite;
}

@keyframes float{
0%{transform:translateY(100vh);}
100%{transform:translateY(-10vh);}
}

/* Music Cards */
.song{
background:white;
margin:10px auto;
padding:15px;
width:250px;
border-radius:15px;
box-shadow:0 0 10px rgba(0,0,0,0.1);
transition:0.3s;
}

.song:hover{
transform:scale(1.05);
}

/* Surprise box */
.box{
font-size:80px;
cursor:pointer;
}

/* Hidden Letter */
#letter{
display:none;
background:white;
padding:20px;
border-radius:20px;
max-width:500px;
margin:auto;
box-shadow:0 0 10px rgba(0,0,0,0.2);
}

/* Gallery */
img{
width:200px;
border-radius:15px;
margin:10px;
transition:0.3s;
}

img:hover{
transform:scale(1.1);
}

/* Countdown */
#countdown{
font-size:24px;
color:#ff6fa5;
}
</style>
</head>

<body>

<!-- Floating Hearts Script -->
<script>
setInterval(()=>{
let heart=document.createElement("div");
heart.innerHTML="❤️";
heart.className="heart";
heart.style.left=Math.random()*100+"vw";
document.body.appendChild(heart);
setTimeout(()=>heart.remove(),6000);
},500);
</script>

<!-- Landing Page -->
<section>
<h1>To The One Who Holds My Heart ❤️</h1>
<p>
Distance may keep us apart physically, but my heart finds its home in you every single day. 
This little website is a piece of my love, wrapped in memories, songs, and feelings that remind me of you.
</p>
<a href="#story"><button>Start Journey</button></a>
</section>

<!-- Love Story -->
<section id="story">
<h2>Our Love Story</h2>
<p>
We met online, through a mutual friend. I texted you first with a simple "heyyyy"... 
and somehow that small message turned into something beautiful.  
Every conversation made me smile, every late night talk made me fall deeper.
Even though distance separates us, it has only made our bond stronger.
</p>
</section>

<!-- Music Section -->
<section>
<h2>Songs That Reminds Me Of You 🎵</h2>

<div class="song">
<p>Can't Help Falling In Love</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/vGJTaP6anOU"></iframe>
</div>

<div class="song">
<p>Maula Mere Maula</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/3qjJk3zK8yM"></iframe>
</div>

<div class="song">
<p>Kiss Me Like It's The First Time</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/2Vv-BfVoq4g"></iframe>
</div>

<div class="song">
<p>Tum Ho</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/MT0hV6QyJm8"></iframe>
</div>

<div class="song">
<p>Apocalypse</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/sElE_BfQ67s"></iframe>
</div>

<div class="song">
<p>Ruposh</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/0zG1r5nM5nY"></iframe>
</div>

<div class="song">
<p>You're All I Want</p>
<iframe width="220" height="120" src="https://open.spotify.com/track/2cTvZSCqzjkTMkIypLxUFH?si=nsy-NC8IT_GcXtvnk9JP-Q"></iframe>
</div>

<div class="song">
<p>Tu Hi Mera</p>
<iframe width="220" height="120" src="https://www.youtube.com/embed/J0kYvK0Q6PQ"></iframe>
</div>

</section>

<!-- Surprise Box -->
<section>
<h2>Click The Surprise 🎁</h2>

<div class="box" onclick="openLetter()">🎁</div>

<div id="letter">
<h3>My Love Letter 💌</h3>
<p>
You are my comfort, my happiness, and my favorite person in the entire world.
No distance can change how deeply I care about you.
I cannot wait for the day when miles turn into hugs.
</p>
</div>

</section>

<!-- Gallery -->
<section>
<h2>Photo Memories 📸</h2>
<p>(You can replace these with your photos later)</p>

<img src="https://via.placeholder.com/200">
<img src="https://via.placeholder.com/200">
<img src="https://via.placeholder.com/200">

</section>

<!-- Poetry -->
<section>
<h2>Poetry For You 🖋️</h2>
<p>
If distance had a sound, it would whisper your name.  
If love had a color, it would paint your smile.  
Across miles, my heart still finds its way to you.
</p>
</section>

<!-- Countdown -->
<section>
<h2>Counting Until Our 5th Month ❤️</h2>
<div id="countdown"></div>
</section>

<!-- Ending -->
<section>
<h2>Forever Yours 🌷</h2>
<p>
Thank you for being part of my life.  
This is only one chapter of our story… and I cannot wait to write the rest with you.
</p>
</section>

<script>
function openLetter(){
document.getElementById("letter").style.display="block";
}

/* Countdown */
const target=new Date("Feb 18, 2026 00:00:00").getTime();

setInterval(()=>{
let now=new Date().getTime();
let diff=target-now;

let d=Math.floor(diff/(1000*60*60*24));
let h=Math.floor((diff%(1000*60*60*24))/(1000*60*60));
let m=Math.floor((diff%(1000*60*60))/(1000*60));
let s=Math.floor((diff%(1000*60))/1000);

document.getElementById("countdown").innerHTML=
d+" Days "+h+" Hours "+m+" Minutes "+s+" Seconds";
},1000);
</script>

</body>
</html>