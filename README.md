<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FARHAN STORE</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Inter,sans-serif}
body{
background:linear-gradient(180deg,#020617,#0f172a);
color:#e5e7eb;
}

/* NAV */
header{
position:sticky;top:0;
background:rgba(2,6,23,.85);
backdrop-filter:blur(10px);
border-bottom:1px solid rgba(255,255,255,.05);
z-index:99
}
.nav{
max-width:1100px;margin:auto;
padding:18px 20px;
display:flex;justify-content:space-between;align-items:center
}
.logo{font-weight:700;color:#fbbf24}
.nav a{margin-left:18px;color:#cbd5f5;font-size:14px}

/* HERO */
.hero{
max-width:1100px;margin:auto;
padding:80px 20px;
display:grid;grid-template-columns:1.2fr 1fr;
gap:40px
}
.hero h1{font-size:40px}
.hero p{color:#94a3b8;margin-top:16px}

/* CARD */
.card{
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.06);
border-radius:20px;
padding:30px;
margin-bottom:30px;
transition:.4s
}
.card:hover{transform:translateY(-6px)}

/* BUTTON */
.btn{
display:inline-block;
padding:14px 26px;
border-radius:14px;
background:linear-gradient(135deg,#22c55e,#16a34a);
color:#000;
font-weight:600;
margin-top:20px;
cursor:pointer
}

/* CONTACT */
.contact{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px
}
.contact a{
background:rgba(255,255,255,.05);
border:1px solid rgba(255,255,255,.08);
border-radius:14px;
padding:18px;
text-align:center
}

/* QR MODAL */
.overlay{
position:fixed;inset:0;
background:rgba(0,0,0,.7);
display:none;
align-items:center;
justify-content:center;
z-index:999
}
.qr-box{
background:#fff;color:#000;
padding:20px;
border-radius:18px;
text-align:center;
animation:zoom .3s ease
}
.qr-box img{width:260px;margin:10px 0}
@keyframes zoom{from{scale:.8;opacity:0}to{scale:1;opacity:1}}

footer{
text-align:center;
padding:30px;
color:#94a3b8;
border-top:1px solid rgba(255,255,255,.05)
}

@media(max-width:900px){
.hero{grid-template-columns:1fr}
.hero h1{font-size:32px}
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

<section class="hero">
<div>
<h1>FARHAN STORE</h1>
<p>
Layanan joki Free Fire & Mobile Legends serta penyedia room wangi terpercaya.
Mengutamakan keamanan akun, transparansi, dan pelayanan profesional.
</p>
<button class="btn" onclick="openQR()">💳 Bayar via QRIS</button>
</div>

<div class="card">
<h3>Kenapa Pilih Kami?</h3>
<ul style="margin-top:12px;line-height:1.8">
<li>✅ Akun aman & privasi terjaga</li>
<li>⚡ Proses cepat & jelas</li>
<li>🤝 Support WhatsApp aktif</li>
<li>🎮 Fokus FF & ML</li>
</ul>
</div>
</section>

<section id="about" style="max-width:1100px;margin:auto;padding:20px">
<div class="card">
<h2>Tentang Kami</h2>
<p style="color:#94a3b8;margin-top:10px">
Farhan Store hadir sebagai partner gamer untuk membantu meningkatkan rank
dan pengalaman bermain secara aman dan efisien.
</p>
</div>
</section>

<section id="contact" style="max-width:1100px;margin:auto;padding:20px">
<h2>Kontak</h2>
<div class="contact">
<a href="https://wa.me/6285717426626" target="_blank">WhatsApp</a>
<a href="https://instagram.com/huyrehan" target="_blank">Instagram</a>
<a href="https://www.tiktok.com/@farhanstore86" target="_blank">TikTok</a>
</div>
</section>

<!-- QRIS MODAL -->
<div class="overlay" id="qris">
<div class="qr-box">
<h3>Scan QRIS</h3>
<img src="RHN LOGO.jpg" alt="QRIS">
<p>Setelah bayar, kirim bukti ke WhatsApp</p>
<button class="btn" onclick="closeQR()">Tutup</button>
</div>
</div>

<footer>
© 2025 FARHAN STORE — Joki FF & ML Terpercaya
</footer>

<script>
function openQR(){
document.getElementById("qris").style.display="flex"
}
function closeQR(){
document.getElementById("qris").style.display="none"
}
</script>

</body>
</html>
