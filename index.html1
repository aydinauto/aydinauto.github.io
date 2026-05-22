
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AYDIN AUTO</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700;900&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:#050505;
color:white;
overflow-x:hidden;
}

/* LOADER */

#loader{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:black;
display:flex;
align-items:center;
justify-content:center;
flex-direction:column;
z-index:999999;
animation:loaderOut 1s forwards;
animation-delay:4s;
}

#loader h1{
font-size:55px;
font-weight:900;
letter-spacing:4px;
animation:pulse 1s infinite;
}

#loader p{
margin-top:15px;
opacity:.8;
}

@keyframes pulse{
0%{transform:scale(1);}
50%{transform:scale(1.1);}
100%{transform:scale(1);}
}

@keyframes loaderOut{
to{
opacity:0;
visibility:hidden;
}
}

/* CONFETTI */

.confetti{
position:fixed;
width:10px;
height:10px;
background:red;
top:-10px;
animation:fall linear forwards;
z-index:99999;
}

@keyframes fall{
to{
transform:translateY(110vh) rotate(720deg);
opacity:0;
}
}

/* NAVBAR */

nav{
position:fixed;
top:0;
left:0;
width:100%;
padding:18px 25px;
display:flex;
justify-content:space-between;
align-items:center;
backdrop-filter:blur(12px);
background:rgba(0,0,0,.5);
z-index:999;
border-bottom:1px solid rgba(255,255,255,.08);
}

.logo{
font-size:32px;
font-weight:900;
}

.menu-btn{
font-size:35px;
cursor:pointer;
}

/* MENU */

#menu{
position:fixed;
top:0;
right:-100%;
width:80%;
height:100%;
background:#0d0d0d;
z-index:99999;
transition:.5s;
padding:90px 30px;
}

#menu.active{
right:0;
}

.close-btn{
position:absolute;
top:20px;
right:25px;
font-size:40px;
cursor:pointer;
}

#menu a{
display:block;
margin:25px 0;
font-size:28px;
color:white;
text-decoration:none;
}

/* HERO */

.hero{
height:100vh;
background:
linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.8)),
url('35C20A1F-C4C5-4C2D-AE1C-BB8B82E47414.png');
background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
position:relative;
overflow:hidden;
}

.hero::after{
content:'';
position:absolute;
width:500px;
height:500px;
background:#ffd70022;
filter:blur(120px);
border-radius:50%;
animation:float 6s infinite alternate;
}

@keyframes float{
from{transform:translate(-100px,-50px);}
to{transform:translate(100px,50px);}
}

.hero-content{
position:relative;
z-index:2;
}

.hero h1{
font-size:70px;
font-weight:900;
line-height:1;
margin-bottom:20px;
}

.hero p{
font-size:20px;
opacity:.9;
margin-bottom:35px;
}

.hero button{
padding:18px 35px;
border:none;
border-radius:15px;
font-size:18px;
font-weight:700;
margin:10px;
cursor:pointer;
transition:.3s;
}

.btn1{
background:white;
color:black;
}

.btn2{
background:#ffd700;
color:black;
}

.hero button:hover{
transform:scale(1.05);
}

/* LANGUAGE */

.lang{
position:absolute;
top:100px;
right:20px;
display:flex;
gap:10px;
z-index:3;
}

.lang button{
padding:10px 16px;
border:none;
border-radius:10px;
background:#151515;
color:white;
font-weight:700;
}

/* STATS */

.stats{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:20px;
padding:40px 20px;
}

.stat{
background:#111;
padding:30px;
border-radius:25px;
text-align:center;
border:1px solid rgba(255,255,255,.06);
}

.stat h2{
font-size:45px;
color:#ffd700;
}

/* CARS */

.section-title{
font-size:45px;
font-weight:900;
padding:20px;
}

.cars{
padding:20px;
display:flex;
flex-direction:column;
gap:35px;
}

.car{
background:#0f0f0f;
border-radius:35px;
overflow:hidden;
box-shadow:0 0 40px rgba(255,255,255,.04);
transition:.4s;
}

.car:hover{
transform:translateY(-10px);
}

.car img{
width:100%;
height:300px;
object-fit:cover;
}

.car-content{
padding:25px;
}

.car-content h2{
font-size:40px;
margin-bottom:15px;
}

.car-content p{
opacity:.8;
line-height:1.7;
}

/* VIDEO */

.video-section{
padding:20px;
}

.video-section video{
width:100%;
border-radius:30px;
}

/* TAKAS */

.trade{
padding:20px;
}

.trade-box{
background:#101010;
padding:30px;
border-radius:30px;
}

.trade input,
.trade select{
width:100%;
padding:18px;
margin:12px 0;
background:#181818;
border:none;
border-radius:15px;
color:white;
font-size:17px;
}

.trade button{
width:100%;
padding:18px;
border:none;
border-radius:15px;
background:#ffd700;
font-weight:700;
font-size:18px;
margin-top:10px;
}

#priceResult{
margin-top:20px;
font-size:25px;
font-weight:700;
color:#ffd700;
}

/* AI CHAT */

.ai{
padding:20px;
}

.ai-box{
background:#0f0f0f;
padding:25px;
border-radius:30px;
}

.chat{
height:300px;
overflow:auto;
background:#111;
padding:15px;
border-radius:15px;
margin-bottom:15px;
}

.msg{
background:#1a1a1a;
padding:12px;
border-radius:12px;
margin:10px 0;
}

.ai input{
width:100%;
padding:18px;
border:none;
border-radius:15px;
background:#181818;
color:white;
}

.ai button{
width:100%;
padding:16px;
margin-top:12px;
background:#ffd700;
border:none;
border-radius:15px;
font-weight:700;
}

/* CONTACT */

.contact{
padding:20px;
}

.contact-box{
background:#101010;
padding:30px;
border-radius:30px;
}

.contact-item{
margin:20px 0;
font-size:20px;
}

/* MAP */

iframe{
width:100%;
height:300px;
border:none;
border-radius:30px;
margin-top:20px;
}

/* WHATSAPP */

.whatsapp{
position:fixed;
bottom:25px;
right:25px;
width:70px;
height:70px;
background:#25D366;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
font-size:35px;
z-index:999;
box-shadow:0 0 30px #25D366;
animation:bounce 1.5s infinite;
}

@keyframes bounce{
0%{transform:translateY(0);}
50%{transform:translateY(-10px);}
100%{transform:translateY(0);}
}

/* REVIEWS */

.reviews{
padding:20px;
display:flex;
flex-direction:column;
gap:20px;
}

.review{
background:#101010;
padding:25px;
border-radius:25px;
}

/* FOOTER */

footer{
padding:50px 20px;
text-align:center;
opacity:.7;
}

/* PARTICLES */

.particle{
position:fixed;
width:4px;
height:4px;
background:white;
border-radius:50%;
opacity:.3;
animation:particleMove linear infinite;
}

@keyframes particleMove{
from{
transform:translateY(100vh);
}
to{
transform:translateY(-100vh);
}
}

</style>
</head>

<body>

<div id="loader">
<h1>AYDIN AUTO</h1>
<p>PREMIUM EXPERIENCE</p>
</div>

<nav>
<div class="logo">AYDIN AUTO</div>
<div class="menu-btn" onclick="openMenu()">☰</div>
</nav>

<div id="menu">
<div class="close-btn" onclick="closeMenu()">✕</div>

<a href="#">Ana Sayfa</a>
<a href="#cars">Araçlarımız</a>
<a href="#trade">Takas</a>
<a href="#ai">AI Destek</a>
<a href="#contact">İletişim</a>
<a href="https://instagram.com/aydinautoresmi">Instagram</a>
</div>

<section class="hero">

<div class="lang">
<button>TR</button>
<button>EN</button>
<button>AR</button>
</div>

<div class="hero-content">
<h1>AYDIN AUTO</h1>
<p>Premium otomobil deneyimi.</p>

<button class="btn1">Araçlarımız</button>
<button class="btn2">İletişim</button>
</div>

</section>

<section class="stats">

<div class="stat">
<h2>500+</h2>
<p>Satılan Araç</p>
</div>

<div class="stat">
<h2>4.9★</h2>
<p>Müşteri Puanı</p>
</div>

<div class="stat">
<h2>24/7</h2>
<p>Destek</p>
</div>

<div class="stat">
<h2>12+</h2>
<p>Premium Marka</p>
</div>

</section>

<h1 class="section-title">Araçlarımız</h1>

<section class="cars" id="cars">

<div class="car">
<img src="02F96023-A74D-4FDE-A4A1-1C2C9EDD6195.jpeg">
<div class="car-content">
<h2>Lamborghini Urus</h2>
<p>Süper spor ruhunu SUV dünyasına taşıyan canavar.</p>
</div>
</div>

<div class="car">
<img src="1E77547B-A49D-4769-8CE2-CE3C2ECC6960.jpeg">
<div class="car-content">
<h2>Mercedes G63 AMG</h2>
<p>Agresif görünüm ve gerçek AMG ruhu.</p>
</div>
</div>

<div class="car">
<img src="062B7BCA-316E-49EE-AC93-179B9EC6AC71.png">
<div class="car-content">
<h2>Porsche Cayenne</h2>
<p>Üst düzey konfor ve premium sürüş deneyimi.</p>
</div>
</div>

</section>

<section class="video-section">
<h1 class="section-title">Showroom</h1>

<video autoplay muted loop>
<source src="https://www.w3schools.com/html/mov_bbb.mp4">
</video>
</section>

<section class="trade" id="trade">

<h1 class="section-title">Takas Fiyatı Al</h1>

<div class="trade-box">

<input type="text" id="brand" placeholder="Marka">
<input type="text" id="model" placeholder="Model">
<input type="number" id="year" placeholder="Yıl">

<button onclick="calculatePrice()">Fiyat Hesapla</button>

<div id="priceResult"></div>

</div>
</section>

<section class="ai" id="ai">

<h1 class="section-title">AI Müşteri Hizmeti</h1>

<div class="ai-box">

<div class="chat" id="chat">
<div class="msg">🤖 Merhaba. Size nasıl yardımcı olabilirim?</div>
</div>

<input type="text" id="userInput" placeholder="Mesaj yazın...">

<button onclick="sendMessage()">Gönder</button>

</div>

</section>

<section class="reviews">

<h1 class="section-title">Müşteri Yorumları</h1>

<div class="review">
★★★★★ “Hayatımda gördüğüm en premium galeri.”
</div>

<div class="review">
★★★★★ “Araçlar kusursuzdu.”
</div>

<div class="review">
★★★★★ “Gerçekten VIP hizmet.”
</div>

</section>

<section class="contact" id="contact">

<h1 class="section-title">İletişim</h1>

<div class="contact-box">

<div class="contact-item">
📞 +90 212 519 70 12
</div>

<div class="contact-item">
📧 aydinauto@help.business
</div>

<div class="contact-item">
📍 İstanbul / Tekirdağ
</div>

<div class="contact-item">
📱 @aydinautoresmi
</div>

<iframe src="https://maps.google.com/maps?q=istanbul&t=&z=13&ie=UTF8&iwloc=&output=embed"></iframe>

</div>

</section>

<a class="whatsapp" href="https://wa.me/902125197012">📞</a>

<footer>
© 2026 AYDIN AUTO • Premium Otomobil Deneyimi
</footer>

<script>

/* MENU */

function openMenu(){
document.getElementById("menu").classList.add("active");
}

function closeMenu(){
document.getElementById("menu").classList.remove("active");
}

/* TAKAS */

function calculatePrice(){

let year=document.getElementById("year").value;

let price=
(2026-year)*-150000+5000000;

if(price<300000){
price=300000;
}

document.getElementById("priceResult").innerHTML=
"Tahmini Teklif: "+price.toLocaleString()+" TL";
}

/* AI CHAT */

function sendMessage(){

let input=document.getElementById("userInput");

let chat=document.getElementById("chat");

if(input.value.trim()=="") return;

chat.innerHTML+=`
<div class="msg">🧑 ${input.value}</div>
`;

setTimeout(()=>{

chat.innerHTML+=`
<div class="msg">🤖 Ekibimiz en kısa sürede size yardımcı olacaktır.</div>
`;

chat.scrollTop=chat.scrollHeight;

},700);

input.value="";
}

/* CONFETTI */

for(let i=0;i<80;i++){

let conf=document.createElement("div");

conf.classList.add("confetti");

conf.style.left=Math.random()*100+"vw";

conf.style.background=
`hsl(${Math.random()*360},100%,50%)`;

conf.style.animationDuration=
(Math.random()*3+2)+"s";

document.body.appendChild(conf);
}

/* PARTICLES */

for(let i=0;i<70;i++){

let p=document.createElement("div");

p.classList.add("particle");

p.style.left=Math.random()*100+"vw";

p.style.animationDuration=
(Math.random()*20+10)+"s";

p.style.opacity=Math.random();

document.body.appendChild(p);
}

</script>

</body>
</html>