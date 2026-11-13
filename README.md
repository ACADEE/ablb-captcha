# ABLB CAPTCHA

Jeu de patience et de logique : dix défis successifs avec validation, progression et écran de réussite animé.

## Démarrage

```sh
python3 -m http.server 8080 --directory dist
```

Ouvrir http://localhost:8080. Le fichier `dist/index.html` est autonome, sans dépendance ni compilation.

## Parcours

1. Cliquer sur « Commencer les 10 défis ».
2. Sélectionner et valider une réponse à chaque épreuve. Une réponse incorrecte permet de réessayer.
3. Terminer les dix défis pour afficher « Bravo, vous avez une grande patience ! » et deux jets de confettis.
4. Rejouer à volonté.

Les confettis respectent la préférence système de réduction des animations.

## Confidentialité

Aucun compte, aucune donnée personnelle, aucun stockage et aucun appel réseau applicatif. L'application ne représente pas une banque et ne réalise aucune opération bancaire.

## Déploiement

Publier le répertoire `dist` sur un hébergement statique.
