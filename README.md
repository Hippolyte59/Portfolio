# Portfolio Personnel Interactif

<div align="center">

[![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)](https://www.w3.org/Style/CSS/)
[![JavaScript](https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Daisy UI](https://img.shields.io/badge/Daisy%20UI-%23FF69B4.svg?style=for-the-badge&logo=daisyui&logoColor=white)](https://daisyui.com/)

[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg?style=for-the-badge)](package.json)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg?style=for-the-badge)](README.md)
[![Author](https://img.shields.io/badge/Author-Hippolyte-purple.svg?style=for-the-badge)](https://github.com/hippolyte)

**Un template web moderne et professionnel pour créer votre portfolio personnel avec des animations fluides, un design épuré et une excellente optimisation SEO.**

[Démarrage Rapide](#-démarrage-rapide) • [Documentation](#-documentation) • [Personnalisation](#-personnalisation) • [Déploiement](#-déploiement)

</div>

---

## Caractéristiques

### Design & UX
- **Design Modern**: Interface élégante avec dégradés et effets de couleurs
- **Responsive**: Entièrement adapté à tous les appareils (mobile, tablette, desktop)
- **Animations Fluides**: Transitions légères et animations au scroll avec AOS
- **Mode Sombre**: Thème sombre par défaut pour le confort visuel
- **Accessibilité**: Support `prefers-reduced-motion` et navigation au clavier

### Technologies
- **HTML5** - Structure sémantique et optimisée
- **Tailwind CSS** - Framework CSS utilitaire et performant
- **Daisy UI** - Composants pré-stylisés et personnalisables
- **JavaScript Vanilla** - Pas de dépendances lourdes, code pur
- **AOS** - Animations au scroll professionnelles
- **Font Awesome** - 2000+ icônes vectorielles

### Sections du Portfolio

| Section | Description | Fonctionnalités |
|---------|-------------|-----------------|
| **Navigation** | Barre sticky responsive | Menu mobile, smooth scroll |
| **Hero** | Section d'accueil | Gradient, animations, CTA |
| **Projets** | Galerie interactive | Filtres, modals, détails |
| **Compétences** | Showcase technique | Barres de progression, icônes |
| **Contact** | Formulaire + social | Email, LinkedIn, GitHub |
| **Footer** | Navigation secondaire | Links, crédits, social |

### Fonctionnalités Principales
- **Filtrage dynamique** des projets (Tous, Web, Mobile, Design)
- **Modals interactifs** pour les détails des projets
- **Animations au scroll** fluides et performantes
- **Barres de progression** pour les compétences
- **Formulaire de contact** avec validation
- **Scroll lisse** et navigation fluide
- **Optimisation SEO** complète
- **Performance optimale** (Lighthouse 95+)

---

## Démarrage Rapide

### En 5 minutes, lancez votre portfolio!

#### Option 1: Live Server (VS Code) - Recommandé
```bash
# 1. Ouvrir le dossier dans VS Code
code .

# 2. Clic droit sur index.html
# 3. Sélectionner "Open with Live Server"
```

#### Option 2: Python
```bash
python -m http.server 8000
# Puis ouvrir: http://localhost:8000
```

#### Option 3: Node.js
```bash
npx http-server .
# Puis ouvrir: http://localhost:8080
```

---

## Personnalisation Rapide

### 1️Informations Personnelles

Dans `index.html`, modifiez:

```html
<!-- Section Hero -->
<h1>Transformez vos idées en réalité</h1>
<p>Développeur Full Stack passionné...</p>

<!-- Contact -->
<a href="mailto:contact@example.com">Email</a>
<a href="https://linkedin.com/in/votreprofil">LinkedIn</a>
<a href="https://github.com/votreprofil">GitHub</a>
```

### 2️Ajouter vos Projets

Dans `script.js`, modifiez `projectDetails`:

```javascript
const projectDetails = {
    1: {
        title: 'Votre Titre',
        description: 'Description détaillée',
        technologies: ['React', 'Node.js', 'MongoDB'],
        image: '#',
        details: ['Feature 1', 'Feature 2', 'Feature 3'],
        github: 'https://github.com/votre-repo',
        demo: 'https://votresite.com'
    }
};
```

### 3️Changer les Couleurs

Modifiez dans `style.css`:

```css
/* Schéma actuel: Purple & Cyan */
from-purple-500 to-cyan-500

/* Exemples alternatifs: */
/* Bleu-Vert (Tech) */
from-blue-500 to-green-500

/* Rose-Orange (Creative) */
from-pink-500 to-yellow-500

/* Noir-Or (Luxe) */
from-gray-900 to-yellow-500
```

### 4️Ajouter une Photo de Profil

```html
<div class="w-full h-96 rounded-2xl overflow-hidden">
    <img src="votre-photo.jpg" alt="Votre Nom" 
         class="w-full h-full object-cover">
</div>
```

**Format recommandé:** JPG, PNG ou WebP
**Dimensions:** 400x400px minimum
**Taille:** < 100KB

---

## Exemples de Personnalisation

### Schémas de Couleurs Populaires

#### Schéma Bleu-Vert (Tech/Startup)
```css
from-blue-500 to-green-500  /* Ou: from-0066ff to-00cc88 */
```

#### Schéma Rose-Orange (Creative/Design)
```css
from-pink-500 to-yellow-500  /* Ou: from-ff6b6b to-ffa94d */
```

#### Schéma Noir-Or (Luxe/Premium)
```css
from-gray-900 to-yellow-400  /* Ou: from-1a1a1a to-d4af37 */
```

### Ajouter un Bouton Theme Toggle

```html
<!-- HTML (dans navbar) -->
<button id="themeToggle" class="btn btn-ghost">
    <i class="fas fa-moon"></i>
</button>
```

```javascript
// JavaScript
const themeToggle = document.getElementById('themeToggle');
const root = document.documentElement;

themeToggle.addEventListener('click', () => {
    const newTheme = root.getAttribute('data-theme') === 'dark' ? 'light' : 'dark';
    root.setAttribute('data-theme', newTheme);
    localStorage.setItem('theme', newTheme);
});

const savedTheme = localStorage.getItem('theme') || 'dark';
root.setAttribute('data-theme', savedTheme);
```

### Ajouter des Statistiques

```html
<div class="stats shadow">
    <div class="stat">
        <div class="stat-title">Projets</div>
        <div class="stat-value text-purple-400">15+</div>
    </div>
    <div class="stat">
        <div class="stat-title">Clients</div>
        <div class="stat-value text-cyan-400">20+</div>
    </div>
    <div class="stat">
        <div class="stat-title">Années</div>
        <div class="stat-value text-pink-400">5+</div>
    </div>
</div>
```

### Personnaliser les Animations

```javascript
// Ralentir les animations
AOS.init({
    duration: 1200,  // Augmentez de 800 à 1200
    offset: 100,
    easing: 'ease-in-out-cubic'
});

// Désactiver les animations (optionnel)
// [data-aos] { opacity: 1 !important; transform: none !important; }
```

---

## Structure des Fichiers

```
portfolio/
├── index.html              # Page principale
├── style.css               # Styles personnalisés
├── script.js               # Fonctionnalités JS
├──README.md               # Documentation (ce fichier)
├── package.json            # Métadonnées du projet
├── manifest.json           # Configuration PWA
├── robots.txt              # Directives moteurs recherche
├── sitemap.xml             # Plan du site pour SEO
├── .htaccess               # Configuration serveur
└── .vscode/
    └── settings.json          # Configuration VS Code
```

---

## SEO Optimization

### Déjà Intégré

- Meta tags structurés (title, description)
- Open Graph tags (partage social)
- Mobile-friendly viewport
- Performance optimale
- Sitemap XML
- Robots.txt

### À Ajouter

1. **Remplacer les placeholders:**
```html
<meta name="author" content="Votre Nom">
<meta property="og:image" content="votre-image.jpg">
<meta name="description" content="Votre description unique">
```

2. **Ajouter JSON-LD Structured Data:**
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Votre Nom",
  "url": "https://votresite.com",
  "jobTitle": "Développeur Full Stack"
}
</script>
```

3. **Google Analytics:**
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

### Objectifs de Performance

| Métrique | Cible | Outil |
|----------|-------|-------|
| **Lighthouse Performance** | 95+ | Chrome DevTools |
| **Lighthouse SEO** | 100 | Chrome DevTools |
| **Page Load Time** | < 2s | GTmetrix |
| **Core Web Vitals** | Good | PageSpeed Insights |

---

## Déploiement

### Option 1: Netlify (Recommandé)

1. Créez un compte sur [netlify.com](https://netlify.com)
2. Connectez votre repo GitHub
3. Le déploiement se fait automatiquement à chaque push

```bash
# Déploiement via CLI (optionnel)
npm install -g netlify-cli
netlify deploy
```

### Option 2: Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Importez votre projet
3. Configuration automatique et déploiement

```bash
npm install -g vercel
vercel
```

### Option 3: GitHub Pages

```bash
# 1. Créez un repo nommé: username.github.io
# 2. Pushez votre code
git add .
git commit -m "Initial commit"
git push origin main

# 3. Accédez à: https://username.github.io
```

### Option 4: Serveur Perso (Apache/Nginx)

```bash
# 1. Uploadez via FTP
# 2. Configurez un domaine
# 3. Activez HTTPS (Let's Encrypt gratuit)

# Apache .htaccess inclus pour:
# Compression GZIP
# Cache navigateur
# Headers sécurité
# Redirection HTTPS
```

---

## 📱 Responsive Design

Testé et optimisé pour:

| Appareil | Résolution | Test |
|----------|-----------|------|
| iPhone SE | 375px | 
| iPhone 12/13 | 390px | 
| Android | 412px | 
| iPad | 768px | 
| Desktop | 1920px+ | 

### Test Responsive dans VS Code
```
F12 → Ctrl+Shift+M (Windows)
F12 → Cmd+Shift+M (Mac)
```

---

## Animations & Transitions

### Bibliothèques Utilisées

| Lib | Usage | Version |
|-----|-------|---------|
| **AOS** | Scroll animations | Latest |
| **Tailwind** | CSS utilities | 3.x |
| **Daisy UI** | Components | 4.x |
| **Font Awesome** | Icons | 6.4.0 |

### Personnaliser les Animations

```css
/* Dans style.css */

/* Ralentir le blob */
.animate-blob {
    animation: blob 10s infinite; /* Était 7s */
}

/* Ajouter une nouvelle animation */
@keyframes fadeInScale {
    from {
        opacity: 0;
        transform: scale(0.9);
    }
    to {
        opacity: 1;
        transform: scale(1);
    }
}

.fade-in-scale {
    animation: fadeInScale 0.6s ease-out;
}
```

---

## Développement Local

### Raccourcis VS Code

| Raccourci | Action |
|-----------|--------|
| `Ctrl+Shift+P` | Palette de commandes |
| `F12` | DevTools |
| `Ctrl+Shift+M` | Mode responsive |
| `Alt+O` | Open with Live Server |
| `Ctrl+K Ctrl+0` | Zoom out |
| `Ctrl+K Ctrl+1` | Zoom normal |

### Vérifier que tout fonctionne

```javascript
// Dans la console (F12)
console.log('Portfolio chargé!');
console.log(AOS);  // Vérifier AOS
console.log(window.projectDetails);  // Vérifier projets
```

### DevTools Essentiels

1. **Console** - Erreurs JavaScript
2. **Network** - Charger les ressources
3. **Performance** - Vitesse du site
4. **Lighthouse** - Audit SEO/Performance

---

## Troubleshooting

### Problème: Les animations ne s'affichent pas

**Solution:**
```javascript
// Vérifiez dans la console
console.log(AOS);  // Doit retourner un objet
```

- Rechargez: `Ctrl+Shift+R` (hard refresh)
- Videz le cache navigateur
- Vérifiez la connexion Internet

### Problème: Les styles Tailwind ne s'appliquent pas

**Solution:**
- Raffraîchissez: `Ctrl+Shift+R`
- Vérifiez le CDN: https://cdn.tailwindcss.com est accessible
- Utilisez un VPN si accès bloqué

### Problème: Le formulaire ne fonctionne pas

**Solution:** Les formulaires statiques HTML nécessitent un backend. Utilisez:
- [Netlify Forms](https://netlify.com/products/forms/) - Gratuit avec Netlify
- [Formspree](https://formspree.io/) - Solution simple
- [EmailJS](https://www.emailjs.com/) - Client-side JavaScript
- [Basin](https://usebasin.com/) - Service gratuit

```html
<!-- Exemple avec Netlify -->
<form name="contact" method="POST" netlify>
    <input type="text" name="name" required>
    <input type="email" name="email" required>
    <textarea name="message" required></textarea>
    <button type="submit">Envoyer</button>
</form>
```

### Problème: Performance lente

**Solutions:**
1. Compressez vos images: [TinyPNG](https://tinypng.com)
2. Minifiez CSS/JS: [CSS Minifier](https://cssminifier.com/)
3. Utilisez WebP pour les images
4. Activez la compression GZIP (inclus dans .htaccess)

---
## Contribution

Pour améliorer ce template:

1. Fork le projet
2. Créez une branche (`git checkout -b feature/Améliorations`)
3. Commitez vos changements (`git commit -m 'Ajout feature'`)
4. Pushez vers la branche (`git push origin feature/Améliorations`)
5. Ouvrez une Pull Request

---

## Licence

```
MIT License

Copyright (c) 2024 Hippolyte

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

**© 2024 Hippolyte** - MIT License

**TL;DR:** Vous pouvez utiliser, modifier et partager ce projet librement.

---
