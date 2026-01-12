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
    <div class="logo">FARHAN STORE</div>
    <nav>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>
<img src="file_00000000d06471f88de72ec4ce9cac39.png" alt="Logo RHN" style="width:1000px;">
<section class="hero">
  <div>
    <h1>FARHAN STORE</h1>
    <p>
      FARHAN STORE adalah layanan independen yang berfokus pada jasa joki game Free Fire (FF) dan Mobile Legends (ML) serta penjualan room wangi terpercaya. Farhan Store mengedepankan pelayanan yang aman, cepat, dan transparan, dengan komitmen penuh terhadap kepuasan pelanggan.
Beroperasi dengan sistem yang rapi dan bertanggung jawab, Farhan Store mengutamakan keamanan akun, ketepatan waktu, serta hasil yang sesuai kesepakatan. Dengan pendekatan profesional dan komunikasi yang jelas, Farhan Store hadir sebagai solusi bagi pemain yang ingin meningkatkan performa permainan secara efisien dan terpercaya.
Berorientasi pada kepercayaan dan konsistensi, Farhan Store siap menjadi partner andalan bagi komunitas gamer FF dan ML.
    </p>
    
  </div>

 
</section>

<section id="about">
  <h2>Tentang Kami</h2>
  <p class="text-muted">
    Farhan Store adalah layanan joki FF & ML serta penjual room wangi yang mengutamakan kepercayaan, keamanan akun, dan pelayanan cepat dengan harga yang transparan.
  </p>
</section>

<section class="card fade-up">
  <h2>Kenapa Pilih Farhan Store?</h2>
  <ul>
    <li>✅ Akun aman & privasi terjaga</li>
    <li>⚡ Proses cepat & transparan</li>
    <li>🤝 Komunikasi jelas via WhatsApp</li>
    <li>🎮 Fokus FF & ML (bukan abal-abal)</li>
  </ul>
</section>

  <h2>FARHAN STORE</h2>
  <div class="portfolio">
    <div class="card">
      <img src="file_00000000d06471f88de72ec4ce9cac39.png" width="250">
      <h3>FARHAN STORE</h3>
     
    </div>
  </div>
      <div style="text-align:center;">
    
      </div>
<section id="contact">
  <h2>Kontak</h2>
  <div class="contact">
    <a href="https://wa.me/6285717426626" target="_blank">WhatsApp</a>
    <a href="https://instagram.com/huyrehan" target="_blank">Instagram</a>
    <a href="https://www.tiktok.com/@farhanstore86?_r=1&_t=ZS-92xb5ODYqyl" target="_blank">Tiktok</a>
  </div>
</section>
<button onclick="window.open('https://wa.me/6285717426626?text=Halo%20FARHAN%20STORE,%20saya%20ingin%20melakukan%20pembayaran.','_blank')" style="
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
💳 Bayar
</button>

<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FARHAN STORE – AKSES ROOM WANGI</title>

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
<h1>FARHAN STORE</h1>
<p>Akses ROOM WANGI</p>

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
<a href="ANALISA.html" class="btn">ROOM WANGI</a>

<p style="margin-top:10px;font-size:13px;opacity:.7">
Akses ini bersifat berbayar
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

<!-- ===== FARHAN STORE ULTRA ANIMATION ===== -->
<style>
/* CINEMATIC BACKGROUND */
body {
  background: radial-gradient(circle at top, #022c22, #020617 60%);
  animation: bgSlow 20s ease-in-out infinite;
}

@keyframes bgSlow {
  0% {background-position: 0% 0%;}
  50% {background-position: 100% 100%;}
  100% {background-position: 0% 0%;}
}

/* LOADER CINEMATIC */
#fs-loader {
  position: fixed;
  inset: 0;
  background: #020617;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 9999;
}

#fs-loader h1 {
  font-size: 28px;
  letter-spacing: 6px;
  color: #22c55e;
  animation: logoGlow 2.5s ease-in-out infinite;
}

@keyframes logoGlow {
  0% {opacity: .2; text-shadow: 0 0 0 #22c55e;}
  50% {opacity: 1; text-shadow: 0 0 25px #22c55e;}
  100% {opacity: .2; text-shadow: 0 0 0 #22c55e;}
}

/* CARD SUPER SLOW */
.card {
  background: rgba(15, 23, 42, 0.75);
  backdrop-filter: blur(18px);
  border-radius: 26px;
  padding: 26px;
  margin: 24px 0;
  transform: translateY(80px) scale(0.9);
  opacity: 0;
  transition: all 1.4s cubic-bezier(.16,1,.3,1);
  box-shadow: 0 0 0 rgba(34,197,94,0);
}

.card.show {
  transform: translateY(0) scale(1);
  opacity: 1;
  box-shadow: 0 0 50px rgba(34,197,94,0.2);
}

/* FLOAT EFFECT (HIDUP TERUS) */
.card.show {
  animation: floatCard 6s ease-in-out infinite;
}

@keyframes floatCard {
  0% {transform: translateY(0);}
  50% {transform: translateY(-6px);}
  100% {transform: translateY(0);}
}

/* BUTTON GOD-TIER */
.btn-premium {
  display: block;
  width: 100%;
  text-align: center;
  background: linear-gradient(135deg, #22c55e, #16a34a);
  color: #fff;
  padding: 20px;
  border-radius: 20px;
  font-weight: bold;
  letter-spacing: 1.5px;
  margin-top: 18px;
  animation: slowPulse 3.5s infinite;
  transition: all .35s ease;
}

.btn-premium:hover {
  transform: scale(1.08);
  box-shadow: 0 0 40px rgba(34,197,94,.9);
}

@keyframes slowPulse {
  0% {box-shadow: 0 0 0 rgba(34,197,94,0);}
  50% {box-shadow: 0 0 35px rgba(34,197,94,0.6);}
  100% {box-shadow: 0 0 0 rgba(34,197,94,0);}
}

/* TEXT FADE PREMIUM */
.fade-text {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeText 2.2s ease forwards;
}

@keyframes fadeText {
  to {opacity: 1; transform: translateY(0);}
}
</style>

<div id="fs-loader">
  <h1>FARHAN STORE</h1>
</div>

<script>
/* LOADER LEBIH LAMA (PREMIUM FEEL) */
window.addEventListener("load", () => {
  setTimeout(() => {
    document.getElementById("fs-loader")?.remove();
  }, 2500);
});

/* SCROLL ANIMATION SUPER HALUS */
const observer = new IntersectionObserver(entries => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add("show");
    }
  });
}, { threshold: 0.12 });

document.querySelectorAll(".card").forEach(card => observer.observe(card));
</script>
<!-- ===== END ULTRA ===== -->

<footer>
  © 2025 FARHAN STORE. JOKI FF DAN ML TERPERCAYA DAN ROOM WANGI 
</footer>



</body>
</html>
</body>
</html>
