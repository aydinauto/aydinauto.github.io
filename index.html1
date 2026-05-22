
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>AYDIN AUTO</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">

<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:
radial-gradient(circle at top left,#1a1a1a,#050505 60%);
color:white;
overflow-x:hidden;
}

/* LOADER */

#loader{
position:fixed;
width:100%;
height:100vh;
background:black;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
z-index:999999;
transition:1s;
}

#loader h1{
font-size:60px;
font-weight:800;
animation:pulse 1.2s infinite alternate;
}

#loader p{
margin-top:15px;
font-size:20px;
color:#aaa;
}

@keyframes pulse{
from{transform:scale(1);}
to{transform:scale(1.08);}
}

/* NAVBAR */

.navbar{
position:fixed;
top:0;
left:0;
width:100%;
padding:18px 22px;
display:flex;
justify-content:space-between;
align-items:center;
background:rgba(0,0,0,0.45);
backdrop-filter:blur(14px);
z-index:9999;
}

.logo{
font-size:32px;
font-weight:800;
letter-spacing:2px;
}

.menu-btn{
font-size:34px;
cursor:pointer;
}

/* SIDE MENU */

.side-menu{
position:fixed;
top:0;
right:-320px;
width:300px;
height:100%;
background:#0d0d0d;
z-index:99999;
transition:0.4s;
padding-top:100px;
}

.side-menu.active{
right:0;
}

.close-btn{
position:absolute;
top:25px;
right:25px;
font-size:34px;
cursor:pointer;
}

.side-menu a{
display:block;
padding:22px 30px;
color:white;
text-decoration:none;
font-size:22px;
border-bottom:1px solid #181818;
}

/* HERO */

.hero{
height:100vh;
background:
linear-gradient(to bottom,rgba(0,0,0,.45),rgba(0,0,0,.88)),
url('35C20A1F-C4C5-4C2D-AE1C-BB8B82E47414.png');

background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
position:relative;
}

.hero::after{
content:'';
position:absolute;
width:300px;
height:300px;
background:#d4af3735;
filter:blur(100px);
top:80px;
right:-50px;
border-radius:50%;
}

.hero-content{
z-index:2;
animation:fadeUp 1.5s;
}

.hero-content h1{
font-size:72px;
font-weight:800;
line-height:1.1;
}

.hero-content p{
margin-top:20px;
font-size:22px;
color:#ddd;
line-height:1.6;
}

.hero-buttons{
margin-top:35px;
display:flex;
justify-content:center;
gap:15px;
flex-wrap:wrap;
}

.hero-buttons a{
padding:16px 34px;
border-radius:18px;
font-size:18px;
font-weight:700;
text-decoration:none;
transition:0.3s;
}

.btn-white{
background:white;
color:black;
}

.btn-gold{
background:#d4af37;
color:black;
}

.hero-buttons a:hover{
transform:translateY(-5px);
}

/* LANG */

.languages{
position:absolute;
top:100px;
right:20px;
display:flex;
gap:10px;
z-index:999;
}

.languages button{
padding:12px 18px;
border:none;
background:#121212;
color:white;
border-radius:14px;
font-size:15px;
cursor:pointer;
}

/* TITLES */

.section-title{
font-size:52px;
font-weight:800;
padding:80px 25px 20px;
}

/* STATS */

.stats{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:18px;
padding:25px;
}

.stat{
background:#101010;
padding:35px 20px;
border-radius:30px;
text-align:center;
box-shadow:0 0 25px rgba(255,255,255,0.03);
}

.stat h2{
font-size:40px;
margin-bottom:10px;
}

/* CARS */

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
position:relative;
box-shadow:0 0 30px rgba(255,255,255,0.03);
transition:0.4s;
}

.car:hover{
transform:translateY(-7px);
}

.car img{
width:100%;
height:320px;
object-fit:cover;
display:block;
}

.favorite{
position:absolute;
top:20px;
right:20px;
background:rgba(0,0,0,.5);
padding:12px;
border-radius:50%;
font-size:25px;
}

.car-info{
padding:28px;
}

.car-info h2{
font-size:42px;
margin-bottom:15px;
}

.car-info p{
font-size:18px;
line-height:1.7;
color:#bbb;
}

.specs{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:12px;
margin-top:20px;
}

.spec{
background:#171717;
padding:14px;
border-radius:15px;
text-align:center;
}

.badge{
display:inline-block;
margin-top:20px;
padding:10px 18px;
background:#1d7f3f;
border-radius:12px;
font-size:14px;
font-weight:700;
}

/* TRADE */

.trade{
padding:25px;
}

.trade-box{
background:#101010;
padding:30px;
border-radius:30px;
}

.trade-box h2{
font-size:40px;
margin-bottom:20px;
}

.trade-box select,
.trade-box input{
width:100%;
padding:18px;
margin-bottom:15px;
border:none;
border-radius:15px;
background:#181818;
color:white;
font-size:16px;
}

.trade-box button{
width:100%;
padding:18px;
border:none;
background:#d4af37;
color:black;
font-weight:700;
border-radius:15px;
font-size:18px;
cursor:pointer;
}

.result{
margin-top:20px;
font-size:22px;
font-weight:700;
text-align:center;
}

/* AI */

.ai-chat{
padding:25px;
}

.ai-box{
background:#101010;
padding:30px;
border-radius:30px;
}

.ai-box textarea{
width:100%;
height:120px;
padding:18px;
background:#181818;
border:none;
border-radius:15px;
color:white;
font-size:16px;
resize:none;
}

.ai-box button{
width:100%;
padding:18px;
margin-top:15px;
border:none;
background:white;
color:black;
font-size:18px;
font-weight:700;
border-radius:15px;
cursor:pointer;
}

.ai-response{
margin-top:20px;
color:#ccc;
line-height:1.8;
}

/* CONTACT */

.contact{
padding:80px 25px;
text-align:center;
}

.contact h1{
font-size:52px;
margin-bottom:30px;
}

.contact p{
font-size:22px;
margin:15px 0;
color:#ccc;
}

.contact-buttons{
margin-top:35px;
display:flex;
flex-direction:column;
gap:15px;
}

.contact-buttons a{
padding:18px;
border-radius:18px;
font-size:20px;
font-weight:700;
text-decoration:none;
}

.whatsapp{
background:#25D366;
color:white;
}

.instagram{
background:white;
color:black;
}

/* MAP */

.map{
padding:20px;
}

.map iframe{
width:100%;
height:300px;
border:none;
border-radius:30px;
}

/* FLOAT */

.float{
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
font-size:36px;
color:white;
text-decoration:none;
z-index:9999;
box-shadow:0 0 30px rgba(37,211,102,0.5);
}

/* FOOTER */

.footer{
padding:40px;
text-align:center;
font-size:16px;
color:#777;
}

/* ANIM */

@keyframes fadeUp{
from{
opacity:0;
transform:translateY(40px);
}
to{
opacity:1;
transform:translateY(0);
}
}

</style>
</head>

<body>

<div id="loader">
<h1>AYDIN AUTO</h1>
<p>Hoşgeldiniz...</p>
</div>

<div class="navbar">

<div class="logo">
AYDIN AUTO
</div>

<div class="menu-btn" onclick="toggleMenu()">
☰
</div>

</div>

<div class="languages">
<button onclick="setLang('tr')">TR</button>
<button onclick="setLang('en')">EN</button>
<button onclick="setLang('ar')">AR</button>
</div>

<div class="side-menu" id="sideMenu">

<div class="close-btn" onclick="toggleMenu()">
✕
</div>

<a href="#">Ana Sayfa</a>
<a href="#cars">Araçlarımız</a>
<a href="#trade">Takas</a>
<a href="#ai">AI Destek</a>
<a href="#contact">İletişim</a>

</div>

<section class="hero">

<div class="hero-content">

<h1 id="heroTitle">
AYDIN AUTO
</h1>

<p id="heroText">
Premium otomobil deneyimi ve lüks yaşam tarzı.
</p>

<div class="hero-buttons">

<a href="#cars" class="btn-white">
Araçlarımız
</a>

<a href="#contact" class="btn-gold">
İletişim
</a>

</div>

</div>

</section>

<h1 class="section-title">
İstatistikler
</h1>

<section class="stats">

<div class="stat">
<h2>250+</h2>
<p>Müşteri</p>
</div>

<div class="stat">
<h2>120+</h2>
<p>Araç</p>
</div>

<div class="stat">
<h2>7/24</h2>
<p>Destek</p>
</div>

<div class="stat">
<h2>%100</h2>
<p>Ekspertiz</p>
</div>

</section>

<h1 class="section-title" id="cars">
Araçlarımız
</h1>

<section class="cars">

<div class="car">

<div class="favorite">🔥</div>

<img src="8785FCE8-273D-499B-B370-3481D5DAC245.png">

<div class="car-info">

<h2>BMW 7 Serisi</h2>

<p>
Luxury sedan dünyasının zirvesi.
</p>

<div class="specs">

<div class="spec">2024</div>
<div class="spec">374 HP</div>
<div class="spec">12.000 KM</div>
<div class="spec">3.0 Motor</div>

</div>

<div class="badge">
STOKTA
</div>

</div>

</div>

<div class="car">

<div class="favorite">❤️</div>

<img src="73134C2B-05A4-4A36-B23E-8AD0646CA75F.png">

<div class="car-info">

<h2>Mercedes G63 AMG</h2>

<p>
Gerçek AMG ruhu.
</p>

<div class="specs">

<div class="spec">585 HP</div>
<div class="spec">2025</div>
<div class="spec">4.0 V8</div>
<div class="spec">8.000 KM</div>

</div>

<div class="badge">
YENİ GELEN
</div>

</div>

</div>

</section>

<h1 class="section-title" id="trade">
Takas Hesaplama
</h1>

<section class="trade">

<div class="trade-box">

<h2>Aracınızı Değerlendirin</h2>

<select id="brand">
<option>BMW</option>
<option>Mercedes</option>
<option>Audi</option>
<option>Porsche</option>
</select>

<input type="number" id="year" placeholder="Model Yılı">

<button onclick="calculatePrice()">
Tahmini Fiyat Hesapla
</button>

<div class="result" id="result">
</div>

</div>

</section>

<h1 class="section-title" id="ai">
AI Müşteri Hizmetleri
</h1>

<section class="ai-chat">

<div class="ai-box">

<textarea id="question"
placeholder="Bir soru sorun..."></textarea>

<button onclick="askAI()">
Soruyu Gönder
</button>

<div class="ai-response" id="aiResponse">
</div>

</div>

</section>

<section class="contact" id="contact">

<h1>İLETİŞİM</h1>

<p>📞 +90 212 519 70 12</p>

<p>📧 aydinauto@help.business</p>

<div class="contact-buttons">

<a class="whatsapp"
href="https://wa.me/902125197012">
WhatsApp
</a>

<a class="instagram"
href="https://instagram.com/aydinautoresmi">
Instagram
</a>

</div>

</section>

<section class="map">

<iframe
src="https://maps.google.com/maps?q=florya&t=&z=13&ie=UTF8&iwloc=&output=embed">
</iframe>

</section>

<div class="footer">
© 2026 AYDIN AUTO
</div>

<a href="https://wa.me/902125197012"
class="float">
☎
</a>

<script>

window.onload=function(){

setTimeout(()=>{
document.getElementById("loader").style.opacity="0";
document.getElementById("loader").style.visibility="hidden";
},3000);

confetti({
particleCount:180,
spread:120,
origin:{y:0.6}
});

}

function toggleMenu(){
document.getElementById("sideMenu").classList.toggle("active");
}

function calculatePrice(){

let year=document.getElementById("year").value;

let base=1500000;

let price=base-(2026-year)*50000;

document.getElementById("result").innerHTML=
"Tahmini Değer: "+price.toLocaleString()+" TL";

}

function askAI(){

let q=document.getElementById("question").value;

let response="";

if(q.includes("fiyat")){
response="Size en uygun fiyat teklifini WhatsApp üzerinden sağlayabiliriz.";
}
else if(q.includes("takas")){
response="Takas desteğimiz mevcuttur.";
}
else{
response="AYDIN AUTO premium destek ekibi sizinle ilgilenecektir.";
}

document.getElementById("aiResponse").innerHTML=response;

}

function setLang(lang){

if(lang=="en"){
document.getElementById("heroText").innerHTML=
"Premium automobile experience and luxury lifestyle.";
}

if(lang=="ar"){
document.getElementById("heroText").innerHTML=
"تجربة سيارات فاخرة";
}

if(lang=="tr"){
document.getElementById("heroText").innerHTML=
"Premium otomobil deneyimi ve lüks yaşam tarzı.";
}

}

</script>

</body>
</html>