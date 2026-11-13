# ABLB CAPTCHA

Prototype ludique d’une banque fictive suivi de dix défis de vérification humaine. La simulation est identifiée dans l’interface et ne traite aucune opération bancaire réelle.

## Démarrage

Aucune dépendance à installer. Depuis la racine du dépôt :

```sh
python3 -m http.server 8080 --directory dist
```

Ouvrir http://localhost:8080.

## Parcours

1. Saisir un e-mail quelconque et le code de démonstration `1234`.
2. Consulter le solde fictif de 9 600 000 €.
3. Cliquer sur « Faire un virement ».
4. Réussir les dix défis. Le mode démo permet de naviguer entre les écrans et de pré-sélectionner les solutions.
5. Afficher le message « Bravo, vous avez une grande patience ! » avec une animation de confettis.

Les confettis respectent la préférence système de réduction des animations.

## Données

Les saisies restent en mémoire dans le navigateur et sont effacées après connexion. Aucun e-mail ni code n’est envoyé à un serveur. Pas de webhook, de traqueur, de stockage de données personnelles ou de connexion à une banque réelle.

## Contenu

- `dist/index.html` : écrans et structure.
- `dist/style.css` : présentation responsive.
- `dist/app.js` : dix défis et validation.
- `dist/bank.js` : navigation et connexion de démonstration.
- `dist/confetti.js` : animation de réussite.
- `dist/assets/` : dix images générées pour le prototype.

Site statique sans compilation, installable sur tout hébergement statique dont la racine est `dist`.
