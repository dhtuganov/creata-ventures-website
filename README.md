# Creata Ventures Website

Official website for **Creata Ventures** - an AIFC-registered Venture Studio focused on Creative Industries and DeepTech in Central Asia.

## Live Site

- **Production:** [www.creata.ventures](https://www.creata.ventures)
- **Netlify Preview:** Available after connecting to GitHub

## Features

- **Bilingual:** English (default) and Russian versions
- **Responsive:** Mobile-first design, works on all devices
- **Forms:** Netlify Forms integration for founder applications and contact
- **Modern Design:** Deep Blue + Gold color scheme, clean typography
- **Performance:** Static HTML/CSS/JS, optimized for fast loading

## Pages

| Page | EN | RU |
|------|----|----|
| Homepage | `/index.html` | `/ru/index.html` |
| About/Thesis | `/about.html` | `/ru/about.html` |
| Team | `/team.html` | `/ru/team.html` |
| Portfolio | `/portfolio.html` | `/ru/portfolio.html` |
| Apply | `/apply.html` | `/ru/apply.html` |
| Contact | `/contact.html` | `/ru/contact.html` |

## Team (8 Members)

### Core Team
- **David Tuganov** - Managing Director
- **Zarina Satubaldinam** - Portfolio Founder (NMT)
- **Saida Tleulenova** - Finance & Operations

### Advisory Board
- Sergey Makarov - Venture & Innovation Expert
- Kendrick White - Tech Commercialization Expert
- Ekaterina Runova - IP & Tech Transfer Specialist
- Abylay Akhymbekov - Technology Broker
- Evgeny "Brooks" Evdokimov - Venture Capital Expert

## Portfolio Companies

1. **iWendy** - MBTI-based founder matching platform (Active Development)
2. **NMT (NeuroMindTherapy)** - HealthTech platform with EEG monitoring (PMF)

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, Flexbox, Grid
- **JavaScript** - Vanilla JS, no dependencies
- **Fonts** - Montserrat (headings), Inter (body) via Google Fonts
- **Forms** - Netlify Forms with honeypot spam protection
- **Hosting** - Netlify

## Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/creata-ventures/website.git
   cd website
   ```

2. Serve locally (any static server):
   ```bash
   # Using Python
   python -m http.server 8000

   # Using Node.js
   npx serve .

   # Using PHP
   php -S localhost:8000
   ```

3. Open `http://localhost:8000` in your browser

## Deployment to Netlify

### Option 1: Git Integration (Recommended)

1. Push to GitHub repository
2. Connect repository to Netlify
3. Netlify auto-deploys on every push

### Option 2: Drag & Drop

1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the `Website` folder to the deploy area
3. Site is live in seconds

### Option 3: Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy
netlify deploy --prod
```

## Custom Domain Setup

1. In Netlify dashboard, go to **Domain settings**
2. Add custom domain: `creata.ventures`
3. Configure DNS at your registrar:
   - CNAME: `www` → `[your-site].netlify.app`
   - A record: `@` → Netlify IP addresses

## Forms Configuration

Forms are automatically processed by Netlify. Submissions appear in:
- Netlify Dashboard → Forms
- Optional: Email notifications in Netlify settings

### Form Names
- `founder-application` - English application form
- `founder-application-ru` - Russian application form
- `contact` - English contact form
- `contact-ru` - Russian contact form

## File Structure

```
Website/
├── index.html          # Homepage (EN)
├── about.html          # About/Thesis (EN)
├── team.html           # Team (EN)
├── portfolio.html      # Portfolio (EN)
├── apply.html          # Application form (EN)
├── contact.html        # Contact (EN)
├── css/
│   └── style.css       # All styles
├── js/
│   └── main.js         # All JavaScript
├── images/             # Image assets (add photos here)
├── ru/                 # Russian versions
│   ├── index.html
│   ├── about.html
│   ├── team.html
│   ├── portfolio.html
│   ├── apply.html
│   └── contact.html
├── netlify.toml        # Netlify configuration
└── README.md           # This file
```

## Customization

### Adding Team Photos

1. Add photos to `/images/` folder (recommended: 400x400px, JPEG/WebP)
2. Update team cards in `team.html` and `ru/team.html`:
   ```html
   <!-- Replace placeholder -->
   <div class="team-avatar">👤</div>

   <!-- With actual image -->
   <img src="images/david-tuganov.jpg" alt="David Tuganov" class="team-avatar">
   ```

### Social Media Links

Update social links in all page footers:
```html
<a href="https://linkedin.com/company/creata-ventures" target="_blank">in</a>
<a href="https://t.me/creataventures" target="_blank">tg</a>
```

### Google Maps

Replace map placeholder in `contact.html` and `ru/contact.html`:
```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%"
  height="400"
  style="border:0;"
  loading="lazy">
</iframe>
```

## Design System

### Colors
- Primary (Deep Blue): `#1a365d`
- Secondary (Medium Blue): `#2d4a7c`
- Accent (Gold): `#d69e2e`
- Light background: `#f7fafc`

### Typography
- Headings: Montserrat 600/700
- Body: Inter 400/500/600

### Breakpoints
- Desktop: > 1024px
- Tablet: 768px - 1024px
- Mobile: < 768px

## License

Copyright 2025 Creata Ventures Studio Ltd. All rights reserved.

---

**Built with care for Creata Ventures**
AIFC, Astana, Kazakhstan
