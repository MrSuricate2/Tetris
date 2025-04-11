# Tetris vs IA

Un projet de jeu Tetris à deux joueurs (Humain vs IA) développé en HTML, CSS et JavaScript vanilla, créé à l'aide de prompts d'IA.

## 📋 Description

Ce projet a été réalisé dans le cadre d'un cours sur l'interaction avec l'intelligence artificielle. L'objectif était de créer un jeu Tetris compétitif où un joueur humain affronte une IA, le tout en utilisant uniquement des technologies web standards (sans frameworks).

Le jeu a été développé en guidant une IA générative à travers une série de prompts soigneusement conçus pour obtenir un code fonctionnel et optimisé, avec des règles amusantes qui enrichissent l'expérience de jeu.

## 🎮 Fonctionnalités principales

### Deux grilles
- Une grille pour le joueur humain et une pour l'IA, affichées côte à côte
- Interface visuelle claire permettant de suivre les deux parties simultanément

### Contrôles
- **Humain** : Flèches du clavier (gauche, droite, bas, haut pour tourner)
- **IA** : Joue automatiquement avec une logique simple (placement optimal des pièces)

### Tableau des scores
- 50 points par ligne complétée
- Bonus : 100 points pour 2 lignes, 200 pour 3 lignes, 300 pour un Tetris (4 lignes)
- Affichage en temps réel des scores des deux joueurs

## 🛠️ Technologies utilisées

- **HTML5** - Structure de la page avec `<canvas>` ou grilles de `<div>` pour les terrains de jeu
- **CSS3** - Stylisation, animations (notamment pour la disparition des lignes) et effets visuels
- **JavaScript Vanilla** - Logique de jeu, tableaux 2D pour les grilles et algorithmes d'IA
- **IA générative** - Aide à la génération du code via prompts

## 🚀 Installation et lancement

1. Clonez ce dépôt :
   ```
   git clone https://github.com/MrSuricate2/Tetris.git
   ```

2. Naviguez vers le répertoire du projet :
   ```
   cd Tetris
   ```

3. Ouvrez le fichier `index.html` dans votre navigateur préféré.

Aucune dépendance externe ou installation supplémentaire n'est nécessaire !

## 🎯 Comment jouer

- **Flèche gauche/droite** : Déplacer les pièces horizontalement
- **Flèche bas** : Accélérer la chute
- **Flèche haut** : Rotation des pièces

L'IA joue automatiquement sur sa propre grille pendant que vous jouez sur la vôtre. Le tableau des scores vous permet de suivre qui est en tête. Soyez attentif aux règles spéciales qui s'activent pendant la partie pour maximiser votre score !

## 🧠 Architecture de l'IA adversaire

L'intelligence artificielle implémentée est intentionnellement simple mais compétitive :

- Elle analyse où chaque pièce "fit" le mieux dans la grille
- Elle évalue les mouvements possibles (rotation, déplacement)
- Elle prend ses décisions rapidement, sans trop de calculs complexes
- Elle est conçue pour être un adversaire stimulant sans être imbattable

Cette approche correspond à la consigne de créer une IA qui "pose les pièces là où ça fit le mieux" sans être trop sophistiquée, rendant le jeu compétitif mais accessible.

## 🎁 Règles fun (version soft)

Le jeu intègre plusieurs règles amusantes qui rendent l'expérience plus engageante :

1. **Cadeau surprise** : Quand un joueur complète 2 lignes d'un coup, l'adversaire reçoit une "pièce facile" (carré ou ligne droite).

2. **Pause douceur** : Tous les 1 000 points, les pièces tombent 20% plus lentement pendant 10 secondes pour les deux joueurs.

3. **Pièce rigolote** : Tous les 3 000 points, une pièce spéciale apparaît (forme de cœur ou d'étoile), qui vaut 100 points bonus si bien placée.

4. **Échange amical** : Si un joueur fait un Tetris (4 lignes), il peut échanger une de ses lignes pleines avec une ligne vide de l'adversaire.

5. **Arc-en-ciel** : Toutes les 2 minutes, les pièces changent de couleur pendant 20 secondes pour un effet visuel plaisant.

## 📝 Licence

Ce projet est sous licence [MIT](LICENSE).
