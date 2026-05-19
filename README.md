<!DOCTYPE html>
<html lang="sq">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Gjimnazi “Ali Demi” | Vlorë</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

:root{
    --primary:#081b33;
    --secondary:#102d52;
    --gold:#f5c542;
    --white:#ffffff;
    --light:#f4f7fb;
    --text:#2c2c2c;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:var(--light);
    color:var(--text);
}

/* HERO */

.landing-page{
    min-height:100vh;
    background:linear-gradient(180deg,#081b33,#102d52);
    padding:40px 20px;
}

.landing-content{
    max-width:900px;
    margin:auto;
    text-align:center;
    color:white;
}

.landing-content h1{
    font-size:65px;
    font-weight:700;
    margin-top:50px;
}

.landing-content h2{
    font-size:70px;
    color:var(--gold);
    margin-top:-10px;
}

.landing-content p{
    font-size:22px;
    color:#ddd;
    margin-top:10px;
}

/* MENU */

.menu-box{
    margin-top:40px;
    background:white;
    padding:20px;
    border-radius:25px;
    box-shadow:0 10px 30px rgba(0,0,0,0.2);
}

.menu-box select{
    width:100%;
    padding:18px;
    border:none;
    border-radius:15px;
    background:#f4f4f4;
    font-size:22px;
    font-weight:600;
    color:#0b1f3a;
    outline:none;
    cursor:pointer;
}

/* FOTO */

.main-image{
    margin-top:50px;
    background:white;
    padding:18px;
    border-radius:25px;
}

.main-image img{
    width:100%;
    border-radius:20px;
    display:block;
}

/* SECTION */

section{
    padding:100px 10%;
}

.section-title{
    text-align:center;
    margin-bottom:50px;
}

.section-title h2{
    font-size:42px;
    color:var(--primary);
    margin-bottom:10px;
}

.section-title p{
    color:#666;
}

/* HISTORY */

.history{
    background:white;
    border-radius:20px;
    padding:40px;
    box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.history p{
    margin-bottom:20px;
    line-height:1.9;
}

/* CARDS */

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.card{
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.08);
    transition:0.3s;
}

.card:hover{
    transform:translateY(-6px);
}

.card h3{
    color:var(--secondary);
    margin-bottom:15px;
}

/* CONTACT */

.contact{
    background:white;
    padding:50px;
    border-radius:20px;
    box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.contact p{
    margin-bottom:20px;
    font-size:18px;
}

/* FOOTER */

footer{
    background:var(--primary);
    color:white;
    text-align:center;
    padding:30px;
}

/* MOBILE */

@media(max-width:768px){

.landing-content h1{
    font-size:42px;
}

.landing-content h2{
    font-size:48px;
}

.landing-content p{
    font-size:18px;
}

.menu-box select{
    font-size:18px;
}

}

</style>

</head>

<body>

<!-- FAQJA E PARË -->

<section class="landing-page" id="home">

<div class="landing-content">

<h1>
Gjimnazi “Ali Demi”
</h1>

<h2>
Vlorë
</h2>

<p>
Traditë dhe ekselencë që prej vitit 1947
</p>

<!-- MENU -->

<div class="menu-box">

<select onchange="goToSection(this.value)">

<option value="">MENU</option>

<option value="#historiku">Historiku</option>

<option value="#synimi">Synimi</option>

<option value="#drejtuesit">Drejtuesit</option>

<option value="#aktivitetet">Aktivitetet</option>

<option value="#kontakt">Kontakt</option>

</select>

</div>

<!-- FOTO KRYESORE -->

<div class="main-image">

<img src="images/foto1.jpg">

</div>

</div>

</section>

<!-- HISTORIKU -->

<section id="historiku">

<div class="section-title">

<h2>Historiku</h2>

<p>
Historia dhe tradita e shkollës
</p>

</div>

<div class="history">

<p>
Gjimnazi “Ali Demi” u themelua më 20 Tetor 1947
në qytetin e Vlorës dhe konsiderohet një nga
gjimnazet më të njohura në Shqipëri.
</p>

<p>
Ishte shkolla e parë e mesme e pasçlirimit
që mbulonte rrethet Vlorë dhe Fier.
</p>

<p>
Drejtori i parë ishte Koço Papaproko
dhe shkolla fillimisht kishte 42 nxënës.
</p>

<p>
Me kalimin e viteve u krijuan laboratorë,
bibliotekë moderne, aktivitete sportive,
kulturore dhe projekte ndërkombëtare.
</p>

<p>
Sot Gjimnazi “Ali Demi” vazhdon të jetë
një institucion i rëndësishëm arsimor
me rezultate të larta akademike.
</p>

</div>

</section>

<!-- SYNIMI -->

<section id="synimi">

<div class="section-title">

<h2>Synimi i Shkollës</h2>

<p>
Misioni dhe vizioni
</p>

</div>

<div class="grid">

<div class="card">

<h3>Ekselencë Akademike</h3>

<p>
Përgatitja e nxënësve me rezultate të larta
dhe edukim modern.
</p>

</div>

<div class="card">

<h3>Zhvillim Personal</h3>

<p>
Nxitja e talentit, kreativitetit dhe
aftësive profesionale.
</p>

</div>

<div class="card">

<h3>Edukimi Qytetar</h3>

<p>
Formimi i qytetarëve të përgjegjshëm
dhe aktivë në shoqëri.
</p>

</div>

</div>

</section>

<!-- DREJTUESIT -->

<section id="drejtuesit">

<div class="section-title">

<h2>Drejtuesit</h2>

<p>
Stafi drejtues i shkollës
</p>

</div>

<div class="grid">

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

<p>
Aktivitete edukative dhe kulturore
</p>

</div>

<div class="grid">

<div class="card">

<h3>Olimpiada</h3>

<p>
Pjesëmarrje në olimpiada kombëtare
dhe ndërkombëtare.
</p>

</div>

<div class="card">

<h3>Aktivitete Kulturore</h3>

<p>
Koncerte, konkurse dhe evente artistike.
</p>

</div>

<div class="card">

<h3>Sport</h3>

<p>
Aktivitete sportive dhe kampionate shkollore.
</p>

</div>

<div class="card">

<h3>Projekte Europiane</h3>

<p>
Bashkëpunime dhe projekte ndërkombëtare.
</p>

</div>

</div>

</section>

<!-- KONTAKT -->

<section id="kontakt">

<div class="section-title">

<h2>Kontakt</h2>

<p>
Informacionet zyrtare të shkollës
</p>

</div>

<div class="contact">

<p>
<strong>Emri:</strong>
Gjimnazi “Ali Demi”
</p>

<p>
<strong>Adresa:</strong>
Bulevardi “Ismail Qemali”, Vlorë, Shqipëri
</p>

<p>
<strong>Telefon:</strong>
+355 XX XXX XXXX
</p>

<p>
<strong>Email:</strong>
gjimnazialidemi1947@gmail.com
</p>

<p>
<strong>Themeluar:</strong>
20 Tetor 1947
</p>

</div>

</section>

<!-- FOOTER -->

<footer>

<p>
© 2026 Gjimnazi “Ali Demi” —
Të gjitha të drejtat e rezervuara
</p>

</footer>

<script>

function goToSection(section){

if(section !== ""){

window.location.href = section;

}

}

</script>

</body>

</html>