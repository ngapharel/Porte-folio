<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - SIYEP NGANTCHOU Pharel</title>
    <style>
        :root {
            --primary: #9F7AEA;
            --secondary: #805AD5;
            --dark: #2D3748;
            --light: #F7FAFC;
            --accent: #F687B3;
            --text: #4A5568;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #FAF5FF;
            color: var(--text);
            line-height: 1.6;
        }
        
        .container {
            max-width: 900px;
            margin: 40px auto;
            padding: 40px;
            background-color: white;
            box-shadow: 0 10px 30px rgba(159, 122, 234, 0.1);
            border-radius: 15px;
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 10px;
            background: linear-gradient(90deg, var(--primary), var(--accent));
        }
        
        header {
            display: flex;
            align-items: center;
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .photo-container {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            overflow: hidden;
            border: 5px solid white;
            box-shadow: 0 10px 20px rgba(159, 122, 234, 0.2);
            flex-shrink: 0;
            position: relative;
        }
        
        .photo-container::after {
            content: "";
            position: absolute;
            inset: -5px;
            border-radius: 50%;
            padding: 5px;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
            -webkit-mask-composite: xor;
            mask-composite: exclude;
            pointer-events: none;
        }
        
        .photo {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .header-content {
            flex-grow: 1;
        }
        
        h1 {
            color: var(--primary);
            margin: 0;
            font-size: 2.5rem;
            font-weight: 700;
        }
        
        h2 {
            color: var(--secondary);
            font-size: 1.5rem;
            margin-top: 0;
            font-weight: 600;
        }
        
        h3 {
            color: var(--primary);
            font-size: 1.3rem;
            margin: 30px 0 15px;
            position: relative;
            display: inline-block;
        }
        
        h3::after {
            content: "";
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--accent);
            border-radius: 3px;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            background-color: var(--light);
            padding: 10px 15px;
            border-radius: 30px;
            font-size: 0.9rem;
        }
        
        .contact-item svg {
            color: var(--primary);
        }
        
        .about {
            background-color: var(--light);
            padding: 25px;
            border-radius: 10px;
            margin-bottom: 30px;
            position: relative;
        }
        
        .about::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 100%;
            background: linear-gradient(to bottom, var(--primary), var(--accent));
            border-radius: 4px 0 0 4px;
        }
        
        .availability {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 15px;
        }
        
        .availability-item {
            background-color: white;
            padding: 10px 15px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .availability-item svg {
            color: var(--accent);
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }
            
            .photo-container {
                margin: 0 auto;
            }
            
            .contact-info {
                justify-content: center;
            }
            
            .container {
                padding: 30px;
                margin: 20px;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <div class="container">
        <header>
            <!-- Remplacez "chemin/vers/photo-profil.jpg" par votre photo -->
            <div class="photo-container">
                <img src="profil.jpg" alt="Photo de Siyep Ngantchou Pharel" class="photo">
            </div>
            <div class="header-content">
                <h1>SIYEP NGANTCHOU Pharel</h1>
                <h2>Développeuse Web Passionnée</h2>
                
                <div class="contact-info">
                    <div class="contact-item">
                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path>
                            <circle cx="12" cy="10" r="3"></circle>
                        </svg>
                        Douala, Cameroun
                    </div>
                    <div class="contact-item">
                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path>
                        </svg>
                        +237 658 87 01 08
                    </div>
                    <div class="contact-item">
                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                            <polyline points="22,6 12,13 2,6"></polyline>
                        </svg>
                        <a href="mailto:manuelalorraine80@gmail.com">manuelalorraine80@gmail.com</a>
                    </div>
                </div>
            </div>
        </header>

        <section class="about">
            <h3>À Propos de Moi</h3>
            <p>
                Je suis une développeuse Web passionnée par l'informatique. Être toujours à la recherche 
                de techniques innovantes est mon centre d'intérêt principal. J'aime créer des solutions 
                web élégantes et fonctionnelles qui répondent aux besoins des utilisateurs.
            </p>
        </section>

        <section>
            <h3>Disponibilités</h3>
            <div class="availability">
                <div class="availability-item">
                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <circle cx="12" cy="12" r="10"></circle>
                        <polyline points="12 6 12 12 16 14"></polyline>
                    </svg>
                    Lundi à Vendredi: 08h - 17h
                </div>
                <div class="availability-item">
                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <circle cx="12" cy="12" r="10"></circle>
                        <polyline points="12 6 12 12 16 14"></polyline>
                    </svg>
                    Samedi & Dimanche: 10h - 15h
                </div>
            </div>
        </section>

        <section>
            <h3>Compétences Techniques</h3>
            <div style="display: flex; flex-wrap: wrap; gap: 10px; margin-top: 15px;">
                <span style="background-color: #EDF2F7; color: var(--primary); padding: 8px 15px; border-radius: 20px; font-weight: 500;">HTML/CSS</span>
                <span style="background-color: #EDF2F7; color: var(--primary); padding: 8px 15px; border-radius: 20px; font-weight: 500;">JavaScript</span>
                <span style="background-color: #EDF2F7; color: var(--primary); padding: 8px 15px; border-radius: 20px; font-weight: 500;">Développement Frontend</span>
                <span style="background-color: #EDF2F7; color: var(--primary); padding: 8px 15px; border-radius: 20px; font-weight: 500;">UI/UX Design</span>
                <span style="background-color: #EDF2F7; color: var(--primary); padding: 8px 15px; border-radius: 20px; font-weight: 500;">Résolution de problèmes</span>
            </div>
        </section>
    </div>
</body>
</html>
