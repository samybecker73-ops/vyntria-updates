# Processus de publication VYNTRIA

Ce dépôt public est réservé aux versions validées et à leurs métadonnées.

## Procédure manuelle initiale

1. Préparer le build depuis le dépôt privé `vyntria`.
2. Tester le programme et vérifier que l'installateur démarre correctement.
3. Calculer une empreinte SHA-256 de chaque fichier distribué.
4. Créer une GitHub Release avec un tag `vMAJOR.MINOR.PATCH`.
5. Joindre les installateurs/archives comme assets de la Release.
6. Publier les notes de version.
7. Mettre à jour le manifeste de mise à jour après validation du format attendu par l'application.

## Manifeste

`latest.example.json` illustre un format possible, à confirmer à partir du code du mécanisme de mise à jour de VYNTRIA. Il ne constitue pas encore un endpoint de mise à jour actif.

## Règles

- Ne pas publier de version non testée.
- Ne jamais inclure de secrets ou de données utilisateurs.
- Vérifier que chaque URL d'asset est accessible avant d'annoncer une mise à jour.
- Ne pas automatiser les publications avant d'avoir validé le processus et le cadre d'utilisation des automatisations.
