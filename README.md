Le fichier `index.html` est tout simplement **un document texte qui contient le code du site**. C'est le fichier principal que le navigateur (Chrome, Safari, Firefox) lit pour afficher votre page web.

Puisque vous n'en avez pas encore, **voici comment le créer en 2 minutes sur votre ordinateur** :

### 1. Copiez le code
Copiez l'intégralité du code ci-dessous (c'est la version bilingue optimisée pour vous) :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abdallah Allal | Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #007b8c; 
            --secondary-color: #444;
            --bg-light: #f4f7f6;
            --white: #ffffff;
            --border-color: #007b8c;
        }
        body {
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--secondary-color);
            background-color: var(--bg-light);
            margin: 0;
            padding: 0;
            transition: all 0.3s ease;
        }
        .lang-switch {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 1000;
            background: var(--primary-color);
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 20px;
            cursor: pointer;
            font-weight: bold;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
            transition: transform 0.2s;
        }
        .lang-switch:hover { transform: scale(1.05); }
        .container {
            max-width: 900px;
            margin: 40px auto;
            background: var(--white);
            padding: 40px;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
            border-radius: 8px;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            border-bottom: 3px solid var(--border-color);
            padding-bottom: 20px;
            margin-bottom: 20px;
        }
        .header-left h1 {
            margin: 0;
            font-size: 2.5rem;
            color: #000;
            text-transform: uppercase;
        }
        .header-left h2 {
            margin: 5px 0;
            font-size: 1.2rem;
            color: var(--primary-color);
            font-weight: 600;
        }
        .header-right {
            text-align: right;
            font-size: 0.9rem;
        }
        .contact-item {
            margin-bottom: 5px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
        }
        .contact-item i {
            margin-left: 10px;
            color: var(--primary-color);
            width: 20px;
        }
        section { margin-bottom: 30px; }
        h3 {
            color: var(--primary-color);
            text-transform: uppercase;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 5px;
            margin-bottom: 15px;
            font-size: 1.3rem;
        }
        .intro {
            font-style: italic;
            margin-bottom: 30px;
            text-align: justify;
            border-left: 4px solid var(--primary-color);
            padding-left: 15px;
        }
        .item { margin-bottom: 20px; }
        .item-title {
            font-weight: bold;
            display: flex;
            justify-content: space-between;
            color: #000;
        }
        .item-subtitle {
            color: var(--primary-color);
            font-weight: 500;
            font-size: 0.95rem;
        }
        .item-details {
            margin-left: 20px;
            font-size: 0.9rem;
        }
        .skills-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        .skills-table td {
            padding: 10px;
            border: 1px solid #ddd;
            vertical-align: top;
        }
        .skill-category {
            background-color: #eef9fa;
            color: var(--primary-color);
            font-weight: bold;
            width: 30%;
        }
        [lang="en"] { display: none; }
        @media (max-width: 600px) {
            header { flex-direction: column; text-align: center; }
            .header-right { text-align: center; margin-top: 20px; }
            .contact-item { justify-content: center; }
            .item-title { flex-direction: column; }
        }
    </style>
</head>
<body>

<button class="lang-switch" onclick="toggleLanguage()" id="langBtn">English 🇺🇸</button>

<div class="container">
    <header>
        <div class="header-left">
            <h1>ABDALLAH ALLAL</h1>
            <h2 lang="fr">Ingénieur en devenir – Électronique & Systèmes Embarqués</h2>
            <h2 lang="en">Future Engineer – Electronics & Embedded Systems</h2>
        </div>
        <div class="header-right">
            <div class="contact-item"><i class="fas fa-phone"></i> +33 7 43 30 97 86</div>
            <div class="contact-item"><i class="fas fa-envelope"></i> <a href="mailto:abdallahallal700@gmail.com" style="text-decoration:none; color:inherit;">abdallahallal700@gmail.com</a></div>
            <div class="contact-item"><i class="fas fa-map-marker-alt"></i> France</div>
            <div class="contact-item"><i class="fab fa-linkedin"></i> <a href="https://linkedin.com/in/abdallah-allal-3440b83a3" target="_blank" style="text-decoration:none; color:inherit;">linkedin.com/in/abdallah-allal</a></div>
            <div class="contact-item"><i class="fas fa-id-card"></i> Permis B | 06/12/2003</div>
        </div>
    </header>

    <div class="intro" lang="fr">
        Admis en cycle ingénieur à l'EPF (spécialisation Systèmes d'Information, option Génie Industriel, Campus de Cachan), titulaire d'un BTS Systèmes Électroniques et d'une Licence EEA, je recherche une alternance à partir de septembre 2026 en automatisme, électronique industrielle ou systèmes embarqués.
    </div>
    <div class="intro" lang="en">
        Admitted to the engineering program at EPF (Information Systems specialization, Industrial Engineering option, Cachan Campus), holding a BTS in Electronic Systems and a Bachelor's degree in EEA, I am seeking an apprenticeship starting September 2026 in automation, industrial electronics, or embedded systems.
