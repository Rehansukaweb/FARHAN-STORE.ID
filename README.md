<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RHN Capital</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0b1220;
  --card:#111a2e;
  --accent:#4f8cff;
  --text:#e5e7eb;
  --muted:#9ca3af;
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Inter',sans-serif;
}

body{
  background: radial-gradient(circle at top, #0f1c38, #050812);
  color:var(--text);
  line-height:1.6;
}

/* NAVBAR */
nav{
  position:fixed;
  top:0;
  width:100%;
  backdrop-filter:blur(10px);
  background:rgba(5,8,18,.7);
  border-bottom:1px solid rgba(255,255,255,.05);
  z-index:100;
}

.nav-container{
  max-width:1100px;
  margin:auto;
  padding:16px;
  display:flex;
  justify-content:space-between;
  align-items:center;
}

.logo{
  font-weight:700;
  letter-spacing:1px;
  color:white;
}

nav a{
  color:var(--muted);
  margin-left:20px;
  text-decoration:none;
  font-size:14px;
}

nav a:hover{
  color:white;
}

/* HERO */
.hero{
  min-height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  padding:120px 20px 40px;
}

.hero h1{
  font-size:42px;
  font-weight:700;
  margin-bottom:16px;
  animation:fadeUp .8s ease;
}

.hero p{
  max-width:620px;
  margin:auto;
  color:var(--muted);
  animation:fadeUp 1s ease;
}

.hero button{
  margin-top:32px;
  padding:14px 28px;
  border:none;
  border-radius:10px;
  background:linear-gradient(135deg,#4f8cff,#6aa7ff);
  color:white;
  font-size:15px;
  cursor:pointer;
  box-shadow:0 10px 30px rgba(79,140,255,.4);
  animation:fadeUp 1.2s ease;
}

.hero button:hover{
  transform:translateY(-2px);
}

/* SECTION */
section{
  max-width:1100px;
  margin:auto;
  padding:80px 20px;
}

/* CARDS */
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:24px;
}

.card{
  background:linear-gradient(180deg,#111a2e,#0b1220);
  border:1px solid rgba(255,255,255,.06);
  border-radius:14px;
  padding:24px;
  transition:.3s;
}

.card:hover{
  transform:translateY(-6px);
  box-shadow:0 20px 40px rgba(0,0,0,.4);
}

.card h3{
  margin-bottom:8px;
}

.card p{
  color:var(--muted);
  font-size:14px;
}

/* PORTFOLIO */
.portfolio{
  text-align:center;
}

.portfolio img{
  width:90px;
  margin:20px auto;
}

/* FOOTER */
footer{
  text-align:center;
  padding:40px 20px;
  color:var(--muted);
  font-size:13px;
}

/* ANIMATION */
@keyframes fadeUp{
  from{opacity:0;transform:translateY(20px);}
  to{opacity:1;transform:none;}
}

</style>
</head>

<body>

<nav>
  <div class="nav-container">
    <div class="logo">RHN CAPITAL</div>
    <div>
      <a href="#about">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<div class="hero">
  <div>
    <h1>Independent Digital Asset Management</h1>
    <p>RHN Capital adalah entitas independen yang fokus pada pengelolaan aset digital jangka panjang dengan pendekatan rasional, disiplin, dan berbasis teknologi.</p>
    <button onclick="location.href='ANALISA.html'">Analisa RHN Capital</button>
  </div>
</div>

<section id="about">
  <div class="grid">
    <div class="card">
      <h3>Visi</h3>
      <p>Menjadi entitas profesional dan mandiri dalam pengelolaan aset digital modern.</p>
    </div>
    <div class="card">
      <h3>Misi</h3>
      <p>Mengelola dana secara bertanggung jawab dan meningkatkan literasi keuangan digital.</p>
    </div>
    <div class="card">
      <h3>Prinsip</h3>
      <p>Disiplin, transparan, rasional, dan berorientasi jangka panjang.</p>
    </div>
  </div>
</section>

<section id="portfolio" class="portfolio">
  <h2>Portofolio</h2>
  <img src="https://assets.coingecko.com/coins/images/1/large/bitcoin.png" alt="BTC">
  <p>Bitcoin (BTC) — Alokasi 100%</p>
  <p><a href="https://www.coingecko.com/en/coins/bitcoin" target="_blank" style="color:var(--accent)">Lihat di CoinGecko →</a></p>
</section>

<section id="contact">
  <div class="grid">
    <div class="card">
      <h3>WhatsApp</h3>
      <p>0857-1782-6626</p>
    </div>
    <div class="card">
      <h3>Instagram</h3>
      <p>@huyrehan</p>
    </div>
  </div>
</section>

<footer>
  © 2026 RHN Capital. All rights reserved.
</footer>

</body>
</html>
