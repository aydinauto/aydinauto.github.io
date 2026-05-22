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

/* LOADING */

#loader{
position:fixed;
width:100%;
height:100vh;
background:black;
display:flex;
justify-content:center;
align-items:center;
font-size:40px;
font-weight:800;
z-index:99999;
animation:fadeOut 2.5s forwards;
}

@keyframes fadeOut{
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
background:rgba(0,0,0,0.55);
backdrop-filter:blur(12px);
z-index:9999;
}

.logo{
font-size:30px;
font-weight:800;
letter-spacing:2px;
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
background:#0b0b0b;
z-index:10000;
transition:0.4s;
padding-top:100px;
box-shadow:-10px 0 30px rgba(0,0,0,0.5);
}

.side-menu.active{
right:0;
}

.close-btn{
position:absolute;
top:25px;
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
linear-gradient(to bottom, rgba(0,0,0,0.45), rgba(0,0,0,0.85)),
url('35C20A1F-C4C5-4C2D-AE1C-BB8B82E47414.png');

background-size:cover;
background-position:center;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero-content h1{
font-size:75px;
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
padding:15px 30px;
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

.btn-dark{
background:#1a1a1a;
color:white;
border:1px solid #333;
}

/* SECTION */

.section-title{
font-size:58px;
font-weight:800;
padding:70px 25px 10px;
}

/* STATS */

.stats{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:20px;
padding:25px;
}

.stat-box{
background:#0e0e0e;
padding:35px 20px;
border-radius:25px;
text-align:center;
}

.stat-box h2{
font-size:45px;
margin-bottom:10px;
}

.stat-box p{
font-size:18px;
color:#bbb;
}

/* CARS */

.cars{
padding:20px;
display:flex;
flex-direction:column;
gap:35px;
}

.car-card{
background:#0d0d0d;
border-radius:35px;
overflow:hidden;
box-shadow:0 0 25px rgba(255,255,255,0.04);
transition:0.4s;
}

.car-card:hover{
transform:translateY(-5px);
}

.car-card img{
width:100%;
height:320px;
object-fit:cover;
display:block;
}

.car-info{
padding:28px;
}

.car-info h2{
font-size:42px;
margin-bottom:15px;
}

.car-info p{
font-size:19px;
line-height:1.7;
color:#bbb;
margin-bottom:20px;
}

.car-specs{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:12px;
margin-top:15px;
}

.spec{
background:#151515;
padding:14px;
border-radius:14px;
font-size:15px;
text-align:center;
}

/* BADGE */

.badge{
display:inline-block;
margin-top:15px;
padding:10px 18px;
border-radius:12px;
background:#1d7f3f;
font-size:14px;
font-weight:700;
}

/* WHY US */

.why{
padding:70px 25px;
}

.why-box{
background:#0d0d0d;
padding:30px;
border-radius:30px;
margin-bottom:20px;
}

.why-box h3{
font-size:28px;
margin-bottom:12px;
}

.why-box p{
font-size:18px;
color:#bbb;
line-height:1.7;
}

/* REVIEWS */

.reviews{
padding:30px 20px;
display:flex;
flex-direction:column;
gap:20px;
}

.review{
background:#101010;
padding:25px;
border-radius:25px;
}

.review h4{
font-size:22px;
margin-bottom:10px;
}

.review p{
color:#bbb;
line-height:1.6;
}

/* CONTACT */

.contact{
padding:80px 25px;
background:#0a0a0a;
text-align:center;
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
border-radius:18px;
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
padding:40px 20px;
text-align:center;
font-size:16px;
color:#666;
}

/* FLOATING BUTTON */

.whatsapp-float{
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

</style>
</head>

<body>

<div id="loader">
AYDIN AUTO
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

<!-- MENU -->

<div class="side-menu" id="sideMenu">

<div class="close-btn" onclick="toggleMenu()">
✕
</div>

<a href="#">Ana Sayfa</a>
<a href="#cars">Araçlarımız</a>
<a href="#why">Neden Biz?</a>
<a href="#reviews">Yorumlar</a>
<a href="#contact">İletişim</a>
<a href="https://instagram.com/aydinautoresmi" target="_blank">
Instagram
</a>

</div>

<!-- HERO -->

<section class="hero">

<div class="hero-content">

<h1>AYDIN AUTO</h1>

<p>
Premium otomobil deneyimi.<br>
Lüks, performans ve prestiji bir araya getiriyoruz.
</p>

<div class="hero-buttons">

<a href="#cars" class="btn-white">
Araçlarımız
</a>

<a href="#contact" class="btn-dark">
İletişim
</a>

</div>

</div>

</section>

<!-- STATS -->

<section class="stats">

<div class="stat-box">
<h2>250+</h2>
<p>Mutlu Müşteri</p>
</div>

<div class="stat-box">
<h2>120+</h2>
<p>Premium Araç</p>
</div>

<div class="stat-box">
<h2>7/24</h2>
<p>Destek Hizmeti</p>
</div>

<div class="stat-box">
<h2>%100</h2>
<p>Ekspertiz Garantisi</p>
</div>

</section>

<!-- CARS -->

<h1 class="section-title" id="cars">
Araçlarımız
</h1>

<section class="cars">

<div class="car-card">

<img src="8785FCE8-273D-499B-B370-3481D5DAC245.png">

<div class="car-info">

<h2>BMW 7 Serisi</h2>

<p>
Luxury sedan deneyimi ve üst düzey Alman mühendisliği.
</p>

<div class="car-specs">

<div class="spec">2024 Model</div>
<div class="spec">3.0 Motor</div>
<div class="spec">374 HP</div>
<div class="spec">12.000 KM</div>

</div>

<div class="badge">
STOKTA VAR
</div>

</div>

</div>

<div class="car-card">

<img src="73134C2B-05A4-4A36-B23E-8AD0646CA75F.png">

<div class="car-info">

<h2>Mercedes Maybach</h2>

<p>
Agresif  ruhu ve benzersiz lüks deneyimi.
</p>

<div class="car-specs">

<div class="spec">503 HP</div>
<div class="spec">2025 Model</div>
<div class="spec">V8</div>
<div class="spec">8.000 KM</div>

</div>

<div class="badge">
YENİ GELEN
</div>

</div>

</div>

<div class="car-card">

<img src="1E77547B-A49D-4769-8CE2-CE3C2ECC6960.jpeg">

<div class="car-info">

<h2>Audi Rs6</h2>

<p>
Gerçek süper spor deneyimi ve eşsiz tasarımı.
</p>

<div class="car-specs">

<div class="spec">670 HP</div>
<div class="spec">2023 Model</div>
<div class="spec">V8 Turbo</div>
<div class="spec">5.000 KM</div>

</div>

<div class="badge">
ÖZEL SERİ
</div>

</div>

</div>

</section>

<!-- WHY -->

<h1 class="section-title" id="why">
Neden AYDIN AUTO?
</h1>

<section class="why">

<div class="why-box">
<h3>Ekspertiz Garantisi</h3>
<p>
Tüm araçlarımız detaylı ekspertiz kontrolünden geçmektedir.
</p>
</div>

<div class="why-box">
<h3>Premium Hizmet</h3>
<p>
Müşteri memnuniyetini ön planda tutan VIP hizmet anlayışı.
</p>
</div>

<div class="why-box">
<h3>Geniş Araç Yelpazesi</h3>
<p>
SUV, sedan ve süper spor segmentlerinde özel araçlar.
</p>
</div>

</section>

<!-- REVIEWS -->

<h1 class="section-title" id="reviews">
Müşteri Yorumları
</h1>

<section class="reviews">

<div class="review">
<h4>Alara A.</h4>
<p>
“Hayatımda gördüğüm en profesyonel galeri hizmetlerinden biri.”
</p>
</div>

<div class="review">
<h4>Buse T.</h4>
<p>
“Araçlar gerçekten anlatıldığı gibi kusursuz durumda.”
</p>
</div>

</section>

<!-- CONTACT -->

<section class="contact" id="contact">

<h1>İLETİŞİM</h1>

<p>📍 İstanbul / Florya</p>

<p>📞 +90 212 519 70 12</p>

<p>📧 aydinauto@help.business</p>

<div class="contact-buttons">

<a class="whatsapp" href="https://wa.me/902125197012">
WhatsApp İletişim
</a>

<a class="instagram" href="https://instagram.com/aydinautoresmi" target="_blank">
Instagram Sayfamız
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

© 2026 AYDIN AUTO <br>
Tüm Hakları Saklıdır

</div>

<!-- FLOATING -->

<a
href="https://wa.me/902125197012"
class="whatsapp-float">

☎

</a>

<script>

function toggleMenu(){
document.getElementById("sideMenu").classList.toggle("active");
}

</script>

</body>
</html>