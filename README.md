# 🥋 Judo Club des Avirons - Site Web

Bienvenue ! Ce dossier contient le site web complet du Judo Club des Avirons.

## 📁 Structure du Projet

```
judo-club-website/
├── index.html              ← Page d'accueil (COMMENCEZ ICI)
├── club.html               ← Présentation du club
├── equipe.html             ← Profils des entraîneurs
├── horaires.html           ← Horaires et inscriptions
├── tarifs.html             ← Tarifs 2025/2026
├── histoire.html           ← Histoire du judo
├── actualites.html         ← Blog et news
├── contact.html            ← Contact et formulaire
├── css/
│   └── style.css           ← Feuille de style commune
├── images/                 ← Dossier pour vos photos
└── README.md               ← Ce fichier
```

## 🚀 Comment Utiliser

### Localement (sur votre ordinateur)

1. **Téléchargez tous les fichiers** dans un dossier
2. **Ouvrez `index.html`** avec votre navigateur préféré (double-clic)
3. Vous pouvez naviguer dans le site normalement

### En Ligne (hébergement web)

Pour mettre votre site en ligne, vous devez :

1. **Choisir un hébergeur** (OVH, 1&1, Hostinger, DreamHost, etc.)
2. **Enregistrer un nom de domaine** (ex: www.judoclubavirons.com)
3. **Uploader les fichiers** via FTP ou l'interface de gestion de votre hébergeur
4. **Configurer l'index** pour que `index.html` soit la page par défaut

## 🎨 Intégrer Vos Images

Les images sont actuellement des **placeholders** (zones vides avec texte). Voici comment les remplacer :

### Créer un dossier `images`

```
judo-club-website/
├── images/
│   ├── dojo.jpg
│   ├── entrainees.jpg
│   ├── bruno-pion.jpg
│   ├── logo.png
│   └── ... autres images
```

### Remplacer les placeholders

Cherchez dans le HTML les lignes comme :

```html
<div class="image-placeholder image-large">
    [Image : Dojo principal]
</div>
```

Et remplacez-les par :

```html
<img src="images/dojo.jpg" alt="Dojo principal" style="width: 100%; height: 400px; border-radius: 8px; object-fit: cover;">
```

**Propriétés essentielles pour l'image :**
- `width: 100%;` - largeur totale
- `height: XXXpx;` - hauteur (adapté selon le placeholder)
- `object-fit: cover;` - remplit l'espace sans déformation
- `border-radius: 8px;` - coins arrondis

### Images à ajouter prioritairement

1. **Logo du club** (en haut à gauche de chaque page)
2. **Photos du dojo** (principal et secondaire)
3. **Photos des entraîneurs** (sur la page équipe.html)
4. **Photos d'événements** (sur actualites.html)
5. **Galerio de groupe** (entraînements, compétitions)

## ✏️ Modifier le Contenu

### Changer le texte

Ouvrez n'importe quel fichier `.html` avec un éditeur texte (Notepad++, VS Code, Sublime Text) et modifiez directement le texte. Les balises HTML ne changent pas.

### Ajouter une nouvelle article de blog

1. Ouvrez `actualites.html`
2. Trouvez l'article le plus récent
3. Copiez-le et collez-le au-dessus
4. Modifiez la date, le titre et le contenu

### Changer les coordonnées de contact

Cherchez cette section dans chaque page et mettez à jour :

```html
<p>📧 judoclub.avirons@hotmail.fr</p>
<p>📍 Les Avirons, La Réunion</p>
```

### Modifier les horaires des cours

Ouvrez `horaires.html` et mettez à jour le tableau :

```html
<table class="schedule-table">
    <thead>
        <tr>
            <th>Jour</th>
            <th>Horaire</th>
            <th>Groupe</th>
            <th>Entraîneur</th>
        </tr>
    </thead>
    <tbody>
        <!-- Modifiez les lignes ici -->
    </tbody>
</table>
```

### Modifier les tarifs

Ouvrez `tarifs.html` et cherchez les sections `.price-box`. Modifiez les prix et descriptions.

## 🔧 Personnalisation Avancée

### Couleurs

Les couleurs principales sont définies en haut de `css/style.css` :

```css
:root {
    --primary-blue: #185FA5;        /* Bleu principal */
    --dark-blue: #042C53;           /* Bleu foncé */
    --light-blue: #E6F1FB;          /* Bleu clair */
    --accent-gold: #BA7517;         /* Or/accent */
}
```

Vous pouvez les changer pour personnaliser l'apparence globale.

### Fonts

Les polices utilisées sont :
- `Segoe UI` (police système moderne)
- Arial et Verdana en secours

Pour changer, modifiez dans `css/style.css` :

```css
body {
    font-family: 'Votre Police', sans-serif;
}
```

### Spacing & Dimensions

Modifiez dans `css/style.css` :

```css
.container {
    max-width: 1200px;  /* Largeur max du site */
}

section {
    padding: 4rem 0;    /* Hauteur des sections */
}
```

## 📱 Tester la Version Mobile

1. Ouvrez le site dans votre navigateur
2. Appuyez sur `F12` (ou clic droit → Inspecter)
3. Cliquez l'icône mobile en haut à gauche
4. Le site s'affiche comme sur téléphone

Le site est entièrement **responsive** - il s'adapte automatiquement à tous les appareils !

## 🌐 Hébergement Web

### Option 1 : OVH (Français)
- Site: ovh.com
- Tarif: ~3-5€/mois
- Facile d'utilisation

### Option 2 : 1&1 IONOS
- Site: ionos.fr
- Tarif: ~2-4€/mois
- Très populaire

### Option 3 : Hostinger
- Site: hostinger.fr
- Tarif: ~2-3€/mois
- Bon rapport qualité/prix

### Option 4 : GitHub Pages (Gratuit !)
- Site: github.com
- Gratuit !
- Un peu plus technique

## 📧 Formulaire de Contact

Le formulaire sur `contact.html` est actuellement **de démonstration**. Pour qu'il fonctionne vraiment, vous devez :

1. Utiliser un service comme **Formspree** (formspree.io) - gratuit
2. Ou configurer un **backend PHP/Node.js** chez votre hébergeur
3. Ou intégrer **Google Forms** embedded

## 🔍 SEO (Référencement)

Pour améliorer le positionnement Google :

1. Modifiez les balises `<title>` et `<meta>` dans chaque page
2. Ajoutez des descriptions pertinentes
3. Utilisez Google Search Console
4. Créez un sitemap XML

## ⚠️ Points Importants

- **Backup** : Sauvegardez régulièrement vos fichiers
- **Certificat SSL** : Essentiellement pour HTTPS (sécurité)
- **Mises à jour** : Gardez votre contenu à jour
- **Analytics** : Installez Google Analytics pour suivre les visites

## 🆘 Besoin d'Aide ?

### Erreurs courantes

**"Certaines images ne s'affichent pas"**
- Vérifiez le chemin du dossier `images/`
- Les fichiers HTML doivent être dans le dossier racine

**"Les styles ne s'appliquent pas"**
- Vérifiez que `css/style.css` existe
- Rafraîchissez la page (Ctrl+F5)

**"Le lien vers une autre page ne fonctionne pas"**
- Les fichiers `.html` doivent être dans le même dossier
- Les liens relatifs doivent être corrects

## 📞 Support Technique

Pour les questions sur l'hébergement ou les domaines, contactez directement votre hébergeur. Ils ont généralement un support 24/7.

## 🎓 Ressources Utiles

- [W3Schools HTML](https://www.w3schools.com/html/)
- [W3Schools CSS](https://www.w3schools.com/css/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [Google Search Central](https://developers.google.com/search)

---

**Bonne chance avec votre nouveau site ! 🥋**

Créé avec ❤️ pour la communauté judo réunionnaise
2025
# judo-club-des-avirons
