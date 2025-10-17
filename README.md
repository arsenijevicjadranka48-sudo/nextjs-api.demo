<!DOCTYPE html>
<html lang="sr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Arsenijević – Usluga mašinske obrade</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background-color: #f3f3f3;
      color: #222;
      line-height: 1.6;
    }

    header {
      background-color: #222;
      color: #fff;
      text-align: center;
      padding: 50px 20px;
    }

    header h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
      letter-spacing: 1px;
    }

    nav {
      background-color: #005baa;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }

    nav a {
      color: #fff;
      padding: 15px 20px;
      text-decoration: none;
      transition: background 0.3s;
      font-weight: 500;
    }

    nav a:hover {
      background-color: #004480;
    }

    section {
      max-width: 1000px;
      margin: 40px auto;
      padding: 0 20px;
    }

    h2 {
      color: #005baa;
      margin-bottom: 15px;
      text-align: center;
      border-bottom: 2px solid #005baa;
      display: inline-block;
      padding-bottom: 5px;
    }

    .service {
      background: #fff;
      border-radius: 12px;
      padding: 25px;
      margin-bottom: 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    .service:hover {
      transform: translateY(-4px);
      box-shadow: 0 4px 14px rgba(0,0,0,0.15);
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 15px;
    }

    .gallery img {
      width: 100%;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .reviews {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .review {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .review strong {
      color: #005baa;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      background: #fff;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    input, textarea {
      padding: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
      font-size: 1em;
      width: 100%;
    }

    button {
      background-color: #005baa;
      color: #fff;
      border: none;
      padding: 12px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1em;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #004480;
    }

    footer {
      background-color: #222;
      color: #ccc;
      text-align: center;
      padding: 20px 10px;
      margin-top: 40px;
      font-size: 0.9em;
    }
  </style>
</head>
<body>

<header>
  <h1>Arsenijević – Usluga mašinske obrade</h1>
  <p>Preciznost, iskustvo i kvalitet u svakoj obradi metala</p>
</header>

<nav>
  <a href="#onama">O nama</a>
  <a href="#usluge">Usluge</a>
  <a href="#galerija">Galerija</a>
  <a href="#recenzije">Recenzije</a>
  <a href="#kontakt">Kontakt</a>
</nav>

<section id="onama">
  <h2>O nama</h2>
  <p>
    Firma <strong>Arsenijević</strong> bavi se preciznom mašinskom obradom više od 20 godina.
    Specijalizovani smo za glodanje, struganje, brušenje, erodiranje i lasersko sečenje metala.
    Naš tim stručnjaka garantuje kvalitet, tačnost i brzu isporuku svakog projekta.
  </p>
</section>

<section id="usluge">
  <h2>Usluge</h2>

  <div class="service">
    <h3>Glodanje</h3>
    <p>Visokoprecizno glodanje različitih materijala prema vašim zahtevima.</p>
  </div>

  <div class="service">
    <h3>Struganje</h3>
    <p>Profesionalna obrada na strugu – precizno oblikovanje metalnih delova.</p>
  </div>

  <div class="service">
    <h3>Ravno brušenje</h3>
    <p>Postižemo vrhunsku glatkoću površine i tačne dimenzije ravnim brušenjem.</p>
  </div>

  <div class="service">
    <h3>Obimno brušenje</h3>
    <p>Brušenje obimnih površina za visok nivo završne obrade i preciznosti.</p>
  </div>

  <div class="service">
    <h3>Erodiranje žica</h3>
    <p>Precizno sečenje pomoću žične erozije – idealno za složene oblike.</p>
  </div>

  <div class="service">
    <h3>Erodiranje elektroda</h3>
    <p>Izrada delova složenih oblika erozijom elektroda visoke tačnosti.</p>
  </div>

  <div class="service">
    <h3>Lasersko sečenje lima</h3>
    <p>Brzo i precizno lasersko sečenje čelika, aluminijuma i drugih metala.</p>
  </div>
</section>

<section id="galerija">
  <h2>Galerija</h2>
  <div class="gallery">
    <img src="https://via.placeholder.com/400x250?text=Glodanje" alt="Glodanje">
    <img src="https://via.placeholder.com/400x250?text=Struganje" alt="Struganje">
    <img src="https://via.placeholder.com/400x250?text=Brušenje" alt="Brušenje">
    <img src="https://via.placeholder.com/400x250?text=Erodiranje" alt="Erodiranje">
    <img src="https://via.placeholder.com/400x250?text=Lasersko+sečenje" alt="Lasersko sečenje">
  </div>
</section>

<section id="recenzije">
  <h2>Recenzije</h2>
  <div class="reviews">
    <div class="review">
      <strong>Petar M.</strong> ⭐⭐⭐⭐⭐  
      <p>Izuzetno kvalitetna usluga i tačnost u dogovoru. Preporuka svima!</p>
    </div>
    <div class="review">
      <strong>Marko L.</strong> ⭐⭐⭐⭐⭐  
      <p>Brza izrada i preciznost na visokom nivou. Svaka čast ekipi Arsenijević!</p>
    </div>
    <div class="review">
      <strong>Jovan K.</strong> ⭐⭐⭐⭐☆  
      <p>Odlična komunikacija i profesionalan pristup poslu.</p>
    </div>
  </div>
</section>

<section id="kontakt">
  <h2>Kontakt</h2>
  <form>
    <input type="text" placeholder="Vaše ime" required>
    <input type="email" placeholder="Vaš email" required>
    <textarea rows="5" placeholder="Vaša poruka..." required></textarea>
    <button type="submit">Pošalji poruku</button>
  </form>
</section>

<footer>
  © 2025 Arsenijević | Usluga mašinske obrade
</footer>

</body>
</html>
