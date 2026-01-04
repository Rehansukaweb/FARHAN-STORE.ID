<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>RHN Capital</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: linear-gradient(180deg, #0b1220, #0e1628);
      color: #eaeaea;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* NAVBAR */
    header {
      position: sticky;
      top: 0;
      background: rgba(11,18,32,0.85);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(255,255,255,0.05);
      z-index: 100;
    }

    .nav {
      max-width: 1100px;
      margin: auto;
      padding: 18px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-weight: 700;
      letter-spacing: 1px;
      color: #f5c26b;
      font-size: 18px;
    }

    .nav a {
      margin-left: 20px;
      font-size: 14px;
      color: #cfd6e3;
    }

    .nav a:hover {
      color: #ffffff;
    }

    /* HERO */
    .hero {
      max-width: 1100px;
      margin: auto;
      padding: 90px 20px 70px;
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      gap: 40px;
      align-items: center;
    }

    .hero h1 {
      font-size: 42px;
      font-weight: 700;
      line-height: 1.2;
      margin-bottom: 20px;
    }

    .hero p {
      color: #b6c0d1;
      font-size: 16px;
      margin-bottom: 30px;
    }

    .btn {
      display: inline-block;
      padding: 14px 26px;
      border-radius: 10px;
      background: linear-gradient(135deg,#f5c26b,#d9a441);
      color: #0b1220;
      font-weight: 600;
      transition: transform .2s ease, box-shadow .2s ease;
      box-shadow: 0 10px 30px rgba(245,194,107,0.25);
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 15px 40px rgba(245,194,107,0.35);
    }

    .hero-card {
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.06);
      border-radius: 18px;
      padding: 40px;
      text-align: center;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }

    /* SECTION */
    section {
      max-width: 1100px;
      margin: auto;
      padding: 80px 20px;
    }

    section h2 {
      font-size: 28px;
      margin-bottom: 30px;
    }

    .text-muted {
      color: #b6c0d1;
    }

    /* PORTFOLIO */
    .portfolio {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(260px,1fr));
      gap: 30px;
    }

    .card {
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.06);
      border-radius: 16px;
      padding: 30px;
      transition: transform .3s ease, box-shadow .3s ease;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 20px 50px rgba(0,0,0,0.4);
    }

    .card img {
      width: 80px;
      margin-bottom: 15px;
    }

    /* CONTACT */
    .contact {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }

    .contact a {
      flex: 1;
      min-width: 220px;
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.06);
      border-radius: 14px;
      padding: 18px;
      text-align: center;
      transition: background .3s ease;
    }

    .contact a:hover {
      background: rgba(255,255,255,0.08);
    }

    footer {
      text-align: center;
      padding: 30px;
      color: #8f9bb3;
      font-size: 13px;
      border-top: 1px solid rgba(255,255,255,0.05);
    }

    @media(max-width:900px){
      .hero{
        grid-template-columns: 1fr;
        padding-top: 70px;
      }
      .hero h1{
        font-size: 34px;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="nav">
    <div class="logo">RHN CAPITAL</div>
    <nav>
      <a href="#about">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>
<img src="RHN LOGO.jpg" alt="Logo RHN" style="width:1000px;">
<section class="hero">
  <div>
    <h1>RHN CAPITAL</h1>
    <p>
      Rehan CPTL adalah entitas independen yang berfokus pada pengelolaan aset digital jangka panjang berbasis teknologi blockchain. RHN Capital mengedepankan pendekatan rasional, disiplin, dan manajemen risiko yang ketat dalam setiap pengambilan keputusan, dengan menempatkan Bitcoin sebagai fondasi utama portofolio. Berorientasi pada keberlanjutan dan konsistensi, RHN Capital hadir sebagai representasi investasi modern yang profesional, transparan, dan bertanggung jawab dalam menghadapi dinamika pasar global.
    </p>
    <a href="ANALISA.html" class="btn">Analisa RHN Capital</a>
  </div>

  <div class="hero-card">
    <img src="https://assets.coingecko.com/coins/images/1/large/bitcoin.png" width="500">
    <h3>Bitcoin (BTC)</h3>
    <p class="text-muted">Primary Strategic Asset</p>
  </div>
</section>

<section id="about">
  <h2>Tentang Kami</h2>
  <p class="text-muted">
    RHN Capital dikelola oleh individu muda yang disiplin, rasional,
    dan berorientasi pada pertumbuhan aset digital berkelanjutan.
  </p>
</section>

<section id="portfolio">
  <h2>Portofolio</h2>
  <div class="portfolio">
    <div class="card">
      <img src="https://assets.coingecko.com/coins/images/1/large/bitcoin.png" width="250">
      <h3>Bitcoin (BTC)</h3>
      <p class="text-muted">Alokasi: 100%</p>
      <br>
      <a href="https://www.coingecko.com/en/coins/bitcoin" target="_blank" class="btn">
        Lihat di CoinGecko
      </a>
    </div>
  </div>
</section>
      <div style="text-align:center;">
      <a href="ANALISA.html" class="btn">Analisa RHN Capital</a>
      </div>
<section id="contact">
  <h2>Kontak</h2>
  <div class="contact">
    <a href="https://wa.me/6285717426626" target="_blank">WhatsApp</a>
    <a href="https://instagram.com/huyrehan" target="_blank">Instagram</a>
    <a href="https://www.tiktok.com/@rehanhuy" target="_blank">Tiktok</a>
  </div>
</section>
<button onclick="window.open('https://wa.me/6285717426626?text=Halo%20RHN%20Capital,%20saya%20ingin%20melakukan%20pembayaran%20via%20GoPay.','_blank')" style="
width:100%;
padding:14px;
border:none;
border-radius:12px;
background:linear-gradient(135deg,#00c853,#1de9b6);
color:#000;
font-size:16px;
font-weight:600;
cursor:pointer;
box-shadow:0 8px 20px rgba(0,200,83,.35);
">
💳 Bayar via GoPay
</button>
<footer>
  © 2025 RHN Capital. All rights reserved.
</footer>

<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RHN Capital – Edukasi Premium</title>

<style>
body{
margin:0;
font-family:Inter,system-ui,Arial;
background:linear-gradient(180deg,#020617,#020617);
color:#e5e7eb;
}

.app{
max-width:420px;
margin:auto;
min-height:100vh;
padding:20px;
}

.card{
background:#020617;
border:1px solid #1f2937;
border-radius:18px;
padding:18px;
margin-bottom:16px;
box-shadow:0 20px 40px rgba(0,0,0,.6);
}

h1,h2{
margin:0 0 10px;
}

input{
width:100%;
padding:14px;
border-radius:12px;
border:none;
background:#020617;
border:1px solid #1f2937;
color:#fff;
margin-bottom:12px;
font-size:15px;
}

button{
width:100%;
padding:16px;
border:none;
border-radius:14px;
font-size:16px;
font-weight:600;
cursor:pointer;
}

.btn-primary{
background:#fbbf24;
color:#000;
}

.btn-green{
background:#16a34a;
color:#fff;
}

.btn-gray{
background:#1f2937;
color:#9ca3af;
}

.hidden{
display:none;
}

.footer{
text-align:center;
font-size:12px;
opacity:.5;
margin-top:30px;
}
</style>
</head>

<body>

<div class="app">

<!-- PAGE 1 -->
<div class="card" id="page-register">
<h1>RHN Capital</h1>
<p>Akses edukasi aset digital premium</p>

<input id="name" placeholder="Nama Lengkap">
<input id="contact" placeholder="WhatsApp / Email">

<button class="btn-primary" onclick="nextPayment()">Lanjut Pembayaran</button>
</div>

<!-- PAGE 2 -->
<div class="card hidden" id="page-payment">
<h2>Pembayaran</h2>
<p>Bayar via QRIS (GoPay, DANA, OVO, Mobile Banking)</p>

<button class="btn-green" onclick="openQRIS()">💳 Bayar via QRIS</button>

<button class="btn-gray" onclick="nextAccess()">Saya Sudah Bayar</button>
</div>

<!-- PAGE 3 -->
<div class="card hidden" id="page-access">
<h2>Masukkan Kode Akses</h2>
<input id="pin" placeholder="Kode Akses">

<button class="btn-primary" onclick="checkPIN()">Masuk</button>
</div>

<!-- PAGE 4 -->
<div class="card hidden" id="page-private">
<h2>📚 Edukasi RHN Capital</h2>
<p>
• Mindset Investor Disiplin<br>
• Tidak FOMO & Tidak Leverage<br>
• Strategi Jangka Panjang<br>
• Analisa Rasional Market
</p>

<p style="margin-top:10px;font-size:13px;opacity:.7">
Akses ini bersifat pribadi.
</p>
</div>

<div class="footer">
© 2025 RHN Capital
</div>

</div>

<script>
const QRIS_LINK = "https://gopay.co.id/app/scanqr?deeplink_source=request_money";
const ACCESS_PIN = "RHN2025";

function nextPayment(){
document.getElementById("page-register").classList.add("hidden");
document.getElementById("page-payment").classList.remove("hidden");
}

function openQRIS(){
window.open(QRIS_LINK,"_blank");
}

function nextAccess(){
document.getElementById("page-payment").classList.add("hidden");
document.getElementById("page-access").classList.remove("hidden");
}

function checkPIN(){
const pin = document.getElementById("pin").value;
if(pin === ACCESS_PIN){
document.getElementById("page-access").classList.add("hidden");
document.getElementById("page-private").classList.remove("hidden");
}else{
alert("Kode salah");
}
}
</script>

</body>
</html>
</body>
</html>
