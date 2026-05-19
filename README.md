<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gjimnazi Ali Demi</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#f5f5f5;
    color:#333;
}

header{
    background:#003366;
    color:white;
    padding:20px;
    position:sticky;
    top:0;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

nav ul{
    display:flex;
    list-style:none;
    gap:20px;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

.hero{
    height:90vh;
    background:url('https://images.unsplash.com/photo-1523050854058-8df90110c9f1?q=80&w=1600') center/cover;
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
    text-align:center;
}

.hero h1{
    font-size:60px;
    background:rgba(0,0,0,0.5);
    padding:20px;
    border-radius:10px;
}

section{
    padding:60px 10%;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    background:white;
    padding:20px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

.gallery{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:20px;
}

.gallery img{
    width:100%;
    border-radius:10px;
}

footer{
    background:#003366;
    color:white;
    text-align:center;
    padding:20px;
}

button{
    margin-top:15px;
    padding:12px 25px;
    border:none;
    background:#ffcc00;
    color:black;
    font-weight:bold;
    border-radius:5px;
    cursor:pointer;
}

button:hover{
    background:white;
}
</style>
</head>

<body>

<header>
<nav>
<h2>Gjimnazi Ali Demi</h2>

<ul>
<li><a href="#home">Home</a></li>
<li><a href="#about">Rreth Nesh</a></li>
<li><a href="#staff">Stafi</a></li>
<li><a href="#gallery">Galeria</a></li>
<li><a href="#contact">Kontakt</a></li>
</ul>
</nav>
</header>

<section class="hero" id="home">
<div>
<h1>Mirësevini në Gjimnazin Ali Demi</h1>
<p>Që prej vitit 1947</p>
<button onclick="showMessage()">Lexo më shumë</button>
</div>
</section>

<section id="about">
<h2>Rreth Shkollës</h2>
<br>
<p>
Gjimnazi “Ali Demi” është një nga gjimnazet më të njohura,
duke ofruar arsim cilësor dhe aktivitete të shumta për nxënësit.
</p>
</section>

<section id="staff">
<h2>Stafi Ynë</h2>
<br>

<div class="cards">

<div class="card">
<h3>Drejtori</h3>
<p>Emri i Drejtorit</p>
</div>

<div class="card">
<h3>Mësues Matematikë</h3>
<p>Mësues profesional dhe i kualifikuar.</p>
</div>

<div class="card">
<h3>Mësues Gjuhësh</h3>
<p>Eksperiencë dhe përkushtim.</p>
</div>

</div>
</section>

<section id="gallery">
<h2>Galeria</h2>
<br>

<div class="gallery">
<img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=1200">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=1200">
<img src="https://images.unsplash.com/photo-1513258496099-48168024aec0?q=80&w=1200">
</div>
</section>

<section id="contact">
<h2>Kontakt</h2>
<br>

<p>Email: info@alidemi.edu.al</p>
<p>Telefon: +355 69 000 0000</p>
<p>Adresa: Vlorë, Shqipëri</p>
</section>

<footer>
<p>© 2026 Gjimnazi Ali Demi - Të gjitha të drejtat e rezervuara</p>
</footer>

<script>
function showMessage(){
    alert("Mirësevini në faqen zyrtare të shkollës!");
}
</script>

</body>
</html>
