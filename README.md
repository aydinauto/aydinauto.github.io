
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>AYDIN AUTO</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#050505;
color:white;
overflow-x:hidden;
}

/* ÜST MENÜ */

.topbar{
position:fixed;
top:0;
left:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:20px;
background:rgba(0,0,0,0.65);
backdrop-filter:blur(10px);
z-index:999;
}

.logo{
font-size:28px;
font-weight:800;
letter-spacing:2px;
}

.menu-btn{
font-size:34px;
cursor:pointer;
padding-right:10px;
}

/* MENÜ */

.side-menu{
position:fixed;
top:0;
right:-280px;
width:260px;
height:100%;
background:#111;
transition:0.4s;
padding-top:100px;
z-index:1000;
display:flex;
flex-direction:column;
}

.side-menu a{
color:white;
text-decoration:none;
padding:20px 30px;
font-size:20px;
border-bottom:1px solid #222;
}

.side-menu.active{
right:0;
}

/* HERO */

.hero{
height:100vh;
background:
linear-gradient(to bottom, rgba(0,0,0,0.4), rgba(0,0,0,0.8)),
url('35C20A1F-C4C5-4C2D-AE1C-BB8B82E47414.png');

background-size:cover;
background-position:center;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
padding:20px;
}

.hero-content h1{
font-size:70px;
font-weight:800;
}

.hero-content p{
margin-top:20px;
font-size:22px;
color:#ddd;
}

/* BAŞLIK */

.section-title{
font-size:55px;
font-weight:800;
padding:40px 25px 10px;
}

/* ARAÇLAR */

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
box-shadow:0 0 25px rgba(255,255,255,0.05);
}

.car-card img{
width:100%;
height:300px;
object-fit:cover;
display:block;
}

.car-info{
padding:30px;
}

.car-info h2{
font-size:42px;
margin-bottom:15px;
}

.car-info p{
font-size:20px;
line-height:1.6;
color:#bbb;
}

/* İLETİŞİM */

.contact{
margin-top:80px;
padding:80px 30px;
background:#0b0b0b;
text-align:center;
}

.contact h1{
font-size:55px;
margin-bottom:35px;
}

.contact p{
font-size:22px;
margin:18px 0;
color:#ccc;
}

.contact a{
display:inline-block;
margin-top:25px;
padding:16px 30px;
background:white;
color:black;
text-decoration:none;
font-weight:700;
border-radius:14px;
}

/* FOOTER */

.footer{
padding:40px;
text-align:center;
font-size:16px;
color:#666;
}

</style>
</head>

<body>

<!-- MENÜ -->

<div class="topbar">
<div class="logo">AYDIN AUTO</div>

<div class="menu-btn" onclick="toggleMenu()">
☰
</div>
</div>

<div id="sideMenu" class="side-menu">
<a href="#">Ana Sayfa</a>
<a href="#cars">Araçlarımız</a>
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
Lüks, performans ve prestij bir arada.
</p>
</div>

</section>

<!-- ARAÇLAR -->

<h1 class="section-title" id="cars">
Araçlarımız
</h1>

<section class="cars">

<div class="car-card">
<img src="8785FCE8-273D-499B-B370-3481D5DAC245.png">

<div class="car-info">
<h2>BMW 7 Serisi</h2>
<p>
Luxury sedan deneyimi, üst düzey konfor ve premium detaylar.
</p>
</div>
</div>

<div class="car-card">
<img src="73134C2B-05A4-4A36-B23E-8AD0646CA75F.png">

<div class="car-info">
<h2>Mercedes Maybach</h2>
<p>
Güçlü duruş, agresif lüks ruhu ve benzersiz sürüş hissi.
</p>
</div>
</div>

<div class="car-card">
<img src="1E77547B-A49D-4769-8CE2-CE3C2ECC6960.jpeg">

<div class="car-info">
<h2>Audi Rs6</h2>
<p>
Saf performans, egzotik tasarım ve gerçek süper spor deneyimi.
</p>
</div>
</div>

<div class="car-card">
<img src="AC1DB475-2A48-44E2-A6B7-4F771D0225FE.png">

<div class="car-info">
<h2>Lamborghini Urus</h2>
<p>
Lüks SUV dünyasının en prestijli modellerinden biri.
</p>
</div>
</div>

<div class="car-card">
<img src="02F96023-A74D-4FDE-A4A1-1C2C9EDD6195.jpeg">

<div class="car-info">
<h2>Ferrari GTB</h2>
<p>
Süper spor ruhunu dünyasına taşıyan gerçek canavar.
</p>
</div>
</div>

<div class="car-card">
<img src="062B7BCA-316E-49EE-AC93-179B9EC6AC71.png">

<div class="car-info">
<h2>Porsche Cayanne</h2>
<p>
Üst düzey Alman mühendisliği ve sportif SUV karakteri.
</p>
</div>
</div>

</section>

<!-- İLETİŞİM -->

<section class="contact" id="contact">

<h1>İLETİŞİM</h1>

<p>📍 Esenyurt / Florya / Çorlu</p>

<p>📞 +90 212 519 70 12</p>

<p>📱 WhatsAp: +90 552 555 00 00</p>

<p>📧 info@aydinauto.com</p> </p>

<p>📱 WhatsApp: +90 552 555 00 00</p>

<p>📧 info@aydinauto.com</p>

<a href="https://instagram.com/aydinautoresmi" target="_blank">
Instagram Sayfamız
</a>

</section>

<!-- FOOTER -->

<div class="footer">
© 2026 AYDIN AUTO - Tüm Hakları Saklıdır
</div>

<script>

function toggleMenu(){
document.getElementById("sideMenu").classList.toggle("active");
}

</script>

</body>
</html>