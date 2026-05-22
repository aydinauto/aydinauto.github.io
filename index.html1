<!-- ÇEKİLİŞ MENÜSÜ -->

<div class="menu-item" onclick="openGiveaway()">
🎁 Çekiliş
</div>

<!-- GIVEAWAY POPUP -->

<div id="giveawayPopup">

<div class="giveaway-box">

<div class="close-giveaway" onclick="closeGiveaway()">
✕
</div>

<h1>🎁 MINI COOPER ÇEKİLİŞİ</h1>

<img src="02F96023-A74D-4FDE-A4A1-1C2C9EDD6195.jpeg" class="giveaway-car">

<p class="giveaway-text">
AYDIN AUTO olarak 3 kişiye MINI COOPER hediye ediyoruz.
</p>

<div class="counter-box">

<div class="counter-card">
<h2>719</h2>
<span>Katılımcı</span>
</div>

<div class="counter-card">
<h2>3</h2>
<span>Kazanan</span>
</div>

<div class="counter-card">
<h2>2 Gün</h2>
<span>Kalan Süre</span>
</div>

</div>

<div class="rules">

<h3>Katılım Şartları</h3>

<ul>

<li>Instagram hesabını takip et</li>

<li>Son gönderiyi beğen</li>

<li>2 arkadaşını etiketle</li>

<li>Hikayende paylaş</li>

</ul>

</div>

<a href="https://instagram.com/aydinautoresmi" class="insta-btn">
Instagram’a Git
</a>

<button class="join-btn" onclick="joinGiveaway()">
Çekilişe Katıl
</button>

<p id="joinText"></p>

</div>

</div>

<style>

#giveawayPopup{
position:fixed;
inset:0;
background:rgba(0,0,0,.92);
display:flex;
justify-content:center;
align-items:center;
z-index:999999;
padding:20px;
backdrop-filter:blur(12px);
animation:fadeIn .5s;
}

@keyframes fadeIn{
from{
opacity:0;
transform:scale(.9);
}
to{
opacity:1;
transform:scale(1);
}
}

.giveaway-box{
background:#090909;
width:100%;
max-width:420px;
border-radius:35px;
padding:30px;
position:relative;
border:1px solid rgba(255,255,255,.08);
box-shadow:0 0 60px rgba(255,215,0,.08);
text-align:center;
overflow:hidden;
}

.giveaway-box::before{
content:'';
position:absolute;
width:250px;
height:250px;
background:#ffd700;
filter:blur(120px);
opacity:.15;
top:-100px;
right:-100px;
}

.close-giveaway{
position:absolute;
top:20px;
right:20px;
font-size:34px;
cursor:pointer;
color:white;
}

.giveaway-box h1{
font-size:34px;
margin-bottom:20px;
font-weight:900;
}

.giveaway-car{
width:100%;
height:240px;
object-fit:cover;
border-radius:25px;
margin-bottom:20px;
}

.giveaway-text{
opacity:.82;
line-height:1.7;
margin-bottom:25px;
}

.counter-box{
display:grid;
grid-template-columns:repeat(3,1fr);
gap:10px;
margin-bottom:25px;
}

.counter-card{
background:#151515;
padding:18px 10px;
border-radius:18px;
}

.counter-card h2{
font-size:26px;
color:#ffd700;
margin-bottom:5px;
}

.counter-card span{
font-size:13px;
opacity:.7;
}

.rules{
background:#121212;
padding:20px;
border-radius:20px;
margin-bottom:20px;
text-align:left;
}

.rules h3{
margin-bottom:12px;
}

.rules ul{
padding-left:18px;
line-height:2;
opacity:.8;
}

.insta-btn{
display:block;
background:white;
color:black;
padding:18px;
border-radius:18px;
font-weight:700;
text-decoration:none;
margin-bottom:15px;
transition:.3s;
}

.insta-btn:hover{
transform:translateY(-3px);
}

.join-btn{
width:100%;
padding:18px;
border:none;
border-radius:18px;
background:#ffd700;
font-size:18px;
font-weight:800;
cursor:pointer;
transition:.3s;
}

.join-btn:hover{
transform:scale(1.03);
}

#joinText{
margin-top:18px;
font-size:15px;
color:#00ff88;
font-weight:600;
}

.language-box{
display:flex;
gap:10px;
margin-top:15px;
justify-content:center;
}

.lang-btn{
padding:12px 18px;
background:#151515;
border-radius:14px;
cursor:pointer;
font-weight:700;
}

</style>

<script>

function closeGiveaway(){
document.getElementById("giveawayPopup").style.display="none";
}

function openGiveaway(){
document.getElementById("giveawayPopup").style.display="flex";
}

function joinGiveaway(){

document.getElementById("joinText").innerHTML=
"🎉 Çekilişe başarıyla katıldınız!";

confettiEffect();

}

function confettiEffect(){

for(let i=0;i<80;i++){

let conf=document.createElement("div");

conf.style.position="fixed";
conf.style.width="10px";
conf.style.height="10px";
conf.style.background=
["#ffd700","#ffffff","#00ff88","#ff0033"]
[Math.floor(Math.random()*4)];

conf.style.left=Math.random()*100+"vw";
conf.style.top="-20px";
conf.style.zIndex="9999999";
conf.style.borderRadius="50%";

document.body.appendChild(conf);

let fall=Math.random()*5+3;

conf.animate([

{
transform:"translateY(0px) rotate(0deg)",
opacity:1
},

{
transform:`translateY(${window.innerHeight+200}px)
rotate(720deg)`,
opacity:0
}

],{

duration:fall*1000

});

setTimeout(()=>{
conf.remove();
},6000);

}

}

/* OTOMATİK AÇILIŞ */

setTimeout(()=>{

document.getElementById("giveawayPopup")
.style.display="flex";

},1200);

</script>