<!DOCTYPE html>
<html lang="bs">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Arduino & Automatika - Projekti i Komponente</title>
  <style>
    * { scroll-behavior: smooth; margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: Arial, sans-serif; color: #222; background-color: #f5f5f5; }

    header {
      background: linear-gradient(45deg, #0059b3, #0080ff);
      color: white; text-align: center; padding: 80px 20px;
      background-image: url('mca.png'); background-size: cover; background-position: center;
      position: relative;
    }
    header::after {
      content: ""; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0, 0, 0, 0.5);
    }
    header h1, header p, header a { position: relative; z-index: 2; }
    header h1 { font-size: 2.5em; margin-bottom: 10px; }
    header p { font-size: 1.2em; margin-bottom: 20px; }
    header a {
      background: #ffcc00; color: #000; padding: 10px 20px; text-decoration: none;
      border-radius: 5px; font-weight: bold;
    }

    nav {
      display: flex; justify-content: center; gap: 20px; background: #003366; padding: 15px;
    }
    nav a {
      color: white; text-decoration: none; font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover { color: #ffcc00; }

    section {
      padding: 60px 20px; background: white; margin: 20px auto;
      max-width: 1000px; border-radius: 10px; box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    h2 { color: #003366; margin-bottom: 15px; }
    p { line-height: 1.6; margin-bottom: 20px; }

    .btn-back {
      display: inline-block; background: #003366; color: white; padding: 10px 15px;
      text-decoration: none; border-radius: 5px;
    }
    .btn-back:hover { background: #0059b3; }

    .gallery img {
      width: 150px; height: auto; margin: 10px; border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    .add-part {
      background: #ffcc00; color: #000; padding: 10px 20px;
      border: none; border-radius: 5px; font-weight: bold; cursor: pointer;
    }
    .add-part:hover { background: #ffd633; }

    #novaLista {
      margin-top: 15px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
    .dio {
      background: #e6f0ff;
      border: 1px solid #b3d1ff;
      border-radius: 6px;
      padding: 10px 15px;
      font-weight: bold;
      display: flex;
      align-items: center;
      justify-content: space-between;
      min-width: 180px;
    }
    .obrisi {
      background: red;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      padding: 3px 7px;
    }
  </style>
</head>
<body>

<header id="pocetna">
  <h1>Arduino & Automatika Projekti</h1>
  <p>Profesionalno programiranje i izrada automatizovanih sistema – od ideje do gotovog rješenja.</p>
  <a href="#o-nama">Saznaj više</a>
</header>

<nav>
  <a href="#o-nama">O nama</a>
  <a href="#usluge">Usluge</a>
  <a href="#projekti">Projekti</a>
  <a href="#dijelovi">Dijelovi</a>
  <a href="#recenzije">Recenzije</a>
  <a href="#kontakt">Kontakt</a>
</nav>

<section id="o-nama">
  <h2>O nama</h2>
  <p>Naš tim se bavi razvojem i implementacijom Arduino i industrijskih rješenja za automatizaciju procesa. 
     Više od 10 godina iskustva u industriji omogućava nam da realizujemo i najkompleksnije projekte — od upravljanja
     motorima i senzorima do kompletnog sistema daljinskog nadzora i regulacije.</p>
  <p>Posebnu pažnju posvećujemo kvalitetu, sigurnosti i energetskoj efikasnosti svakog projekta. Naš cilj je da
     pomognemo klijentima da modernizuju svoje proizvodne linije i smanje troškove kroz pametne i pouzdane tehnologije.</p>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<section id="usluge">
  <h2>Usluge</h2>
  <p>Nudimo kompletnu uslugu programiranja, projektovanja i izrade automatizovanih uređaja. 
     Naši projekti uključuju PLC i Arduino kontrolere, razvoj elektronskih ploča, programiranje senzora, releja,
     elektromotora i komunikaciju sa SCADA sistemima. Sve komponente pažljivo biramo kako bismo osigurali pouzdan rad.</p>
  <p>Uz svaku uslugu dobijate dokumentaciju, tehničku podršku i mogućnost kasnijeg nadogradnje sistema.</p>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<section id="projekti">
  <h2>Projekti</h2>
  <p>Naši projekti obuhvataju širok spektar aplikacija: od sistema za automatsko navodnjavanje i detekciju plina, 
     do kontrole temperature i osvjetljenja u industrijskim pogonima. Svaki projekat je jedinstven i prilagođen specifičnim potrebama klijenta.</p>
  <div class="gallery">
    <img src="https://upload.wikimedia.org/wikipedia/commons/8/87/Arduino_Uno_-_R3.jpg" alt="Arduino Uno">
    <img src="https://upload.wikimedia.org/wikipedia/commons/4/4b/Arduino_Mega_2560_R3.jpg" alt="Arduino Mega">
    <img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Relay_module_4_channel.jpg" alt="Relej modul">
  </div>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<section id="dijelovi">
  <h2>Prodaja dijelova</h2>
  <p>U našoj ponudi možete pronaći Arduino ploče, senzore, motore, releje, žice, napajanja i druge komponente potrebne 
     za izradu automatizovanih projekata. Kvalitetne komponente, brza isporuka i mogućnost podrške prilikom odabira dijelova.</p>
  <button class="add-part" onclick="dodajDio()">Dodaj novi dio</button>
  <div id="novaLista"></div>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<section id="recenzije">
  <h2>Recenzije korisnika</h2>
  <p>⭐⭐⭐⭐⭐ “Izuzetno profesionalan pristup! Sistem radi bez greške već godinu dana.” – Marko P.</p>
  <p>⭐⭐⭐⭐⭐ “Preporučujem svakome ko želi kvalitetnu automatiku po razumnoj cijeni.” – Jasmin K.</p>
  <p>⭐⭐⭐⭐ “Odlična komunikacija i podrška nakon završetka projekta.” – Amra D.</p>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<section id="kontakt">
  <h2>Kontakt</h2>
  <p>Želite saradnju ili imate ideju za projekat? Pošaljite nam poruku na e-mail: <b>info@automatika-pro.site</b>  
     ili nas kontaktirajte putem društvenih mreža. Na svaki upit odgovaramo u roku od 24 sata.</p>
  <a class="btn-back" href="#pocetna">Nazad na početak</a>
</section>

<script>
  function ucitajDijelove() {
    const sacuvani = JSON.parse(localStorage.getItem("dijelovi") || "[]");
    sacuvani.forEach(dodajDioNaStranicu);
  }

  function dodajDio() {
    const ime = prompt("Unesite naziv dijela:");
    if (ime) {
      dodajDioNaStranicu(ime);
      const dijelovi = JSON.parse(localStorage.getItem("dijelovi") || "[]");
      dijelovi.push(ime);
      localStorage.setItem("dijelovi", JSON.stringify(dijelovi));
    }
  }

  function dodajDioNaStranicu(ime) {
    const novaLista = document.getElementById("novaLista");
    const div = document.createElement("div");
    div.className = "dio";
    div.innerHTML = `${ime} <button class="obrisi" onclick="obrisiDio(this, '${ime}')">x</button>`;
    novaLista.appendChild(div);
  }

  function obrisiDio(btn, ime) {
    btn.parentElement.remove();
    let dijelovi = JSON.parse(localStorage.getItem("dijelovi") || "[]");
    dijelovi = dijelovi.filter(d => d !== ime);
    localStorage.setItem("dijelovi", JSON.stringify(dijelovi));
  }

  window.onload = ucitajDijelove;
</script>

</body>
</html>
