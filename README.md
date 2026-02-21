# 📱 Productivité Atelier - PWA

Application de gestion de productivité pour atelier automobile.

## 🚀 Installation sur téléphone (Android/iOS)

### Option 1 : Installation directe (PWA)

#### Sur Android (Chrome/Edge) :
1. Ouvrez `productivite-orange.html` dans Chrome
2. Appuyez sur les **3 points** en haut à droite
3. Sélectionnez **"Ajouter à l'écran d'accueil"** ou **"Installer l'application"**
4. L'icône ⚡ apparaîtra sur votre écran d'accueil
5. L'app fonctionne maintenant hors ligne !

#### Sur iOS (Safari) :
1. Ouvrez `productivite-orange.html` dans Safari
2. Appuyez sur le bouton **Partager** (carré avec flèche)
3. Faites défiler et sélectionnez **"Sur l'écran d'accueil"**
4. Appuyez sur **"Ajouter"**
5. L'app est maintenant accessible depuis votre écran d'accueil !

---

### Option 2 : Créer une vraie APK Android

Pour créer un fichier .apk installable :

#### Méthode A - En ligne (gratuit, facile) :
1. Allez sur **https://www.pwabuilder.com/**
2. Cliquez sur **"Start"**
3. Hébergez vos 3 fichiers quelque part (GitHub Pages, Netlify, etc.)
4. Entrez l'URL de votre site
5. Cliquez sur **"Package for Stores"**
6. Sélectionnez **"Android"**
7. Téléchargez le fichier .apk généré
8. Transférez-le sur votre téléphone et installez-le

#### Méthode B - Hébergement gratuit rapide :
1. Allez sur **https://app.netlify.com/drop**
2. Glissez-déposez les 3 fichiers :
   - `productivite-orange.html`
   - `manifest.json`
   - `sw.js`
3. Vous obtenez une URL (ex: https://random-name.netlify.app)
4. Ouvrez cette URL sur votre téléphone
5. Installez l'app avec les instructions de l'Option 1

---

## 📦 Fichiers nécessaires

Pour que la PWA fonctionne, vous avez besoin de ces 3 fichiers dans le même dossier :

1. **productivite-orange.html** - L'application principale
2. **manifest.json** - Configuration de la PWA (nom, icône, couleurs)
3. **sw.js** - Service Worker (permet le mode hors ligne)

---

## ✨ Fonctionnalités

✅ **Fonctionne hors ligne** - Pas besoin d'internet après installation
✅ **Stockage local** - Toutes les données sont sauvegardées dans le navigateur
✅ **Installation facile** - Comme une vraie app native
✅ **Design orange industriel** - Interface moderne et professionnelle
✅ **Timers en temps réel** - Pour chaque véhicule
✅ **Bilan global** - Temps gagné/perdu sur tous les véhicules
✅ **Export PNG** - Générer un rapport de fin de journée

---

## 🔧 Système de temps

**Saisie** : Centièmes d'heure (0.50 = 30 min, 1.90 = 1h 54min)
**Affichage différence** : Heures + minutes (+1h 30min, -45min)
**Timers** : Format HH:MM:SS

---

## 📊 Compteurs

- **Inactivité** : Temps de pause (enlève du temps gagné)
- **Pression** : Temps urgent (juste pour suivi, n'impacte pas le bilan)

---

## 💾 Sauvegarde

- Les données restent **indéfiniment** jusqu'à ce que vous appuyiez sur 🗑️
- **Pas de reset automatique** - Parfait pour les rapports hebdomadaires !
- Les véhicules et compteurs s'accumulent toute la semaine
- Le vendredi, générez votre rapport PNG (bouton 📄)
- Puis videz tout pour recommencer la semaine suivante (bouton 🗑️)
- ⚠️ Pensez à exporter avant de vider !

**Exemple d'utilisation hebdomadaire :**
- Lundi → Jeudi : Accumulez les données
- Vendredi : Exportez le rapport PNG
- Vendredi soir : Videz pour recommencer lundi

---

## 🎨 Design

Police : **Orbitron** (titres) + **Barlow** (corps)
Couleur principale : **#ff6b35** (orange industriel)
Fond : **#0f1419** (noir profond)

---

## 🆘 Support

Si l'installation ne fonctionne pas :
- Vérifiez que les 3 fichiers sont au même endroit
- Utilisez Chrome sur Android ou Safari sur iOS
- Videz le cache du navigateur et réessayez

Bon travail à l'atelier ! 🚗⚡
