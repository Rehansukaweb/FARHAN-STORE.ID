
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RHN Capital App</title>

<!-- ===================== -->
<!-- GLOBAL STYLE -->
<!-- ===================== -->
<style>

/* RESET */
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Inter,Arial,sans-serif;
}

/* ROOT */
:root{
  --bg:#020617;
  --panel:#020617;
  --card:#020617;
  --border:rgba(255,255,255,0.06);
  --text:#e5e7eb;
  --muted:#9ca3af;
  --blue:#2563eb;
  --green:#16a34a;
  --yellow:#facc15;
}

/* BODY */
body{
  background:linear-gradient(180deg,#020617,#020617);
  color:var(--text);
  height:100vh;
  overflow:hidden;
}

/* APP CONTAINER */
.app{
  display:flex;
  flex-direction:column;
  height:100vh;
  max-width:480px;
  margin:auto;
  border-left:1px solid var(--border);
  border-right:1px solid var(--border);
}

/* HEADER */
header{
  height:56px;
  display:flex;
  align-items:center;
  justify-content:center;
  border-bottom:1px solid var(--border);
  background:#020617;
  font-weight:700;
  letter-spacing:1px;
}

/* PAGE WRAPPER */
.pages{
  flex:1;
  overflow-y:auto;
  scroll-behavior:smooth;
}

/* PAGE */
.page{
  display:none;
  padding:16px;
  animation:fade .3s ease;
}
.page.active{
  display:block;
}

/* CARD */
.card{
  background:#020617;
  border:1px solid var(--border);
  border-radius:14px;
  padding:16px;
  margin-bottom:14px;
}
.card h3{
  margin-bottom:6px;
  font-size:16px;
}
.card p{
  font-size:14px;
  color:var(--muted);
}

/* BUTTON */
.btn{
  display:block;
  width:100%;
  padding:14px;
  margin-top:10px;
  border-radius:12px;
  border:none;
  background:var(--blue);
  color:white;
  font-weight:600;
  cursor:pointer;
}
.btn.green{background:var(--green)}
.btn.gray{background:#374151}
.btn.yellow{background:var(--yellow);color:#000}

/* NAV BAR */
nav{
  height:60px;
  display:flex;
  border-top:1px solid var(--border);
  background:#020617;
}
nav button{
  flex:1;
  background:none;
  border:none;
  color:var(--muted);
  font-size:11px;
}
nav button.active{
  color:var(--blue);
  font-weight:600;
}

/* LIST */
.list{
  list-style:none;
}
.list li{
  padding:12px 0;
  border-bottom:1px solid var(--border);
  font-size:14px;
}

/* MODULE */
.module{
  padding:12px;
  border-radius:10px;
  background:#020617;
  border:1px solid var(--border);
  margin-bottom:12px;
}

/* ANIMATION */
@keyframes fade{
  from{opacity:0;transform:translateY(8px)}
  to{opacity:1;transform:none}
}

</style>
</head>

<body>

<div class="app">

<!-- ===================== -->
<!-- HEADER -->
<!-- ===================== -->
<header>
  RHN CAPITAL
</header>

<!-- ===================== -->
<!-- PAGES -->
<!-- ===================== -->
<div class="pages">

<!-- HOME -->
<section id="home" class="page active">
  <div class="card">
    <h3>Selamat Datang</h3>
    <p>Aplikasi edukasi aset digital berbasis disiplin & rasionalitas.</p>
  </div>

  <div class="card">
    <h3>Akses Cepat</h3>
    <button class="btn" onclick="openPage('modules')">📘 Modul Edukasi</button>
    <button class="btn gray" onclick="openPage('analysis')">📊 Analisa</button>
    <button class="btn green" onclick="openPage('payment')">💳 Pembayaran</button>
  </div>

  <div class="card">
    <p><b>Prinsip:</b><br>
    Tidak FOMO. Tidak Leverage. Jangka Panjang.</p>
  </div>
</section>

<!-- MODULES -->
<section id="modules" class="page">
  <div class="card">
    <h3>Modul Edukasi</h3>
    <p>Materi singkat, padat, konsisten.</p>
  </div>

  <div class="module">
    <b>Modul 01 – Mindset</b>
    <p>Disiplin > Profit</p>
  </div>

  <div class="module">
    <b>Modul 02 – Bitcoin</b>
    <p>Supply tetap, anti inflasi.</p>
  </div>

  <div class="module">
    <b>Modul 03 – Risiko</b>
    <p>Jangan bertaruh masa depan.</p>
  </div>

  <button class="btn yellow" onclick="alert('Modul baru akan ditambahkan')">
    ➕ Tambah Modul
  </button>
</section>

<!-- ANALYSIS -->
<section id="analysis" class="page">
  <div class="card">
    <h3>Analisa RHN Capital</h3>
    <p>Analisa bukan sinyal.</p>
  </div>

  <ul class="list">
    <li>Status Market: WAIT</li>
    <li>Fokus: Akumulasi</li>
    <li>Timeframe: Panjang</li>
  </ul>
</section>

<!-- PAYMENT -->
<section id="payment" class="page">
  <div class="card">
    <h3>Pembayaran</h3>
    <p>Dukungan pengembangan edukasi.</p>
    <button class="btn green" onclick="openPayment()">Bayar via WhatsApp</button>
  </div>
</section>

<!-- PROFILE -->
<section id="profile" class="page">
  <div class="card">
    <h3>Tentang RHN Capital</h3>
    <p>Entitas edukasi aset digital independen.</p>
  </div>
</section>

</div>

<!-- ===================== -->
<!-- NAV -->
<!-- ===================== -->
<nav>
  <button class="active" onclick="nav('home',this)">Home</button>
  <button onclick="nav('modules',this)">Modul</button>
  <button onclick="nav('analysis',this)">Analisa</button>
  <button onclick="nav('profile',this)">Profil</button>
</nav>

</div>

<!-- ===================== -->
<!-- SCRIPT -->
<!-- ===================== -->
<script>

function openPage(id){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.getElementById(id).classList.add('active');
}

function nav(id,el){
  openPage(id);
  document.querySelectorAll('nav button').forEach(b=>b.classList.remove('active'));
  el.classList.add('active');
}

function openPayment(){
  window.open("https://wa.me/6285717826626","_blank");
}

</script>
<!-- ===================== -->
<!-- PART 2 : MODULE ENGINE -->
<!-- ===================== -->

<style>
/* MODULE LIST */
.module-list{
  margin-top:12px;
}
.module-item{
  padding:14px;
  border-radius:12px;
  border:1px solid var(--border);
  margin-bottom:10px;
  cursor:pointer;
  background:#020617;
  transition:.2s;
}
.module-item:hover{
  border-color:var(--blue);
}
.module-item b{
  font-size:14px;
}
.module-item span{
  font-size:12px;
  color:var(--muted);
}

/* MODULE DETAIL */
.module-detail{
  line-height:1.7;
}
.module-detail h4{
  margin-bottom:10px;
}
.module-detail p{
  font-size:14px;
  color:var(--text);
}

/* BACK BUTTON */
.back-btn{
  margin-bottom:14px;
  background:#374151;
}
</style>

<script>
// =====================
// MODULE DATA
// =====================
const modules = [
  {
    id:1,
    title:"Mindset Investor",
    content:[
      "Fokus pada proses, bukan hasil instan.",
      "Disiplin mengalahkan kecerdasan.",
      "Loss adalah biaya belajar."
    ]
  },
  {
    id:2,
    title:"Kenapa Bitcoin",
    content:[
      "Supply tetap dan transparan.",
      "Tidak dikontrol pemerintah.",
      "Aset lindung nilai jangka panjang."
    ]
  },
  {
    id:3,
    title:"Manajemen Risiko",
    content:[
      "Jangan all-in.",
      "Jaga modal lebih penting dari profit.",
      "Risiko kecil, konsisten."
    ]
  },
  {
    id:4,
    title:"Mental Saat Market Turun",
    content:[
      "Turun adalah fase.",
      "Market selalu siklikal.",
      "Orang sabar menang."
    ]
  },
  {
    id:5,
    title:"Kesalahan Pemula",
    content:[
      "Overtrade.",
      "FOMO.",
      "Tidak punya rencana."
    ]
  }
];

// =====================
// RENDER MODULE LIST
// =====================
function renderModules(){
  const container = document.getElementById("moduleList");
  container.innerHTML = "";
  modules.forEach(m=>{
    container.innerHTML += `
      <div class="module-item" onclick="openModule(${m.id})">
        <b>Modul ${m.id} – ${m.title}</b><br>
        <span>Klik untuk membaca</span>
      </div>
    `;
  });
}

// =====================
// OPEN MODULE DETAIL
// =====================
function openModule(id){
  const module = modules.find(m=>m.id===id);
  if(!module) return;

  let html = `
    <button class="btn back-btn" onclick="backToModules()">← Kembali</button>
    <div class="card module-detail">
      <h4>${module.title}</h4>
  `;

  module.content.forEach(p=>{
    html += `<p>• ${p}</p>`;
  });

  html += `</div>`;

  document.getElementById("modules").innerHTML = html;
}

// =====================
// BACK TO MODULE LIST
// =====================
function backToModules(){
  document.getElementById("modules").innerHTML = `
    <div class="card">
      <h3>Modul Edukasi</h3>
      <p>Materi singkat, padat, konsisten.</p>
    </div>
    <div id="moduleList" class="module-list"></div>
  `;
  renderModules();
}

// AUTO LOAD MODULES
document.addEventListener("DOMContentLoaded",()=>{
  if(document.getElementById("moduleList")){
    renderModules();
  }
});
</script>

<!-- ===================== -->
<!-- END PART 2 -->
<!-- ===================== -->
<!-- ========================= -->
<!-- APP ENGINE v3 -->
<!-- ========================= -->
<script>
/* =========================
   GLOBAL APP STATE
========================= */
const AppState = {
  user: {
    name: "Guest",
    loggedIn: false,
    balance: 0
  },
  modules: [],
  activeModule: null
};

/* =========================
   LOCAL STORAGE ENGINE
========================= */
const Storage = {
  save(key, value) {
    localStorage.setItem(key, JSON.stringify(value));
  },
  load(key, defaultValue) {
    const data = localStorage.getItem(key);
    return data ? JSON.parse(data) : defaultValue;
  }
};

// Load saved state
Object.assign(AppState, Storage.load("APP_STATE", AppState));

/* =========================
   UI HELPER
========================= */
function $(selector) {
  return document.querySelector(selector);
}
function $all(selector) {
  return document.querySelectorAll(selector);
}

/* =========================
   NOTIFICATION SYSTEM
========================= */
function notify(text, type="info") {
  const box = document.createElement("div");
  box.className = `toast ${type}`;
  box.innerText = text;
  document.body.appendChild(box);

  setTimeout(() => box.classList.add("show"), 50);
  setTimeout(() => {
    box.classList.remove("show");
    setTimeout(() => box.remove(), 300);
  }, 3000);
}

/* =========================
   MODULE SYSTEM
========================= */
function registerModule(id, title, content) {
  AppState.modules.push({ id, title, content });
  renderModules();
  Storage.save("APP_STATE", AppState);
}

function renderModules() {
  const container = $("#moduleList");
  if (!container) return;
  container.innerHTML = "";

  AppState.modules.forEach(m => {
    const btn = document.createElement("button");
    btn.className = "module-btn";
    btn.innerText = m.title;
    btn.onclick = () => openModule(m.id);
    container.appendChild(btn);
  });
}

function openModule(id) {
  const module = AppState.modules.find(m => m.id === id);
  if (!module) return;

  AppState.activeModule = id;
  $("#moduleContent").innerHTML = module.content;
  Storage.save("APP_STATE", AppState);
}

/* =========================
   USER SYSTEM
========================= */
function login(name) {
  AppState.user.name = name;
  AppState.user.loggedIn = true;
  Storage.save("APP_STATE", AppState);
  notify(`Selamat datang, ${name}`, "success");
  updateUserUI();
}

function logout() {
  AppState.user.loggedIn = false;
  Storage.save("APP_STATE", AppState);
  notify("Logout berhasil");
  updateUserUI();
}

function updateUserUI() {
  const el = $("#userName");
  if (!el) return;
  el.innerText = AppState.user.loggedIn ? AppState.user.name : "Guest";
}

/* =========================
   PAYMENT SIMULATION
========================= */
function addBalance(amount) {
  AppState.user.balance += amount;
  Storage.save("APP_STATE", AppState);
  notify(`Saldo bertambah Rp${amount}`, "success");
  updateBalanceUI();
}

function updateBalanceUI() {
  const el = $("#userBalance");
  if (!el) return;
  el.innerText = "Rp " + AppState.user.balance.toLocaleString("id-ID");
}

/* =========================
   APP INIT
========================= */
document.addEventListener("DOMContentLoaded", () => {
  updateUserUI();
  updateBalanceUI();
  renderModules();

  if (AppState.modules.length === 0) {
    // Default modules
    registerModule(
      "edu-bitcoin",
      "Edukasi Bitcoin",
      "<h2>Bitcoin Dasar</h2><p>Bitcoin adalah aset digital terdesentralisasi.</p>"
    );
    registerModule(
      "edu-risk",
      "Manajemen Risiko",
      "<h2>Risk Management</h2><p>Gunakan maksimal 1-2% per trade.</p>"
    );
  }
});
</script>

<style>
:root{
  --bg:#0b1220;
  --card:#121a2f;
  --accent:#f5b942;
  --text:#eaeaf0;
  --muted:#9aa0b3;
}

*{box-sizing:border-box}
body{
  margin:0;
  background:var(--bg);
  color:var(--text);
  font-family:Inter,system-ui,sans-serif;
}

/* HEADER */
.app-header{
  padding:16px;
  font-size:20px;
  font-weight:700;
  text-align:center;
  border-bottom:1px solid #1f2742;
}

/* PAGE */
.page{
  display:none;
  padding:16px;
  animation:fade .25s ease;
}
.page.active{display:block}

@keyframes fade{
  from{opacity:0;transform:translateY(10px)}
  to{opacity:1;transform:none}
}

/* CARD */
.card{
  background:var(--card);
  border-radius:16px;
  padding:16px;
  margin-bottom:16px;
  box-shadow:0 10px 30px rgba(0,0,0,.4);
}
.card h3{margin:0 0 8px}
.card p{margin:0;color:var(--muted)}

/* BUTTON */
.btn{
  width:100%;
  padding:14px;
  border:none;
  border-radius:12px;
  background:var(--accent);
  font-weight:700;
  cursor:pointer;
}
.btn.dark{
  background:#1f2742;
  color:var(--text);
}

/* MODULE LIST */
.module-btn{
  width:100%;
  padding:14px;
  border-radius:12px;
  background:#1f2742;
  color:var(--text);
  border:none;
  margin-bottom:10px;
}

/* BOTTOM NAV */
.bottom-nav{
  position:fixed;
  bottom:0;
  left:0;
  right:0;
  height:64px;
  background:#0e162b;
  display:flex;
  border-top:1px solid #1f2742;
}
.bottom-nav button{
  flex:1;
  background:none;
  border:none;
  color:var(--muted);
  font-size:12px;
}
.bottom-nav button.active{
  color:var(--accent);
  font-weight:700;
}

/* TOAST */
.toast{
  position:fixed;
  bottom:80px;
  left:50%;
  transform:translateX(-50%) scale(.9);
  background:#1f2742;
  padding:12px 18px;
  border-radius:10px;
  opacity:0;
  transition:.3s;
}
.toast.show{opacity:1;transform:translateX(-50%) scale(1)}
.toast.success{background:#1e7f4f}
</style>

<div class="app-header">
  RHN Capital App
</div>

<!-- HOME -->
<div id="home" class="page active">
  <div class="card">
    <h3>Selamat Datang</h3>
    <p>User: <b id="userName">Guest</b></p>
    <p>Saldo: <b id="userBalance">Rp 0</b></p>
  </div>

  <button class="btn" onclick="addBalance(10000)">Tambah Saldo (Demo)</button>
</div>

<!-- EDUKASI -->
<div id="edu" class="page">
  <div class="card">
    <h3>Modul Edukasi</h3>
    <div id="moduleList"></div>
  </div>
  <div class="card" id="moduleContent">
    <p>Pilih modul untuk membaca</p>
  </div>
</div>

<!-- PAYMENT -->
<div id="pay" class="page">
  <div class="card">
    <h3>Pembayaran</h3>
    <p>Akses pembayaran eksternal</p>
    <button class="btn" onclick="openPayment()">Buka WhatsApp</button>
  </div>
</div>

<!-- PROFILE -->
<div id="profile" class="page">
  <div class="card">
    <h3>Akun</h3>
    <button class="btn dark" onclick="login('Rehan')">Login</button>
    <button class="btn dark" onclick="logout()">Logout</button>
  </div>
</div>

<!-- BOTTOM NAV -->
<div class="bottom-nav">
  <button class="active" onclick="nav('home',this)">Home</button>
  <button onclick="nav('edu',this)">Edukasi</button>
  <button onclick="nav('pay',this)">Pay</button>
  <button onclick="nav('profile',this)">Profil</button>
</div>

<script>
function nav(id,el){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.getElementById(id).classList.add('active');

  document.querySelectorAll('.bottom-nav button')
    .forEach(b=>b.classList.remove('active'));
  el.classList.add('active');
}

function openPayment(){
  window.open("https://wa.me/6285717426626","_blank");
}
</script>
<!-- LOGIN MODAL -->
<div id="loginModal" style="display:none;position:fixed;inset:0;background:#0008">
  <div style="max-width:360px;margin:15% auto;background:#121a2f;padding:20px;border-radius:16px">
    <h3>Login</h3>
    <input id="email" placeholder="Email" style="width:100%;padding:12px;margin:8px 0">
    <input id="pass" type="password" placeholder="Password" style="width:100%;padding:12px;margin:8px 0">
    <button class="btn" onclick="fakeLogin()">Masuk</button>
  </div>
</div>

<script>
function fakeLogin(){
  localStorage.setItem("user","Rehan");
  document.getElementById("userName").innerText="Rehan";
  document.getElementById("loginModal").style.display="none";
}
</script>
</body>
</html>
