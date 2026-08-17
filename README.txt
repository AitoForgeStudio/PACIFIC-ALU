PACIFIC-ALU — version hors connexion

Fichiers :
- index.html : application complète
- sw.js : cache/offline PWA
- manifest.json : installation comme application

Installation GitHub :
1. Remplace ton index.html par celui-ci.
2. Ajoute sw.js à la racine du dépôt.
3. Ajoute manifest.json à la racine du dépôt.
4. Active GitHub Pages sur la branche main.
5. Ouvre l'application une première fois avec Internet.
6. Installe-la sur Android depuis Chrome si proposé.

Firebase :
La version utilise le cache local persistant Firestore. Les modifications faites hors connexion restent dans le cache local et sont synchronisées lorsque la connexion revient.

Important :
Les photos sont stockées en base64 dans Firestore comme dans ta version actuelle. Beaucoup de grosses photos peuvent faire dépasser la limite de taille d'un document Firestore. Pour un grand nombre de photos, il faudra ensuite passer les photos dans Firebase Storage.
