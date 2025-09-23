# PrayerApp-Autonomous
# PrayerApp-Autonomous

Une application web autonome pour trouver et réciter 111 prières inspirées de la Bible (canonique et apocryphe), organisées par afflictions et demandes à Dieu. Les prières sont stockées sous forme de fichiers textes (JSON et TXT) dans ce repo public, servant de base de données statique pour une future app HTML/JS utilisant Web Speech API pour la récitation vocale (voix françaises homme/femme, vitesse réglable).

## But du Projet
Offrir un outil spirituel pour guider les utilisateurs dans la prière, avec des textes profonds et théologiquement riches. Ce repo contient uniquement les prières en texte brut pour un accès public. L'application complète (interface, TTS) sera développée localement pour confidentialité.

## Structure du Repo
- `/data/` : Contient les prières.
  - `prieres.json` : Fichier JSON central avec toutes les prières (5 initiales, extensible à 111).
  - Sous-dossiers par catégorie :
    - `afflictions_physiques/` : Prières pour maladies, fatigue, etc.
    - `afflictions_emotionnelles/` : Prières pour anxiété, deuil, etc.
    - `demandes_quotidiennes/` : Prières pour protection, travail, etc.
    - `intentions_spirituelles/` : Prières pour foi, pardon, etc.
    - `apocryphes/` : Prières basées sur des textes apocryphes (ex. : Manassé, Siracide).
    - `autres/` : Prières générales (ex. : gratitude, justice).
- `/index.html`, `/styles.css`, `/script.js` : Squelette pour l'app web (à développer localement).
- `/images/` : Placeholders pour icônes ou fonds (ex. : croix, images libres de droits).

## Instructions
1. **Accéder aux Prières** :
   - Téléchargez `prieres.json` ou les fichiers TXT via les URLs raw (ex. : `https://raw.githubusercontent.com/votreusername/PrayerApp-Autonomous/main/data/prieres.json`).
   - Actuellement : 5 prières (1 par catégorie) pour test. Objectif : 111 prières.
2. **Tester l'App** :
   - Activez GitHub Pages (Settings > Pages > Source: main, Folder: /root).
   - Ouvrez `https://votreusername.github.io/PrayerApp-Autonomous/` pour voir `index.html` (squelette pour l'instant).
3. **Ajouter des Prières** :
   - Créez de nouveaux fichiers TXT dans les sous-dossiers (format : Titre, Texte, Verset, Commentaire, Tags).
   - Mettez à jour `prieres.json` avec les nouveaux objets (id, titre, texte, etc.).
4. **TTS (Text-to-Speech)** :
   - L'app utilisera Web Speech API (natif dans les navigateurs) pour réciter les prières.
   - Voix françaises disponibles : Homme (ex. : Microsoft Paul), Femme (ex. : Google français).
   - Vitesse réglable via JS (ex. : speech.rate = 0.5 à 2).
   - Testez les voix dans la console navigateur (speechSynthesis.getVoices()).

## Prochaines Étapes
- Compléter les 111 prières (20 par catégorie + 11 autres).
- Développer l'app localement : HTML/JS pour afficher les prières, CSS pour design apaisant, Web Speech pour TTS.
- Ajouter des images libres de droits dans `/images/` (optionnel).

## Contribution
- Ajoutez des prières via pull requests (respectez le format JSON/TXT).
- Suggestions bienvenues pour thèmes spécifiques (ex. : prières pour chômage, apocryphes).

## Note
Ce repo est public et contient uniquement les textes des prières pour un accès universel. L'app finale, incluant l'interface et TTS, sera développée localement pour confidentialité.

*Créé le 23 septembre 2025*
