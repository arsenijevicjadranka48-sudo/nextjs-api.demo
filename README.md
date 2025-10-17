<!DOCTYPE html>
<html lang="bs">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Arsenijević - Usluge mašinske obrade</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f8f9fa;
      color: #222;
      line-height: 1.6;
    }

    header {
      background-color: #1f2937;
      color: #fff;
      text-align: center;
      padding: 2rem 1rem;
    }

    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }

    nav {
      background-color: #111827;
      text-align: center;
      padding: 0.6rem 0;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      margin: 0 1rem;
      font-weight: 500;
    }

    nav a:hover {
      color: #38bdf8;
    }

    section {
      padding: 3rem 1rem;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      color: #1f2937;
      border-bottom: 2px solid #38bdf8;
      display: inline-block;
      padding-bottom: 0.3rem;
      margin-bottom: 1rem;
    }

    .services, .projects, .faq {
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      padding: 2rem;
      margin-bottom: 2rem;
    }

    .gallery img {
      width: 100%;
      max-width: 300px;
      border-radius: 10px;
      margin: 0.5rem;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    footer {
      background-color: #1f2937;
      color: #fff;
      text-align: center;
      padding: 1rem;
    }

    .review {
      background-color: #e5e7eb;
      border-left: 4px solid #38bdf8;
      margin: 1rem 0;
      padding: 1rem;
      border-radius: 6px;
    }

    .contact-info {
      background-color: #fff;
      border-radius: 10px;
      padding: 2rem;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .contact-info p {
      margin: 0.5rem 0;
    }

  </style>
</head>
<body>

  <header>
    <h1>Arsenijević</h1>
    <p>Profesionalne usluge mašinske obrade metala</p>
  </header>

  <nav>
    <a href="#onama">O nama</a>
    <a href="#usluge">Usluge</a>
    <a href="#projekti">Projekti</a>
    <a href="#galerija">Galerija</a>
    <a href="#recenzije">Recenzije</a>
    <a href="#kontakt">Kontakt</a>
  </nav>

  <section id="onama">
    <h2>O nama</h2>
    <p>Firma <strong>Arsenijević</strong> već više od 20 godina uspješno posluje u oblasti mašinske obrade metala. Naše iskustvo, preciznost i profesionalnost omogućavaju nam da realizujemo i najzahtjevnije projekte.</p>
    <p>Specijalizovani smo za glodanje, struganje, brušenje, erodiranje i druge procese visoke tačnosti. Naš tim koristi savremenu CNC tehnologiju i garantuje kvalitetnu isporuku u dogovorenim rokovima.</p>
  </section>

  <section id="usluge" class="services">
    <h2>Usluge</h2>
    <ul>
      <li>Glodanje – precizna obrada ravnih i zakrivljenih površina</li>
      <li>Struganje – izrada cilindričnih i konusnih elemenata</li>
      <li>Ravno i obimno brušenje – visoka preciznost i završna obrada</li>
      <li>Erodiranje (žica i elektroda) – kompleksni oblici s minimalnim tolerancijama</li>
      <li>Prototipna i serijska proizvodnja</li>
    </ul>

    <h3>Zašto odabrati nas</h3>
    <ul>
      <li><strong>Iskustvo i tradicija</strong> – preko dvije decenije u industriji.</li>
      <li><strong>Moderni CNC sistemi</strong> – preciznost i ponovljivost.</li>
      <li><strong>Brzi rokovi i pouzdanost</strong> – cijenimo vaše vrijeme.</li>
      <li><strong>Kontrola kvaliteta</strong> – svaki komad prolazi detaljnu inspekciju.</li>
    </ul>
  </section>

  <section id="projekti" class="projects">
    <h2>Projekti</h2>
    <p>Naši projekti uključuju širok spektar industrijskih rješenja:</p>
    <ul>
      <li>Izrada preciznih zupčanika i vratila</li>
      <li>Komponente za automobilske prototipove</li>
      <li>Matice i elementi za hidraulične sisteme</li>
      <li>Alati i nosači za lasersko sečenje</li>
      <li>Specijalne komponente za medicinske uređaje</li>
    </ul>
  </section>

  <section id="galerija" class="gallery">
    <h2>Galerija</h2>
    <p>Pogledajte dio naših proizvoda i procesa rada:</p>
    <div style="display:flex;flex-wrap:wrap;justify-content:center;">
      <img src="https://via.placeholder.com/300x200" alt="Mašinska obrada 1">
      <img src="https://via.placeholder.com/300x200" alt="Mašinska obrada 2">
      <img src="https://via.placeholder.com/300x200" alt="Mašinska obrada 3">
    </div>
  </section>

  <section id="recenzije">
    <h2>Recenzije</h2>
    <div class="review">
      <p>“Izuzetno zadovoljni kvalitetom izrade i tačnošću dimenzija. Topla preporuka!”</p>
      <p><strong>- Metal Inženjering d.o.o.</strong></p>
    </div>
    <div class="review">
      <p>“Profesionalna komunikacija i brza isporuka. Svaki dogovor ispoštovan.”</p>
      <p><strong>- TehnoServis Lukavac</strong></p>
    </div>
  </section>

  <section id="kontakt" class="contact-info">
    <h2>Kontakt</h2>
    <p><strong>Adresa:</strong> Industrijska zona bb, Lukavac</p>
    <p><strong>Telefon:</strong> +387 61 123 456</p>
    <p><strong>Email:</strong> info@arsenijevic.ba</p>
    <p><strong>Radno vrijeme:</strong> Pon–Pet 08:00 – 16:00</p>
  </section>

  <footer>
    <p>&copy; 2025 Arsenijević – Sva prava zadržana.</p>
  </footer>

</body>
</html>
