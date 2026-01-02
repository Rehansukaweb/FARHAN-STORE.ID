<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RHN Capital</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>
:root{
  --navy:#0b1c2d;
  --blue:#102a43;
  --gold:#d4af37;
  --gray:#f4f6f8;
}

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
  font-family:'Inter',sans-serif;
}

body{
  background:#fff;
  color:#222;
  line-height:1.6;
}

/* ===== NAVBAR ===== */
nav{
  background:var(--navy);
  padding:16px 0;
}

.nav-container{
  max-width:1100px;
  margin:auto;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:0 20px;
}

nav h1{
  color:var(--gold);
  font-size:20px;
  letter-spacing:1px;
}

nav a{
  color:#fff;
  text-decoration:none;
  margin-left:20px;
  font-size:14px;
}

/* ===== HERO ===== */
.hero{
  background:linear-gradient(135deg,var(--navy),var(--blue));
  color:#fff;
  padding:80px 20px;
}

.hero-container{
  max-width:1100px;
  margin:auto;
}

.hero h2{
  font-size:38px;
  margin-bottom:20px;
}

.hero p{
  max-width:600px;
  color:#d1d9e6;
  margin-bottom:30px;
}

.hero .btn{
  background:var(--gold);
  color:#000;
  padding:14px 28px;
  border-radius:6px;
  text-decoration:none;
  font-weight:600;
}

/* ===== SECTION ===== */
section{
  padding:70px 20px;
}

.container{
  max-width:1100px;
  margin:auto;
}

.section-title{
  font-size:28px;
  margin-bottom:20px;
  color:var(--navy);
}

.section-desc{
  max-width:700px;
  margin-bottom:40px;
  color:#555;
}

/* ===== PORTFOLIO ===== */
.portfolio-box{
  background:var(--gray);
  padding:40px;
  border-radius:10px;
  display:flex;
  align-items:center;
  gap:30px;
}

.portfolio-box img{
  width:120px;
}

.portfolio-box h3{
  margin-bottom:10px;
}

/* ===== GRID ===== */
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
  gap:24px;
}

.card{
  background:#fff;
  padding:30px;
  border-radius:10px;
  box-shadow:0 10px 30px rgba(0,0,0,0.05);
}

/* ===== CONTACT ===== */
.contact a{
  display:inline-block;
  margin-right:15px;
  margin-top:10px;
  padding:12px 22px;
  border-radius:6px;
  background:var(--navy);
  color:#fff;
  text-decoration:none;
  font-weight:500;
}

/* ===== FOOTER ===== */
footer{
  background:var(--navy);
  color:#aaa;
  text-align:center;
  padding:25px;
  margin-top:60px;
}
</style>
</head>

<body>

<!-- NAV -->
<nav>
  <div class="nav-container">
    <h1>RHN CAPITAL</h1>
    <div>
      <a href="#about">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#vision">Vision</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-container">
    <h2>Independent Digital Asset Management</h2>
    <p>
      RHN Capital adalah entitas independen yang berfokus pada pengelolaan aset digital
      jangka panjang berbasis teknologi blockchain.
    </p>
    <a href="ANALISA.html" class="btn">Analisa RHN Capital</a>
  </div>
</div>

<!-- ABOUT -->
<section id="about">
  <div class="container">
    <h2 class="section-title">Tentang Kami</h2>
    <p class="section-desc">
      RHN Capital dikelola oleh individu muda yang disiplin, rasional,
      dan berorientasi pada pertumbuhan aset digital berkelanjutan.
    </p>
  </div>
</section>

<!-- PORTFOLIO -->
<section id="portfolio">
  <div class="container">
    <h2 class="section-title">Portofolio</h2>
    <div class="portfolio-box">
      <img src="https://assets.coingecko.com/coins/images/1/large/bitcoin.png">
      <div>
        <h3>Bitcoin (BTC)</h3>
        <p>Alokasi portofolio: <strong>100%</strong></p>
        <a href="https://www.coingecko.com/en/coins/bitcoin" target="_blank">Lihat di CoinGecko</a>
      </div>
    </div>
  </div>
</section>

<!-- VISION -->
<section id="vision">
  <div class="container">
    <h2 class="section-title">Visi & Misi</h2>
    <div class="grid">
      <div class="card">
        <h3>Visi</h3>
        <p>
          Menjadi entitas mandiri yang profesional dalam pengelolaan aset digital modern.
        </p>
      </div>
      <div class="card">
        <h3>Misi</h3>
        <p>
          Mengelola dana secara bertanggung jawab dan meningkatkan literasi keuangan digital.
        </p>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="container">
    <h2 class="section-title">Kontak</h2>
    <div class="contact">
      <a href="https://wa.me/6285717826626">WhatsApp</a>
      <a href="https://instagram.com/huyrehan">Instagram</a>
    </div>
  </div>
</section>

<footer>
© 2025 RHN Capital. All rights reserved.
</footer>

</body>
</html>
