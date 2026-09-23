# Mon Talmud V3

Cette version synchronise les coches entre PC et iPhone grâce à Firebase/Firestore.

## Coût
- Hébergement : GitHub Pages peut être utilisé gratuitement avec GitHub Free (dépôt public).
- Firebase : le forfait Spark est sans frais, sans carte bancaire requise pour démarrer, avec des quotas gratuits largement suffisants pour cet usage.
- Domaine personnalisé : optionnel et payant si tu veux une adresse du type montalmud.fr.

## Mise en ligne
1. Crée un compte GitHub.
2. Crée un dépôt public, par exemple `mon-talmud`.
3. Mets `index.html`, `firebase-config.js` et `manifest.webmanifest` à la racine.
4. Dans Firebase Console, crée un projet.
5. Ajoute une application Web et copie la configuration dans `firebase-config.js`.
6. Active Authentication > Google.
7. Crée Firestore Database.
8. Mets les règles Firestore fournies dans `firestore.rules`.
9. Dans GitHub: Settings > Pages > Deploy from branch > main > /root.
10. Ouvre l'adresse GitHub Pages sur PC et iPhone.
11. Sur iPhone: Safari > Partager > Sur l'écran d'accueil.
12. Connecte-toi avec le même compte Google sur les deux appareils.

IMPORTANT : le `firebaseConfig` côté navigateur n'est pas un secret. En revanche, ne mets jamais de clé privée/service account dans le dépôt.
