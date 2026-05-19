<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gjimnazi "Ali Demi" - Vlorë</title>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Poppins', sans-serif;
    background: #f5f7fa;
    scroll-behavior: smooth;
}

/* HEADER */
header {
    height: 100vh;
    background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.6)),
    url('https://images.unsplash.com/photo-1580582932707-520aed937b7b');
    background-size: cover;
    background-position: center;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
}

header h1 {
    font-size: 50px;
}

header p {
    font-size: 20px;
    margin-top: 10px;
}

/* NAVBAR */
nav {
    position: fixed;
    width: 100%;
    top: 0;
    background: rgba(0,0,0,0.7);
    padding: 15px;
    text-align: center;
    z-index: 1000;
}

nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
}

nav a:hover {
    color: #ffd700;
}

/* SECTIONS */
section {
    padding: 60px 20px;
    text-align: center;
}

h2 {
    margin-bottom: 20px;
    color: #003366;
}

/* CARDS */
.cards {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.card {
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-10px);
}

/* GALLERY */
.gallery {
    display: flex;
    flex-wrap: wrap;
}

.gallery img {
    width: 33.3%;
    height: 250px;
    object-fit: cover;
    transition: 0.3s;
}

.gallery img:hover {
    transform: scale(1.05);
}

/* CONTACT */
.contact p {
    margin: 10px 0;
}

/* FOOTER */
footer {
    background: #003366;
    color: white;
    padding: 20px;
}

</style>
</head>

<body>

<nav>
<a href="#home">Kreu</a>
<a href="#about">Rreth</a>
<a href="#programs">Programet</a>
<a href="#gallery">Galeria</a>
<a href="#contact">Kontakt</a>
</nav>

<header id="home">
<h1>Gjimnazi "Ali Demi"</h1>
<p>Vlorë • Arsim • Edukim • Sukses</p>
</header>

<section id="about">
<h2>Rreth Nesh</h2>
<p>
Gjimnazi “Ali Demi” është një ndër shkollat më të njohura në Vlorë,
që synon të zhvillojë potencialin maksimal të çdo nxënësi.
</p>
</section>

<section id="programs">
<h2>Programet</h2>
<div class="cards">
<div class="card">
<h3>Shkenca</h3>
<p>Matematikë, Fizikë, Kimi</p>
</div>

<div class="card">
<h3>Shoqërore</h3>
<p>Histori, Gjeografi</p>
</div>

<div class="card">
<h3>Gjuhë</h3>
<p>Anglisht, Italisht</p>
</div>
</div>
</section>

<section id="gallery">
<h2>Galeria</h2>
<div class="gallery">
<img src="https://images.unsplash.com/photo-1596495577886-d920f1fb7238">
<img src="https://images.unsplash.com/photo-1588072432836-e10032774350">
<img src="https://images.unsplash.com/photo-1509062522246-3755977927d7">
</div>
</section>

<section id="contact" class="contact">
<h2>Kontakt</h2>
<p>Email: info@alidemi.edu.al</p>
<p>Telefon: +355 XXX XXX XXX</p>
<p>Vlorë, Shqipëri</p>
</section>

<footer>
<p>&copy; 2026 Gjimnazi "Ali Demi"</p>
</footer>

</body>
</html>
