<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nolhan Masson | Dépannage Informatique & Rachat Cartouches</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #0056b3; /* Bleu rassurant */
            --secondary: #28a745; /* Vert pour le rachat/argent */
            --dark: #333;
            --light: #f4f4f4;
            --white: #ffffff;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Roboto', sans-serif; line-height: 1.6; color: var(--dark); background: var(--light); }
        a { text-decoration: none; color: inherit; }

        /* HEADER */
        header {
            background: var(--white);
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            z-index: 100;
        }
        
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1100px;
            margin: auto;
            padding: 15px 20px;
        }

        .logo { font-size: 1.5rem; font-weight: 700; color: var(--primary); }
        .logo span { color: var(--dark); }

        .nav-btn {
            background: var(--primary);
            color: var(--white);
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: bold;
        }
        .nav-btn:hover { background: #004494; }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1597852074816-d933c7d2b988?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
        }

        .hero h1 { font-size: 3rem; margin-bottom: 20px; }
        .hero p { font-size: 1.2rem; margin-bottom: 30px; }
        
        .cta-buttons { display: flex; gap: 20px; justify-content: center; flex-wrap: wrap; }
        
        .btn { padding: 12px 30px; border-radius: 5px; font-weight: bold; cursor: pointer; border: none; }
        .btn-primary { background: var(--primary); color: var(--white); }
        .btn-secondary { background: var(--secondary); color: var(--white); }
        .btn:hover { opacity: 0.9; transform: scale(1.05); transition: 0.3s; }

        /* SERVICES */
        .services { padding: 80px 20px; max-width: 1100px; margin: auto; }
        .section-title { text-align: center; margin-bottom: 50px; font-size: 2.2rem; color: var(--primary); }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: var(--white);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            text-align: center;
            border-top: 5px solid var(--primary);
        }

        .card-green { border-top: 5px solid var(--secondary); }

        .icon { font-size: 3rem; margin-bottom: 20px; }
        .card h3 { margin-bottom: 15px; font-size: 1.5rem; }
        .price-tag { 
            display: inline-block; 
            background: var(--secondary); 
            color: white; 
            padding: 5px 15px; 
            border-radius: 20px; 
            margin-top: 15px; 
            font-weight: bold; 
        }

        /* CONTACT & LOCALISATION */
        .contact-section { background: var(--dark); color: var(--white); padding: 60px 20px; text-align: center; }
        .contact-info { margin-top: 30px; display: flex; justify-content: center; gap: 40px; flex-wrap: wrap; }
        .contact-item { display: flex; flex-direction: column; align-items: center; }
        .contact-item i { font-size: 2rem; margin-bottom: 10px; color: var(--primary); }

        /* FOOTER */
        footer { text-align: center; padding: 20px; background: #222; color: #aaa; font-size: 0.9rem; }

        @media(max-width: 768px) {
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <header>
        <div class="navbar">
            <div class="logo">Nolhan<span>Masson</span></div>
            <a href="tel:0600000000" class="nav-btn"><i class="fas fa-phone-alt"></i> Me contacter</a>
        </div>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Vos soucis informatiques,<br>ma solution.</h1>
            <p>Dépannage à domicile & Rachat de cartouches d'encre usagées.</p>
            <div class="cta-buttons">
                <a href="#services" class="btn btn-primary">Voir mes services</a>
                <a href="#rachat" class="btn btn-secondary">Vendre mes cartouches</a>
            </div>
        </div>
    </section>

    <section id="services" class="services">
        <h2 class="section-title">Mes Services</h2>
        <div class="service-grid">
            
            <div class="card">
                <div class="icon" style="color: var(--primary);"><i class="fas fa-tools"></i></div>
                <h3>Dépannage Informatique</h3>
                <p>Votre ordinateur est lent ? Vous avez un virus ? Je me déplace à votre domicile pour réparer vos PC fixes et portables.</p>
                <ul style="list-style: none; margin-top: 15px; text-align: left; padding-left: 20px;">
                    <li><i class="fas fa-check" style="color:green"></i> Nettoyage virus & lenteurs</li>
                    <li><i class="fas fa-check" style="color:green"></i> Installation Windows / Logiciels</li>
                    <li><i class="fas fa-check" style="color:green"></i> Configuration Imprimante / Box</li>
                </ul>
            </div>

            <div class="card card-green" id="rachat">
                <div class="icon" style="color: var(--secondary);"><i class="fas fa-recycle"></i></div>
                <h3>Rachat de Cartouches</h3>
                <p>Ne jetez plus vos cartouches d'encre vides ! Je les rachète pour leur donner une seconde vie.</p>
                <div class="price-tag">Jusqu'à 1€ / cartouche</div>
                <p style="margin-top: 15px; font-size: 0.9rem; color: #666;">
                    *Selon modèle et marque (HP, Canon, Epson...). Contactez-moi pour une estimation rapide.
                </p>
            </div>

        </div>
    </section>

    <section class="contact-section">
        <h2>Besoin d'une intervention rapide ?</h2>
        <p>Disponible sur [VOTRE VILLE] et ses alentours.</p>
        
        <div class="contact-info">
            <div class="contact-item">
                <i class="fas fa-phone-square-alt"></i>
                <span>06 00 00 00 00</span>
                </div>
            <div class="contact-item">
                <i class="fas fa-envelope"></i>
                <span>votre-email@gmail.com</span>
                 </div>
        </div>
        <br>
        <a href="mailto:votre-email@gmail.com" class="btn btn-primary">Prendre rendez-vous</a>
    </section>

    <footer>
        <p>&copy; 2025 Nolhan Masson - Services Informatiques à Domicile.</p>
    </footer>

</body>
</html>
