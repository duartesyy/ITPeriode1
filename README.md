# Portfolio Website

Een persoonlijke portfolio-website gebouwd met HTML, CSS en JavaScript.

## Functies

- Responsief ontwerp voor mobiel en desktop
- Vloeiende navigatie met smooth scrolling
- Mobiel-vriendelijk hamburger menu
- Contact formulier
- Projectoverzicht met kaarten
- Scroll animaties

## Projectstructuur

```
portfolio/
├── index.html        # Hoofdpagina
├── css/
│   └── style.css     # Stijlen
├── js/
│   └── main.js       # Functionaliteit
└── README.md         # Deze bestandsbeschrijving
```

## Gebruik

1. Open `index.html` in een webbrowser
2. Of gebruik een lokale server:
   - Met Python: `python -m http.server 8000`
   - Met VS Code: Live Server extensie

## Hoe pas ik de website aan?

### 1. Je naam en logo aanpassen

Open `index.html` en zoek de nav sectie:
```html
<div class="logo">Mijn Naam</div>
```
Vervang `Mijn Naam` door je eigen naam.

---

### 2. Hero sectie (begintekst)

Zoek deze sectie in `index.html`:
```html
<section id="home" class="hero">
    <h1>Welkom bij mijn portfolio</h1>
    <p>Ik ben een webontwikkelaar</p>
```
Wijzig de tekst naar je eigen naam en beroep, bijvoorbeeld:
```html
<h1>Hallo, ik ben Jan de Vries</h1>
<p>Ik ben een frontend ontwikkelaar</p>
```

---

### 3. Over Mij sectie

Zoek de `about` sectie en pas de teksten aan:
```html
<div class="about-text">
    <p>Hier komt een korte beschrijving over jezelf.</p>
</div>
```
Vervang door iets als:
```html
<p>Ik ben een 16-jarige student die graag websites bouwt. 
   Ik zit op het vmbo en leer momenteel HTML, CSS en JavaScript.</p>
```

#### Vaardigheden toevoegen/wijzigen
```html
<div class="skills">
    <h3>Vaardigheden</h3>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
</div>
```
Voeg extra vaardigheden toe door een nieuw `<li>` element toe te voegen.

---

### 4. Projecten toevoegen

Zoek de `project-grid` in de HTML:
```html
<div class="project-grid">
    <div class="project-card">
        <h3>Project 1</h3>
        <p>Beschrijving van het project.</p>
        <a href="#">Bekijk project</a>
    </div>
```

#### Voorbeeld van een compleet project:
```html
<div class="project-card">
    <h3>Calculator App</h3>
    <p>Een simpele calculator gebouwd met HTML, CSS en JavaScript.</p>
    <a href="https://github.com/jouwnaam/calculator">Bekijk project</a>
</div>
```

#### Meerdere projecten toevoegen:
Kopieer het hele `<div class="project-card">...</div>` blok en plak het erbij.
Elk project krijgt zijn eigen kaart.

---

### 5. Afbeeldingen toevoegen

1. Maak een `images` map aan in de hoofdmap
2. Voeg je afbeeldingen toe (bijvoorbeeld screenshots van projecten)
3. Voeg een afbeelding toe aan een projectkaart:

```html
<div class="project-card">
    <img src="images/project1.png" alt="Screenshot calculator app" style="width:100%; border-radius:5px; margin-bottom:1rem;">
    <h3>Calculator App</h3>
    <p>Een simpele calculator.</p>
    <a href="#">Bekijk project</a>
</div>
```

---

### 6. Contactgegevens

Om je e-mail of social media toe te voegen, wijzig de footer:
```html
<footer>
    <p>&copy; 2026 Jan de Vries</p>
    <p>
        <a href="mailto:jan@example.com">E-mail</a> | 
        <a href="https://github.com/jandevries">GitHub</a>
    </p>
</footer>
```

---

### 7. Kleuren aanpassen

Open `css/style.css` en zoek de variabelen bovenaan:
```css
:root {
    --primary-color: #333;      /* Donker grijs - navigatie, footer */
    --secondary-color: #666;    /* Medium grijs */
    --accent-color: #007bff;    /* Blauw - knoppen, links */
    --bg-color: #fff;           /* Achtergrondkleur */
    --text-color: #333;         /* Tekstkleur */
}
```

Voorbeelden van kleurenschema's:
- **Blauw:** `--accent-color: #007bff;`
- **Groen:** `--accent-color: #28a745;`
- **Paars:** `--accent-color: #6f42c1;`
- **Oranje:** `--accent-color: #fd7e14;`

---

### Samenvatting-bestand

| Bestand | Wat pas je hier aan? |
|---------|---------------------|
| `index.html` | Teksten, projecten, afbeeldingen |
| `css/style.css` | Kleuren, lettertypes, layout |
| `js/main.js` | Animaties, functionaliteit (standaard is goed) |

### Tips
- Gebruik een code editor zoals VS Code
- Test regelmatig in de browser
- Maak eerst een back-up voordat je grote wijzigingen maakt
