# LesLinq Micro Learning Website

Een professionele website voor het promoten van micro learning oplossingen voor SHEQ & KAM Managers.

## 🎯 Over dit project

Deze website is ontworpen om veiligheidskundigen (SHEQ & KAM Managers) kennis te laten maken met de voordelen van micro learning. De site heeft een zakelijke uitstraling en bevat:

- **Hero sectie** met duidelijke waardepropositie
- **Voordelen** specifiek voor de doelgroep
- **Testimonials** van echte gebruikers
- **Call-to-action** voor lead generatie
- **Volledig responsive** design voor alle apparaten

## 🚀 Deployment op Cloudflare Pages

### Methode 1: Via Git Integration (Aanbevolen)

1. **Push je code naar GitHub**
   ```bash
   git add .
   git commit -m "Initial commit: LesLinq micro learning website"
   git push origin main
   ```

2. **Login bij Cloudflare Dashboard**
   - Ga naar [dash.cloudflare.com](https://dash.cloudflare.com)
   - Klik op "Workers & Pages"

3. **Maak een nieuwe Pages deployment**
   - Klik op "Create application"
   - Selecteer "Pages"
   - Klik op "Connect to Git"

4. **Connect je repository**
   - Autoriseer Cloudflare met GitHub
   - Selecteer je repository
   - Klik op "Begin setup"

5. **Configureer de build settings**
   - **Project name**: `leslinq-micro-learning` (of een naam naar keuze)
   - **Production branch**: `main`
   - **Framework preset**: None
   - **Build command**: (laat leeg)
   - **Build output directory**: `/`

6. **Deploy**
   - Klik op "Save and Deploy"
   - Je website wordt automatisch gebouwd en gedeployed!

### Methode 2: Via Direct Upload

1. **Login bij Cloudflare Dashboard**
   - Ga naar [dash.cloudflare.com](https://dash.cloudflare.com)
   - Klik op "Workers & Pages"

2. **Upload direct**
   - Klik op "Create application"
   - Selecteer "Pages"
   - Klik op "Upload assets"
   - Selecteer alle bestanden (`index.html`, `styles.css`, `script.js`)
   - Klik op "Deploy site"

### Methode 3: Via Wrangler CLI

1. **Installeer Wrangler**
   ```bash
   npm install -g wrangler
   ```

2. **Login**
   ```bash
   wrangler login
   ```

3. **Deploy**
   ```bash
   wrangler pages publish . --project-name=leslinq-micro-learning
   ```

## 📁 Bestandsstructuur

```
micro_learning_website/
├── index.html          # Hoofdpagina
├── styles.css          # Styling en layout
├── script.js           # Interactiviteit en animaties
└── README.md           # Deze documentatie
```

## 🎨 Design Kenmerken

### Kleuren
- **Primary Blue**: #0066CC (vertrouwen en professionaliteit)
- **Primary Dark**: #003D7A (autoriteit)
- **Accent Orange**: #FF6B35 (energie en actie)
- **Grays**: Voor tekst en achtergronden

### Typografie
- **Font**: Inter (Google Fonts)
- Modern, professioneel en goed leesbaar

### Componenten
- ✅ Sticky navigation met smooth scroll
- ✅ Hero sectie met statistieken
- ✅ Voordelen cards met hover effecten
- ✅ Testimonials met authentieke quotes
- ✅ Volledig responsive voor mobile, tablet en desktop
- ✅ Smooth animaties en transitions

## 📱 Responsive Breakpoints

- **Desktop**: > 1024px
- **Tablet**: 768px - 1024px
- **Mobile**: < 768px

## ⚡ Performance Features

- Optimale laadtijd door minimale dependencies
- Lazy loading voor afbeeldingen
- Geoptimaliseerde CSS en JavaScript
- Goede Core Web Vitals scores

## 🔧 Aanpassingen maken

### Logo wijzigen
Het logo wordt geladen vanaf:
```
https://www.leslinq.com/wp-content/uploads/2024/05/LesLinq-logo-pay-off-EN-2024.png
```

Om een ander logo te gebruiken, vervang de URL in `index.html`.

### Kleuren aanpassen
Pas de CSS variabelen aan in `styles.css`:
```css
:root {
    --primary-blue: #0066CC;
    --accent-orange: #FF6B35;
    /* etc. */
}
```

### Content wijzigen
Bewerk de HTML in `index.html`. Alle secties zijn duidelijk gelabeld met comments.

### Testimonials aanpassen
Zoek naar de `.testimonials-grid` sectie in `index.html` en pas de quotes, namen en functies aan.

## 🌐 Custom Domain instellen

1. **In Cloudflare Pages Dashboard**
   - Ga naar je project
   - Klik op "Custom domains"
   - Klik op "Set up a custom domain"

2. **Voeg je domein toe**
   - Voer je domein in (bijv. `microlearning.leslinq.com`)
   - Volg de DNS instructies

3. **SSL Certificaat**
   - Cloudflare genereert automatisch een gratis SSL certificaat
   - Je site is bereikbaar via HTTPS

## 📊 Analytics toevoegen (optioneel)

### Google Analytics
Voeg dit toe voor de sluitende `</head>` tag in `index.html`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Cloudflare Web Analytics (Aanbevolen)
- Gratis, privacy-vriendelijk
- In Cloudflare Dashboard > Web Analytics
- Volg de instructies om de beacon toe te voegen

## 🔒 Security Headers

Cloudflare Pages voegt automatisch security headers toe:
- HTTPS enforcement
- HSTS
- X-Content-Type-Options
- X-Frame-Options

## 🐛 Troubleshooting

### Website laadt niet correct
- Check of alle bestanden zijn geüpload
- Controleer browser console voor errors
- Clear cache en probeer opnieuw

### Responsive design werkt niet
- Check viewport meta tag in `<head>`
- Test in verschillende browsers

### Animaties werken niet
- Controleer of `script.js` correct is geladen
- Check browser console voor JavaScript errors

## 📞 Support

Voor vragen over de website:
- Email: info@leslinq.com
- Website: https://www.leslinq.com

Voor Cloudflare Pages support:
- Docs: https://developers.cloudflare.com/pages/
- Community: https://community.cloudflare.com/

## 📝 Licentie

© 2024 LesLinq. Alle rechten voorbehouden.

---

**Gemaakt met** ❤️ **voor LesLinq**
