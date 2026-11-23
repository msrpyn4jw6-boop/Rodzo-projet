# Rodzo

Un petit monde de jeux dans le navigateur, avec un menu d'accueil façon plateforme de jeux : recherche, catégories (Horreur, Obby, Tycoon…), fiche de chaque jeu et bouton Jouer.

Jeux disponibles :
- **Les Salles-Piscines** : une immense salle carrelée noyée de brume, avec de grandes plateformes au-dessus d'une eau verte. Il faut trouver 5 jetons puis la sortie, pendant qu'une créature noire à quatre pattes marche sur les plateformes et nage. Elle se guide au bruit.
- **Rodzo Parkour** : 9 étapes au-dessus de l'eau, avec un serpent attiré par les éclaboussures.
- **Salon Rodzo** : l'espace social où l'on retrouve ses amis.
- Annoncés « Bientôt » : Rodzo Tycoon, Cache-cache, Course de bateaux.

Dans l'eau, Espace fait sauter sur une plateforme.

## Lobby, amis et avatar

- **Salon** : une grande salle-piscine carrelée, avec des portails vers les jeux.
- **Amis** : sur claude.ai, les personnes invitées à la page (menu Partager, par e-mail) se voient en direct dans le lobby et pendant les parties, avec leur pseudo et un chat. Avec le simple lien public, on joue seul.
- **Avatar** : couleurs du corps, des jambes, de la peau, des yeux, chapeaux et accessoires de dos. Une partie est gratuite, le reste s'achète avec des **Rodzos**, la monnaie du jeu (gagnée aux étapes, à l'arrivée et avec le bonus du jour). Il n'y a pas de paiement en argent réel.
- La sauvegarde (pseudo, Rodzos, objets) est gardée dans le navigateur et, quand c'est possible, dans le compte Claude du joueur.

## Rodzo Parkour

Jeu de parcours d'obstacles en 3D (genre « obby »), jouable dans le navigateur, sur ordinateur comme sur téléphone. Tout tient dans `index.html` ; Three.js r128 est chargé depuis cdnjs.

Une créature noire vit dans l'eau sous le parcours. Elle ne voit rien mais entend chaque bruit d'eau : plongeon, brasse, pas sur les dalles immergées. Les pierres ramassées sur les plateformes, lancées dans l'eau, l'attirent ailleurs. Quand on tombe, on nage et on est repêché au bout de 4 s, sauf si le monstre arrive avant.

## Jouer

Ouvrir `index.html` dans un navigateur (une connexion internet est nécessaire pour charger Three.js et les polices).

| Action | Clavier / souris | Tactile |
| --- | --- | --- |
| Se déplacer | ZQSD, WASD ou flèches | Pouce gauche (joystick) |
| Sauter | Espace | Bouton « Saut » |
| Marcher sans bruit | Maj | Joystick poussé à moitié |
| Lancer une pierre | Clic ou F | Bouton « Lancer » |
| Caméra | Cliquer sur le jeu puis bouger la souris (Échap pour libérer), molette pour zoomer | Glisser à droite de l'écran |
| Retour au point de sauvegarde | R | Bouton « Retour » |

## Les 9 étapes

1. Premiers sauts
2. Le couloir piégé (blocs rouges)
3. Plates-formes mobiles
4. Dalles fragiles (disparaissent après qu'on marche dessus)
5. La piscine embrumée (salle fermée, fumée, dalles au ras de l'eau)
6. Le tremplin
7. Les poutres
8. La pale tournante
9. La tour finale, avec le drapeau doré au sommet

Six tenues au choix (bouton « Tenue »). Le meilleur temps et la tenue sont gardés dans le navigateur (`localStorage`).
