# ⚡ Productivité Atelier - PWA

Application de gestion de productivité pour atelier automobile.

---

## 🚀 Installation sur téléphone (Android/iOS)

### Option 1 : Installation directe (PWA)

#### Sur Android (Chrome/Edge) :
1. Hébergez l'app (voir Option 2) ou ouvrez le fichier HTML localement
2. Appuyez sur les 3 points en haut à droite
3. Sélectionnez **"Ajouter à l'écran d'accueil"** ou **"Installer l'application"**
4. L'icône ⚡ apparaîtra sur votre écran d'accueil
5. L'app fonctionne maintenant hors ligne !

#### Sur iOS (Safari) :
1. Ouvrez l'URL dans Safari
2. Appuyez sur le bouton **Partager** (carré avec flèche)
3. Faites défiler et sélectionnez **"Sur l'écran d'accueil"**
4. Appuyez sur **"Ajouter"**
5. L'app est maintenant accessible depuis votre écran d'accueil !

---

### Option 2 : Hébergement & APK Android

#### Méthode A — Hébergement gratuit rapide (Netlify Drop) :
1. Allez sur [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. Glissez-déposez les 3 fichiers :
   - `productivite-orange.html`
   - `manifest.json`
   - `sw.js`
3. Obtenez une URL (ex: `https://random-name.netlify.app`)
4. Ouvrez cette URL sur votre téléphone et installez l'app (Option 1)

#### Méthode B — Créer une vraie APK Android (PWABuilder) :
1. Allez sur [https://www.pwabuilder.com/](https://www.pwabuilder.com/)
2. Hébergez d'abord vos fichiers (Netlify, GitHub Pages…)
3. Entrez l'URL de votre site
4. Cliquez sur **"Package for Stores"** → **"Android"**
5. Téléchargez le `.apk`, transférez-le sur votre téléphone et installez-le

---

## 📦 Fichiers nécessaires

Les 3 fichiers doivent être dans le même dossier :

| Fichier | Rôle |
|---|---|
| `productivite-orange.html` | Application principale |
| `manifest.json` | Configuration PWA (nom, icône, couleurs) |
| `sw.js` | Service Worker (mode hors ligne) |

---

## ✨ Fonctionnalités

- ✅ **Fonctionne hors ligne** — Pas besoin d'internet après installation
- ✅ **Stockage local** — Toutes les données sauvegardées dans le navigateur
- ✅ **Thème clair / sombre** — Bascule en un tap depuis le header (☀️ / 🌙)
- ✅ **Installation facile** — Comme une vraie app native
- ✅ **Timers en temps réel** — Pour chaque véhicule (▶ / ⏸ / ⏹)
- ✅ **Terminer un véhicule** — Confirmation avant arrêt définitif du timer
- ✅ **Bilan global** — Temps gagné/perdu sur tous les véhicules (déduit l'inactivité)
- ✅ **Bannière d'alerte** — Rappel visuel si inactivité ou pression est en cours
- ✅ **Export PNG** — Rapport de bilan avec tableau des véhicules
- ✅ **Multi-lignes de temps** — Jusqu'à 15 lignes de temps prévu par véhicule
- ✅ **Modification du temps réel** — Ajouter ou retirer du temps (correction d'oubli de pause)
- ✅ **Blocage des actions simultanées** — Impossible de lancer deux tâches en même temps

---

## 🔧 Système de temps

- **Saisie** : Centièmes d'heure (`0.50` = 30 min, `1.90` = 1h 54min)
- **Multi-lignes** : Plusieurs opérations sur un même véhicule (total automatique)
- **Affichage différence** : Heures + minutes (`+1h 30min`, `-45min`)
- **Timers** : Format `HH:MM:SS`

---

## 📊 Compteurs globaux

| Compteur | Icône | Impact sur le bilan |
|---|---|---|
| **Inactivité** | ⏸️ | ✅ Déduit du bilan (temps de pause) |
| **Pression/Niveau** | ⚡ | ❌ Suivi uniquement, n'impacte pas le bilan |

> ⚠️ Une seule tâche à la fois — timer véhicule, inactivité ou pression.

---

## 🎨 Design

- **Police** : Outfit (corps) + Space Mono (chiffres/titres)
- **Thème clair** : Fond `#f4f5f7`, accent `#e8590c` (orange industriel)
- **Thème sombre** : Fond `#111318`, accent `#ff6b35` (orange vif)
- **Bascule thème** : Toggle dans le header, préférence sauvegardée

---

## 💾 Sauvegarde

- Les données restent indéfiniment jusqu'au bouton 🗑️
- **Pas de reset automatique** — Parfait pour les rapports hebdomadaires !
- Les véhicules et compteurs s'accumulent toute la semaine

### Exemple d'utilisation hebdomadaire :
| Jour | Action |
|---|---|
| Lundi → Jeudi | Accumulez les données |
| Vendredi | Exportez le rapport PNG (bouton 📄) |
| Vendredi soir | Videz tout pour recommencer lundi (bouton 🗑️) |

> ⚠️ **Pensez à exporter avant de vider !**

---

## 🆘 Support

Si l'installation ne fonctionne pas :
- Vérifiez que les 3 fichiers sont au même endroit
- Utilisez **Chrome** sur Android ou **Safari** sur iOS
- Videz le cache du navigateur et réessayez
- L'app doit être servie via **HTTPS** pour que le Service Worker fonctionne (Netlify, GitHub Pages, etc.)

Bon travail à l'atelier ! 🚗⚡

