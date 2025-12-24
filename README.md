# SDK Solutions Website

Professionele website voor SDK Solutions - AI Adoptie Coach & Digitalisatie Expert voor KMO's in Vlaanderen.

## Over SDK Solutions

SDK Solutions werd opgericht in 2025 door Stijn De Ketelaere met als missie om Vlaamse KMO's te ondersteunen bij AI adoptie en digitalisatie projecten. Met ervaring opgedaan bij PwC, SymphonyAI en S&V Management Consultants wordt expertise toegankelijk gemaakt voor kleine en middelgrote ondernemingen.

## Website Structuur

```
sdk-solutions-website/
├── index.html          # Hoofdpagina met alle secties
├── blog.html           # Blog overzichtspagina
├── css/
│   ├── style.css       # Hoofdstijlen
│   └── blog.css        # Blog-specifieke stijlen
├── js/
│   └── main.js         # JavaScript functionaliteit
├── images/             # Afbeeldingen en logo's
├── netlify.toml        # Netlify deployment configuratie
└── package.json        # Project metadata
```

## Secties

- **Home** - Hero sectie met kernboodschap
- **Diensten** - AI Coaching, Digitalisatie, Automatisering, Web Development, Opleidingen, Analytics
- **Over Mij** - Achtergrond en ervaring
- **Projecten** - Vibe coding experimenten en side projects
- **Portfolio** - Websites in beheer (Joele, Krisma Bouw)
- **Blog** - Artikelen over AI en digitalisatie
- **Contact** - Contactformulier en gegevens

## Deployment naar Netlify

### Optie 1: Via GitHub

1. Maak een nieuwe repository aan op GitHub
2. Push deze code naar de repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - SDK Solutions website"
   git remote add origin https://github.com/JOUW-USERNAME/sdk-solutions-website.git
   git push -u origin main
   ```
3. Ga naar [Netlify](https://app.netlify.com)
4. Klik op "Add new site" > "Import an existing project"
5. Selecteer GitHub en kies je repository
6. Deploy settings worden automatisch ingesteld via `netlify.toml`
7. Klik op "Deploy site"

### Optie 2: Via Drag & Drop

1. Ga naar [Netlify](https://app.netlify.com)
2. Sleep de gehele projectmap naar de dropzone
3. Je site is direct live!

### Custom Domain

Na deployment:
1. Ga naar Site settings > Domain management
2. Klik "Add custom domain"
3. Voer `sdk-solutions.be` in
4. Volg de DNS configuratie instructies

## Lokaal Ontwikkelen

```bash
# Installeer een lokale server (optioneel)
npm install -g live-server

# Start de development server
npx live-server --port=3000
```

Of open simpelweg `index.html` in je browser.

## Aanpassingen

### Contact E-mail wijzigen

In `index.html`, zoek naar `info@sdk-solutions.be` en vervang door je echte e-mailadres.

### Logo toevoegen

1. Plaats je logo in de `images/` map als `logo.png`
2. De website gebruikt het logo automatisch in de navigatie en footer

### Contactformulier activeren

Het contactformulier simuleert momenteel een verzending. Om het werkend te maken:

**Optie 1: Netlify Forms**
Voeg `netlify` attribuut toe aan het form:
```html
<form class="contact-form" id="contact-form" netlify>
```

**Optie 2: Formspree**
1. Maak een account op [Formspree](https://formspree.io)
2. Wijzig de form action naar je Formspree endpoint

### Analytics toevoegen

Voeg Google Analytics of Plausible toe in de `<head>` sectie van `index.html`.

## SEO Features

- Semantic HTML5 structuur
- Schema.org structured data (LocalBusiness, ProfessionalService, Blog)
- Open Graph meta tags voor social media
- Geographic meta tags voor lokale vindbaarheid
- Canonical URLs
- Mobile-responsive design
- Geoptimaliseerde laadtijden

## Technologieën

- HTML5
- CSS3 (Custom Properties, Flexbox, Grid)
- Vanilla JavaScript (ES6+)
- Font Awesome icons
- Google Fonts (Inter, JetBrains Mono)

## Browser Support

- Chrome (laatste 2 versies)
- Firefox (laatste 2 versies)
- Safari (laatste 2 versies)
- Edge (laatste 2 versies)

## Licentie

© 2025 SDK Solutions. Alle rechten voorbehouden.

---

Gebouwd met ❤️ voor Vlaamse KMO's
