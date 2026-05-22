<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>AYDIN AUTO</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">

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
width:100%;
height:100vh;
background:black;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
z-index:99999;
animation:hideLoader 4s forwards;
}

#loader h1{
font-size:55px;
font-weight:800;
animation:zoom 1.5s infinite alternate;
}

#loader p{
margin-top:15px;
font-size:20px;
color:#aaa;
}

@keyframes zoom{
from{transform:scale(1);}
to{transform:scale(1.08);}
}

@keyframes hideLoader{
0%{opacity:1;}
85%{opacity:1;}
100%{
opacity:0;
visibility:hidden;
}
}

/* NAVBAR */

.topbar{
position:fixed;
top:0;
left:0;
width:100%;
padding:18px 25px;
display:flex;
justify-content:space-between;
align-items:center;
background:rgba(0,0,0,0.45);
backdrop-filter:blur(12px);
z-index:999;
}

.logo{
font-size:30px;
font-weight:800;
}

.menu-btn{
font-size:34px;
cursor:pointer;
}

/* MENU */

.side-menu{
position:fixed;
top:0;
right:-320px;
width:300px;
height:100%;
background:#0c0c0c;
transition:0.4s;
z-index:9999;
padding-top:100px;
}

.side-menu.active{
right:0;
}

.close-btn{
position:absolute;
top:20px;
right:25px;
font-size:35px;
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
linear-gradient(to bottom, rgba(0,0,0,.45), rgba(0,0,0,.85)),
url('35C20A1F-C4C5-4C2D-AE1C-BB8B82E47414.png');

background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero-content{
animation:fadeUp 1.5s;
}

.hero-content h1{
font-size:78px;
font-weight:800;
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
padding:16px 32px;
border-radius:15px;
font-size:18px;
text-decoration:none;
font-weight:700;
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

/* LANGUAGE */

.languages{
position:absolute;
top:100px;
right:20px;
display:flex;
gap:10px;
z-index:999;
}

.languages button{
padding:10px 15px;
border:none;
border-radius:10px;
background:#151515;
color:white;
cursor:pointer;
}

/* TITLES */

.section-title{
font-size:55px;
font-weight:800;
padding:70px 25px 20px;
}

/* STATS */

.stats{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:20px;
padding:25px;
}

.stat{
background:#101010;
padding:35px 20px;
border-radius:25px;
text-align:center;
}

.stat h2{
font-size:42px;
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
box-shadow:0 0 25px rgba(255,255,255,0.04);
transition:0.4s;
position:relative;
}

.car:hover{
transform:translateY(-6px);
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
font-size:30px;
background:rgba(0,0,0,0.4);
padding:10px;
border-radius:50%;
}

.car-info{
padding:28px;
}

.car-info h2{
font-size:40px;
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
background:#161616;
padding:14px;
border-radius:14px;
text-align:center;
font-size:15px;
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

/* WHY */

.why{
padding:25px;
display:flex;
flex-direction:column;
gap:20px;
}

.why-box{
background:#101010;
padding:30px;
border-radius:25px;
}

.why-box h3{
font-size:30px;
margin-bottom:10px;
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

/* CONTACT */

.contact{
padding:80px 25px;
text-align:center;
background:#0a0a0a;
}

.contact h1{
font-size:55px;
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
border-radius:16px;
text-decoration:none;
font-size:20px;
font-weight:700;
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

/* FOOTER */

.footer{
padding:40px;
text-align:center;
font-size:16px;
color:#777;
}

/* FLOAT */

.float{
position:fixed;
bottom:25px;
right:25px;
width:65px;
height:65px;
background:#25D366;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
font-size:34px;
text-decoration:none;
color:white;
z-index:999;
box-shadow:0 0 25px rgba(37,211,102,0.5);
}

/* ANIMATIONS */

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

<!-- LOADER -->

<div id="loader">
<h1>AYDIN AUTO</h1>
<p>Hoşgeldiniz</p>
</div>

<!-- NAVBAR -->

<div class="topbar">

<div class="logo">
AYDIN AUTO
</div>

<div class="menu-btn" onclick="toggleMenu()">
☰
</div>

</div>

<!-- LANGUAGE -->

<div class="languages">
<button onclick="setLang('tr')">TR</button>
<button onclick="setLang('en')">EN</button>
<button onclick="setLang('ar')">AR</button>
</div>

<!-- MENU -->

<div class="side-menu" id="sideMenu">

<div class="close-btn" onclick="toggleMenu()">
✕
</div>

<a href="#">Ana Sayfa</a>
<a href="#cars">Araçlarımız</a>
<a href="#reviews">Yorumlar</a>
<a href="#contact">İletişim</a>

</div>

<!-- HERO -->

<section class="hero">

<div class="hero-content">

<h1 id="title">
AYDIN AUTO
</h1>

<p id="subtitle">
Premium otomobil deneyimi.
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

<!-- STATS -->

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

<!-- CARS -->

<h1 class="section-title" id="cars">
Araçlarımız
</h1>

<section class="cars">

<div class="car">

<div class="favorite">❤️</div>

<img src="8785FCE8-273D-499B-B370-3481D5DAC245.png">

<div class="car-info">

<h2>BMW 7 Serisi</h2>

<p>
Luxury sedan deneyimi.
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

<div class="favorite">🔥</div>

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

<!-- REVIEWS -->

<h1 class="section-title" id="reviews">
Yorumlar
</h1>

<section class="reviews">

<div class="review">
<h3>Ahmet K.</h3>
<p>Gerçekten premium hizmet.</p>
</div>

<div class="review">
<h3>Emirhan T.</h3>
<p>Araçlar anlatıldığı gibi.</p>
</div>

</section>

<!-- CONTACT -->

<section class="contact" id="contact">

<h1>İLETİŞİM</h1>

<p>📞 +90 212 519 70 12</p>

<p>📧 aydinauto@help.business</p>

<div class="contact-buttons">

<a class="whatsapp" href="https://wa.me/902125197012">
WhatsApp
</a>

<a class="instagram"
href="https://instagram.com/aydinautoresmi">
Instagram
</a>

</div>

</section>

<!-- MAP -->

<section class="map">

<iframe
src="https://maps.google.com/maps?q=florya&t=&z=13&ie=UTF8&iwloc=&output=embed">
</iframe>

</section>

<!-- FOOTER -->

<div class="footer">
© 2026 AYDIN AUTO
</div>

<!-- FLOAT -->

<a href="https://wa.me/902125197012" class="float">
☎
</a>

<script>

function toggleMenu(){
document.getElementById("sideMenu").classList.toggle("active");
}

function setLang(lang){

if(lang=="tr"){
document.getElementById("subtitle").innerHTML=
"Premium otomobil deneyimi.";
}

if(lang=="en"){
document.getElementById("subtitle").innerHTML=
"Premium automobile experience.";
}

if(lang=="ar"){
document.getElementById("subtitle").innerHTML=
"تجربة سيارات فاخرة";
}

}

</script>

</body>
</html>