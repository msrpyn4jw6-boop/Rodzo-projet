# Rodzo Parkour

Jeu de parcours d'obstacles en 3D (genre « obby »), jouable dans le navigateur. Tout tient dans `index.html` ; Three.js r128 est chargé depuis cdnjs.

## Jouer

Ouvrir `index.html` dans un navigateur (une connexion internet est nécessaire pour charger Three.js et les polices).

| Action | Clavier / souris | Tactile |
| --- | --- | --- |
| Se déplacer | ZQSD, WASD ou flèches | Pouce gauche (joystick) |
| Sauter | Espace | Bouton « Saut » |
| Caméra | Glisser la souris, molette pour zoomer | Glisser à droite de l'écran |
| Retour au point de sauvegarde | R | Bouton « Retour » |

## Les 8 étapes

1. Premiers sauts
2. Le couloir de lave (blocs rouges mortels)
3. Plates-formes mobiles
4. Dalles fragiles (disparaissent après qu'on marche dessus)
5. Le tremplin
6. Les poutres
7. La pale tournante
8. La tour finale, avec le drapeau doré au sommet

Le meilleur temps est gardé dans le navigateur (`localStorage`).
