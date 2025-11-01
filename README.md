<!DOCTYPE html>
<html lang="bs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arduino Projekti - Adis Halilović</title>
    <style>
        /* Osnovni stilovi */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #1e90ff, #00bfff);
            color: white;
            padding: 60px 20px;
            text-align: center;
            animation: fadeIn 1.5s;
        }

        header h1 {
            margin: 0;
            font-size: 3em;
        }

        header p {
            font-size: 1.2em;
            margin-top: 10px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav a {
            color: white;
            padding: 15px 25px;
            text-decoration: none;
            text-transform: uppercase;
            transition: background 0.3s;
        }

        nav a:hover {
            background-color: #1e90ff;
        }

        section {
            padding: 60px 20px;
            max-width: 1200px;
            margin: auto;
        }

        h2 {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        h2::after {
            content: '';
            width: 60px;
            height: 4px;
            background-color: #1e90ff;
            display: block;
            margin: 10px auto 0 auto;
            border-radius: 2px;
        }

        .services, .projects {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .card {
            background-color: white;
            border-radius: 12px;
            padding: 25px;
            margin: 10px;
            width: 300px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 24px rgba(0,0,0,0.2);
        }

        .card h3 {
            margin-top: 0;
            color: #1e90ff;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 50px;
        }

        input, textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border-radius: 6px;
            border: 1px solid #ccc;
        }

        button {
            background-color: #1e90ff;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            border-radius: 6px;
            font-size: 1em;
            transition: background 0.3s;
        }

        button:hover {
            background-color: #0b63c7;
        }

        /* Animacije */
        @keyframes fadeIn {
            from {opacity: 0; transform: translateY(-20px);}
            to {opacity: 1; transform: translateY(0);}
        }

        .project-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }

    </style>
</head>
<body>

<header>
    <h1>Adis Halilović - Arduino Projekti</h1>
    <p>Programiranje i kompletno projektovanje Arduino i industrijskih sistema</p>
</header>

<nav>
    <a href="#about">O meni</a>
    <a href="#services">Usluge</a>
    <a href="#projects">Projekti</a>
    <a href="#contact">Kontakt</a>
</nav>

<section id="about">
    <h2>O meni</h2>
    <p>Zovem se Adis Halilović i nudim profesionalne usluge programiranja Arduino sistema i kompletnog projektovanja elektronskih i mehaničkih rješenja. Specijalizovan sam za industrijske i kućne projekte, uključujući automatizaciju, IoT rješenja i robotske sisteme. Moj cilj je da svaki projekt bude prilagođen klijentu i funkcionalan po svim standardima.</p>
</section>

<section id="services">
    <h2>Usluge</h2>
    <div class="services">
        <div class="card">
            <h3>Programiranje Arduino</h3>
            <p>Pisanje koda za različite Arduino projekte, uključujući senzore, motore, LED matrice i industrijske sisteme.</p>
        </div>
        <div class="card">
            <h3>Projektovanje Kompletnog Sistema</h3>
            <p>Dizajn električnih i mehaničkih komponenti, PCB layout, integracija senzora i aktuatora.</p>
        </div>
        <div class="card">
            <h3>Automatizacija i IoT</h3>
            <p>Pametni industrijski sistemi i IoT rješenja za monitoring, kontrolu i optimizaciju procesa.</p>
        </div>
    </div>
</section>

<section id="projects">
    <h2>Projekti</h2>
    <div class="projects">
        <div class="card">
            <img src="https://via.placeholder.com/300x180?text=Automatski+Navodnjivač" alt="Automatski Navodnjivač" class="project-img">
            <h3>Automatski Navodnjivač</h3>
            <p>Arduino projekt za automatsko navodnjavanje industrijskih i poljoprivrednih površina sa senzorima vlage tla.</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x180?text=Robotska+Ruka" alt="Robotska Ruka" class="project-img">
            <h3>Robotska Ruka za Industriju</h3>
            <p>Programirana robotska ruka za industrijske procese – pakovanje, montaža i precizna manipulacija dijelovima.</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x180?text=Pametna+Kuća" alt="Pametna Kuća" class="project-img">
            <h3>Pametna Kuća i Industrijski Monitoring</h3>
            <p>IoT sistem za kontrolu rasvjete, temperature, sigurnosnih sistema i industrijskog nadzora putem mobilne aplikacije.</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x180?text=Automatizacija+Mašina" alt="Automatizacija Mašina" class="project-img">
            <h3>Automatizacija Mašina</h3>
            <p>Kompletno rješenje za automatizaciju proizvodnih linija i kontrolu mašina pomoću Arduino i PLC integracije.</p>
        </div>
        <div class="card">
            <img src="https://via.placeholder.com/300x180?text=Pametni+Skladišni+Sistem" alt="Pametni Skladišni Sistem" class="project-img">
            <h3>Pametni Skladišni Sistem</h3>
            <p>Sistem za praćenje inventara, automatsko sortiranje i kontrolu skladišnih procesa u industriji.</p>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Kontakt</h2>
    <form action="mailto:your.email@example.com" method="post" enctype="text/plain">
        <input type="text" name="name" placeholder="Vaše ime" required>
        <input type="email" name="email" placeholder="Vaš email" required>
        <textarea name="message" rows="5" placeholder="Vaša poruka" required></textarea>
        <button type="submit">Pošalji</button>
    </form>
</section>

<footer>
    <p>&copy; 2025 Adis Halilović | Sva prava zadržana</p>
</footer>

</body>
</html>
