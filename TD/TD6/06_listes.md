#  TD 6 : Encore des listes


## 1. Revoir les notions vues en cours

1. Créer une fonction qui prend en entrée une liste et qui renvoie une nouvelle liste, correspondant à la liste inversée. Seules les opérations sur les *tranches* de liste sont admises.



2.  Écrire un programme qui demande à l'utilisateur de donner un entier $m$ et qui affiche la table de multiplication de $m$ en une seule commande en utilisant les instructions range() et list().

3.  En utilisant les tests d'appartenance vu en cours, écrire un programme qui prend en entrée une liste et qui renvoie une nouvelle liste contenant les mêmes éléments, mais sans doublons.


4. Compléter la fonction `compter_negatives()` qui prend en argument une liste des nombres et renvoie le nombre d'entrées négatives.


```python
def compter_negatives(nombres) :
    """Renvoie le nombre d'éléments < 0 de la liste passée en paramètre. """

    # Utiliser une boucle
    pass

compter_negatives([3, -1, 1.5, 5, -6.3, -7.9, 2])

```

5. Compléter la fonction suivante qui prend en entrée deux chaînes de caractères et qui renvoie une liste contenant les mots communs de ces deux chaînes.


```python
def motsCommuns(mot1, mot2) :
    """ Fonction qui prend en entrée deux chaînes de caractères et renvoie une liste contenant
        les mots communs de ces deux chaînes."""

    # Compléter


listeMotsCommuns = motsCommuns("Python est un langage de programmation sympa", "Programmer en Python est facile")
print("Les mots communs sont :", listeMotsCommuns)
```


## 2. Ecrire un programme plus complexe

###1. Jeu Scrabble simplifié

En *Scrabble* le tirage des 7 lettres est dit *valide* quand celui-ci comporte au moins 2 voyelles.

On simplifie le jeu en supposant que seules les lettres (E, A, I, N, O, R, S, T) peuvent être tirées.

On suppose qu'on a un sac constritué de ces 8 lettres dans les quantités suivantes :

  * A : 9 fois
  * E, I, N, O, R, S, T : 6 fois pour chacune de ces lettres.

Écrire un programme qui tire au hasard 7 lettres dans le sac :
  * si le tirage est valide, afficher le tirage et arrêter.
  * si le tirage n'est pas valide, recommencer.

### 2. Jeu de morpion

Le jeux de morpion (ou tic-tac-toe) se joue généralement sur une grille de 3*3 cases
ou de 5*5 cases.Écrire un programme demandant aux joueurs la dimension de la grille sur laquelle ils veulent
jouer, et leur permettant de faire une partie. Le gagnant est le joueur alignant un symbole identique (’X’ ou ’O’) sur une ligne, sur une colonne ou sur une diagonale.

  — Initialisez une grille vide

  — Écrire le code permettant à un joueur de choisir sur quelle ligne et quelle colonne il souhaite
  jouer

  — Écrire des fonctions permettant de savoir si une ligne, une colonne, la 1ère diagonale et la
  2ème diagonale sont gagnantes

  — Rassembler le tout pour permettre à 2 joueurs de faire une partie, avec une interface raison-
  nablement conviviale.

Une attention particulière sera portée aux possibles eﬀets de bords (débordement de grille, deux coups sur la même case, etc...)
