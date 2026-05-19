<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>Gjimnazi “Ali Demi” | Vlorë</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

:root{
    --primary:#0b1f3a;
    --secondary:#123c73;
    --gold:#f5c542;
    --light:#f5f7fb;
    --white:#ffffff;
    --text:#2c2c2c;
    --shadow:0 10px 30px rgba(0,0,0,0.1);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins', sans-serif;
    background:var(--light);
    color:var(--text);
    overflow-x:hidden;
}

/* NAVBAR */

header{
    width:100%;
    position:fixed;
    top:0;
    left:0;
    z-index:999;
    background:rgba(11,31,58,0.95);
    backdrop-filter:blur(10px);
    box-shadow:0 2px 10px rgba(0,0,0,0.2);
}

nav{
    width:90%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:18px 0;
}

.logo{
    color:white;
    font-size:28px;
    font-weight:700;
    letter-spacing:1px;
}

.logo span{
    color:var(--gold);
}

nav ul{
    display:flex;
    list-style:none;
    gap:28px;
}

nav a{
    text-decoration:none;
    color:white;
    font-weight:500;
    transition:0.3s;
    position:relative;
}

nav a::after{
    content:'';
    position:absolute;
    width:0%;
    height:2px;
    left:0;
    bottom:-5px;
    background:var(--gold);
    transition:0.3s;
}

nav a:hover::after{
    width:100%;
}

/* HERO */

.hero{
    height:100vh;
    background:
    linear-gradient(rgba(0,0,0,0.65), rgba(0,0,0,0.65)),
    url('https://images.unsplash.com/photo-1523050854058-8df90110c9f1?q=80&w=1600')
    center/cover no-repeat;

    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.hero-content{
    max-width:900px;
    color:white;
    animation:fadeIn 1.5s ease;
}

.hero-content h1{
    font-size:72px;
    margin-bottom:20px;
    font-weight:800;
}

.hero-content p{
    font-size:24px;
    line-height:1.7;
    margin-bottom:35px;
}

.hero-btn{
    padding:16px 38px;
    border:none;
    border-radius:50px;
    background:var(--gold);
    color:black;
    font-size:16px;
    font-weight:700;
    cursor:pointer;
    transition:0.3s;
}

.hero-btn:hover{
    transform:translateY(-4px);
    background:white;
}

/* GENERAL */

section{
    padding:110px 10%;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-size:42px;
    color:var(--primary);
    margin-bottom:15px;
}

.section-title p{
    color:#666;
    font-size:17px;
}

/* INFO */

.info-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.card{
    background:white;
    border-radius:20px;
    padding:35px;
    box-shadow:var(--shadow);
    transition:0.4s;
}

.card:hover{
    transform:translateY(-8px);
}

.card h3{
    color:var(--secondary);
    margin-bottom:15px;
    font-size:24px;
}

.card p{
    line-height:1.9;
    color:#555;
}

/* TIMELINE */

.timeline{
    position:relative;
    max-width:1000px;
    margin:auto;
}

.timeline::after{
    content:'';
    position:absolute;
    width:4px;
    background:var(--gold);
    top:0;
    bottom:0;
    left:50%;
    margin-left:-2px;
}

.timeline-item{
    padding:10px 40px;
    position:relative;
    width:50%;
}

.timeline-item::after{
    content:'';
    position:absolute;
    width:22px;
    height:22px;
    right:-11px;
    background:var(--secondary);
    border:4px solid var(--gold);
    top:20px;
    border-radius:50%;
    z-index:1;
}

.left{
    left:0;
}

.right{
    left:50%;
}

.right::after{
    left:-11px;
}

.timeline-content{
    background:white;
    padding:25px;
    border-radius:15px;
    box-shadow:var(--shadow);
}

.timeline-content h3{
    color:var(--secondary);
    margin-bottom:10px;
}

/* STATS */

.stats{
    background:linear-gradient(135deg,var(--primary),var(--secondary));
    color:white;
}

.stats-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:30px;
    text-align:center;
}

.stat-box h2{
    font-size:55px;
    color:var(--gold);
}

.stat-box p{
    margin-top:10px;
    font-size:18px;
}

/* GALLERY */

.gallery{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:25px;
}

.gallery img{
    width:100%;
    height:260px;
    object-fit:cover;
    border-radius:20px;
    transition:0.4s;
    box-shadow:var(--shadow);
}

.gallery img:hover{
    transform:scale(1.03);
}

/* CONTACT */

.contact-box{
    background:white;
    border-radius:20px;
    padding:50px;
    box-shadow:var(--shadow);
}

.contact-item{
    margin-bottom:25px;
}

.contact-item h3{
    color:var(--secondary);
    margin-bottom:10px;
}

/* FOOTER */

footer{
    background:var(--primary);
    color:white;
    text-align:center;
    padding:35px;
    margin-top:50px;
}

footer p{
    opacity:0.9;
}

/* ANIMATION */

@keyframes fadeIn{

from{
    opacity:0;
    transform:translateY(30px);
}

to{
    opacity:1;
    transform:translateY(0);
}

}

/* MOBILE */

@media(max-width:900px){

.hero-content h1{
    font-size:48px;
}

.hero-content p{
    font-size:18px;
}

nav{
    flex-direction:column;
    gap:20px;
}

nav ul{
    flex-wrap:wrap;
    justify-content:center;
}

.timeline::after{
    left:31px;
}

.timeline-item{
    width:100%;
    padding-left:70px;
    padding-right:25px;
}

.timeline-item::after{
    left:20px;
}

.right{
    left:0%;
}

}

</style>
</head>

<body>

<header>

<nav>

<div class="logo">
Ali <span>Demi</span>
</div>

<ul>
<li><a href="#home">Home</a></li>
<li><a href="#historiku">Historiku</a></li>
<li><a href="#synimi">Synimi</a></li>
<li><a href="#drejtuesit">Drejtuesit</a></li>
<li><a href="#aktivitetet">Aktivitetet</a></li>
<li><a href="#galeria">Galeria</a></li>
<li><a href="#kontakt">Kontakt</a></li>
</ul>

</nav>

</header>

<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<h1>Gjimnazi “Ali Demi”</h1>

<p>
Një traditë ekselence që prej vitit 1947 —
arsim cilësor, kulturë dhe përgatitje për të ardhmen.
</p>

<button class="hero-btn" onclick="welcome()">
Mirësevini
</button>

</div>

</section>

<!-- HISTORIKU -->

<section id="historiku">

<div class="section-title">
<h2>Historiku</h2>
<p>Rruga e suksesit ndër vite</p>
</div>

<div class="timeline">

<div class="timeline-item left">
<div class="timeline-content">
<h3>1947</h3>
<p>
Shkolla u themelua më 20 Tetor 1947
si shkolla e parë e mesme e pasçlirimit
në Vlorë.
</p>
</div>
</div>

<div class="timeline-item right">
<div class="timeline-content">
<h3>Vitet e para</h3>
<p>
Drejtori i parë ishte Koço Papaproko
dhe shkolla kishte 42 nxënës.
</p>
</div>
</div>

<div class="timeline-item left">
<div class="timeline-content">
<h3>Zhvillimi</h3>
<p>
U krijuan laboratorë modernë,
biblioteka dhe aktivitete kulturore.
</p>
</div>
</div>

<div class="timeline-item right">
<div class="timeline-content">
<h3>UNESCO</h3>
<p>
Shkolla u bë pjesë e UNESCO-s
duke përfaqësuar Shqipërinë në projekte
ndërkombëtare.
</p>
</div>
</div>

</div>

</section>

<!-- STATS -->

<section class="stats">

<div class="stats-grid">

<div class="stat-box">
<h2>1947</h2>
<p>Viti i themelimit</p>
</div>

<div class="stat-box">
<h2>75+</h2>
<p>Vite traditë</p>
</div>

<div class="stat-box">
<h2>1000+</h2>
<p>Nxënës të diplomuar</p>
</div>

<div class="stat-box">
<h2>50+</h2>
<p>Aktivitete edukative</p>
</div>

</div>

</section>

<!-- SYNIMI -->

<section id="synimi">

<div class="section-title">
<h2>Synimi i Shkollës</h2>
<p>Edukimi për të ardhmen</p>
</div>

<div class="info-grid">

<div class="card">
<h3>Ekselencë Akademike</h3>
<p>
Shkolla synon rezultate të larta akademike
dhe përgatitje universitare profesionale.
</p>
</div>

<div class="card">
<h3>Zhvillim Personal</h3>
<p>
Nxënësit zhvillojnë kreativitetin,
talentin dhe aftësitë sociale.
</p>
</div>

<div class="card">
<h3>Qytetari Aktive</h3>
<p>
Edukimi qytetar dhe përgjegjësia sociale
janë pjesë thelbësore e shkollës.
</p>
</div>

</div>

</section>

<!-- DREJTUESIT -->

<section id="drejtuesit">

<div class="section-title">
<h2>Drejtuesit</h2>
<p>Stafi drejtues i shkollës</p>
</div>

<div class="info-grid">

<div class="card">
<h3>Drejtori</h3>
<p>Roland Dervishaj</p>
</div>

<div class="card">
<h3>Nëndrejtor</h3>
<p>Marjana Papavangjeli</p>
</div>

<div class="card">
<h3>Nëndrejtor</h3>
<p>Mirela Spiro</p>
</div>

<div class="card">
<h3>Nëndrejtor</h3>
<p>Kostanca Bregasi</p>
</div>

</div>

</section>

<!-- AKTIVITETET -->

<section id="aktivitetet">

<div class="section-title">
<h2>Aktivitetet</h2>
<p>Jetë aktive shkollore</p>
</div>

<div class="info-grid">

<div class="card">
<h3>Olimpiada</h3>
<p>
Pjesëmarrje në olimpiada kombëtare
dhe ndërkombëtare.
</p>
</div>

<div class="card">
<h3>Sport</h3>
<p>
Aktivitete sportive dhe kampionate
mes shkollave.
</p>
</div>

<div class="card">
<h3>Aktivitete Kulturore</h3>
<p>
Koncerte, konkurse artistike
dhe evente festive.
</p>
</div>

<div class="card">
<h3>Projekte Europiane</h3>
<p>
Bashkëpunime me shkolla dhe organizata
ndërkombëtare.
</p>
</div>

</div>

</section>

<!-- GALERIA -->

<section id="galeria">

<div class="section-title">
<h2>Galeria</h2>
<p>Momente nga jeta shkollore</p>
</div>

<div class="gallery">

<img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=1200">

<img src="https://images.unsplash.com/photo-1513258496099-48168024aec0?q=80&w=1200">

</div>

</section>

<!-- KONTAKT -->

<section id="kontakt">

<div class="section-title">
<h2>Kontakt</h2>
<p>Informacionet zyrtare të shkollës</p>
</div>

<div class="contact-box">

<div class="contact-item">
<h3>Adresa</h3>
<p>Bulevardi “Ismail Qemali”, Vlorë, Shqipëri</p>
</div>

<div class="contact-item">
<h3>Telefon</h3>
<p>+355 33 421 321</p>
</div>

<div class="contact-item">
<h3>Email</h3>
<p>gjimnazialidemi1947@gmail.com</p>
</div>

<div class="contact-item">
<h3>Themeluar</h3>
<p>20 Tetor 1947</p>
</div>

</div>

</section>

<footer>

<p>
© 2026 Gjimnazi “Ali Demi” —
Të gjitha të drejtat e rezervuara
</p>

</footer>

<script>

function welcome(){

alert("Mirësevini në faqen zyrtare të Gjimnazit “Ali Demi”!");

}

</script>

</body>
</html>