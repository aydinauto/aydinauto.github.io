<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AYDIN AUTO</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

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

header{
height:100vh;
background:
linear-gradient(to bottom,rgba(0,0,0,.6),rgba(0,0,0,.95)),
url('https://images.unsplash.com/photo-1503376780353-7e6692767b70?q=80&w=1400&auto=format&fit=crop');
background-size:cover;
background-position:center;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
padding:20px;
}

.hero h1{
font-size:60px;
font-weight:700;
letter-spacing:3px;
}

.hero p{
margin-top:15px;
font-size:20px;
color:#d6d6d6;
}

.btn{
display:inline-block;
margin-top:30px;
padding:15px 40px;
background:#d4af37;
color:black;
text-decoration:none;
border-radius:12px;
font-weight:600;
transition:.3s;
}

.btn:hover{
transform:scale(1.05);
}

.section{
padding:70px 20px;
max-width:1200px;
margin:auto;
}

.section-title{
font-size:38px;
margin-bottom:40px;
text-align:center;
}

.cars{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:25px;
}

.card{
background:#111;
border-radius:22px;
overflow:hidden;
transition:.3s;
box-shadow:0 0 20px rgba(0,0,0,.4);
}

.card:hover{
transform:translateY(-8px);
}

.card img{
width:100%;
height:240px;
object-fit:cover;
}

.card-content{
padding:20px;
}

.card-content h3{
font-size:26px;
margin-bottom:10px;
}

.card-content p{
color:#bdbdbd;
line-height:1.6;
}

.branches{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
margin-top:40px;
}

.branch{
background:#111;
padding:30px;
border-radius:20px;
text-align:center;
border:1px solid #222;
}

.branch h3{
font-size:28px;
margin-bottom:10px;
color:#d4af37;
}

footer{
padding:40px 20px;
text-align:center;
background:#0b0b0b;
margin-top:50px;
border-top:1px solid #222;
}

footer p{
color:#888;
}

</style>
</head>

<body>

<header>
<div class="hero">
<h1>AYDIN AUTO</h1>
<p>Premium Otomobil Deneyimi</p>

<a href="https://instagram.com/aydinautoresmi" class="btn">
Instagram
</a>

</div>
</header>

<section class="section">

<h2 class="section-title">Öne Çıkan Araçlar</h2>

<div class="cars">

<div class="card">
<img src="https://images.unsplash.com/photo-1553440569-bcc63803a83d?q=80&w=1200&auto=format&fit=crop">
<div class="card-content">
<h3>BMW 7 Serisi</h3>
<p>Lüks tasarım, premium sürüş deneyimi ve üst düzey konfor.</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1494905998402-395d579af36f?q=80&w=1200&auto=format&fit=crop">
<div class="card-content">
<h3>Mercedes G63 AMG</h3>
<p>Güçlü görünüm, agresif performans ve premium detaylar.</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1502161254066-6c74afbf07aa?q=80&w=1200&auto=format&fit=crop">
<div class="card-content">
<h3>Lamborghini Urus</h3>
<p>Sportif SUV deneyimi ve benzersiz tasarım çizgileri.</p>
</div>
</div>

</div>

</section>

<section class="section">

<h2 class="section-title">Şubelerimiz</h2>

<div class="branches">

<div class="branch">
<h3>Esenyurt</h3>
<p>Merkez Şube</p>
</div>

<div class="branch">
<h3>Florya</h3>
<p>2. Şube</p>
</div>

<div class="branch">
<h3>Çorlu</h3>
<p>3. Şube</p>
</div>

</div>

</section>

<footer>
<h2>AYDIN AUTO</h2>
<p>Sıfır ve 2. El Premium Otomobiller</p>
</footer>

</body>
</html>