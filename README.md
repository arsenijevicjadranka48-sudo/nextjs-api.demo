<!DOCTYPE html>
<html lang="sr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MCA2017 – Mašinska obrada</title>
<style>
body { font-family: Arial, sans-serif; margin:0; padding:0; background:#f9f9f9; color:#222; scroll-behavior:smooth; }
header { display: flex; justify-content: space-between; align-items: center; padding: 10px 20px; position: relative; background:#333; color:white; }
header .left { display: flex; align-items: center; gap: 10px; }
header .right { display: flex; align-items: center; gap: 15px; position: relative; }
nav { display: flex; gap: 15px; }
nav a { color:white; text-decoration:none; font-weight:bold; }
nav a:hover { text-decoration: underline; }

.lang-container {
  opacity: 0;             /* skrivena po defaultu */
  transition: opacity 0.3s ease;
  display: flex;
  gap: 5px;
  align-items: center;
}
header .right:hover .lang-container {
  opacity: 1;             /* pojavljuje se kad hover */
}

.lang-btn { 
  padding: 5px 10px; 
  border:none; 
  border-radius:5px; 
  cursor:pointer; 
  background:#555; 
  color:white; 
  display: flex;
  align-items: center;
  gap: 5px;
}
.lang-btn.active { background:#ff9800; color:#fff; }

section { padding:50px 20px; text-align:center; }
.card { background:#fff; padding:15px; margin:10px auto; max-width:600px; border-radius:10px; box-shadow:0 2px 10px rgba(0,0,0,0.1); text-align:left; }
</style>
</head>
<body>

<header>
  <div class="left">
    <img src="https://i.imgur.com/3g7nmJC.png" alt="MCA2017 Logo" id="logo" height="50">
    <strong>MCA2017 — Mašinska obrada</strong>
  </div>
  <div class="right">
    <nav>
      <a href="#about">O nama</a>
      <a href="#services">Usluge</a>
      <a href="#gallery">Galerija</a>
      <a href="#reviews">Recenzije</a>
      <a href="#contact">Kontakt</a>
    </nav>
    <div class="lang-container">
      <button class="lang-btn active" onclick="setLang('sr')">
        <img src="https://upload.wikimedia.org/wikipedia/commons/f/ff/Flag_of_Serbia.svg" alt="SR" width="20"> SR
      </button>
      <button class="lang-btn" onclick="setLang('en')">
        <img src="https://upload.wikimedia.org/wikipedia/en/a/ae/Flag_of_the_United_Kingdom.svg" alt="EN" width="20"> EN
      </button>
      <button class="lang-btn" onclick="setLang('de')">
        <img src="https://upload.wikimedia.org/wikipedia/en/b/ba/Flag_of_Germany.svg" alt="DE" width="20"> DE
      </button>
    </div>
  </div>
</header>

<section id="about"></section>
<section id="services"></section>
<section id="gallery"></section>
<section id="reviews"></section>
<section id="contact"></section>

<script>
// Funkcija za učitavanje sekcija iz fajlova po jeziku
let currentLang = 'sr';
function loadSection(id, file){
  fetch(file)
    .then(res=>res.text())
    .then(data=>document.getElementById(id).innerHTML = data)
    .catch(err=>document.getElementById(id).innerHTML='<p>Neuspešno učitavanje sekcije.</p>');
}
function loadAllSections(lang){
  loadSection('about', `about-${lang}.html`);
  loadSection('services', `services-${lang}.html`);
  loadSection('gallery', `gallery-${lang}.html`);
  loadSection('reviews', `reviews-${lang}.html`);
  loadSection('contact', `contact-${lang}.html`);
}

// Postavljanje jezika
function setLang(lang){
  currentLang = lang;
  loadAllSections(lang);
  document.querySelectorAll('.lang-btn').forEach(btn=>btn.classList.remove('active'));
  document.querySelector(`.lang-btn[onclick="setLang('${lang}')"]`).classList.add('active');
}

// Učitavanje početnog jezika
loadAllSections(currentLang);
</script>

</body>
</html>
