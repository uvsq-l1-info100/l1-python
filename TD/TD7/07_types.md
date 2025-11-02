#  TD 7 : Encore des types


## 1. Revoir les notions vues en cours

1. Étant donnés deux entiers entrés au clavier - le nombre de lignes *m* et de colonnes *n* d’une liste 2D *m×n* - suivis de la saisie de *m* lignes de *n* entiers, puis de deux entiers non négatifs *i* et *j* plus petits que *n*, échanger les colonnes *i* et *j* de la liste 2D et afficher le résultat.


2.  Étant donné un entier *n* entré au clavier, créer et afficher une liste 2D de taille n×n suivant les règles ci-dessous :

    -Sur l’anti-diagonale, mettre la valeur 1.

    -Sur les diagonales au dessus mettre la valeur 0.

    -Sur les diagonales en dessous mettre la valeur 2.


    Exemple de sortie pour *n=4*.

    ```python
    0 0 0 1
    0 0 1 2
    0 1 2 2
    1 2 2 2
    ```


3.  Pour cet exercice vous devez utiliser les tranches. Les boucles ne sont pas autorisées. Étant donnée une chaîne de caractères entrée au clavier :

    -Sur la première ligne, afficher le troisième caractère de cette chaîne.

    -Sur la seconde ligne, afficher du deuxième jusqu’au dernier caractère de cette chaîne.

    -Sur la troisième ligne, afficher la chaîne à l’envers, tous les deux caractères, en commençant par le dernier.

    -Sur la quatrième, afficher tous les caractères sauf les deux derniers de la chaîne.


4. Étant donnée une chaîne de caractères entrée au clavier, retirer tous ses caractères dont les indices sont divisibles par 3.


5. Étant donnée une série d’entiers (séparés par des espaces) entrée au clavier, compter combien de nombres différents elle contient et afficher ce comptage. Ce problème peut être résolu en une seule ligne.


6. Étant données deux séries de nombres (séparés par des espaces) entrées au clavier l’une après l’autre, compter combien de nombres de la première série apparaissent dans la seconde et afficher ce comptage.

Exemple d'entrée

```python
1 3 2
4 3 2
```
Exemple de sortie

```python
2
```

7. Nous souhaitons écrire une application qui prend en entrée les résultats d'une election présidentielle par région et qui doit comptabiliser les votes totales et le gagnant. Les résultats par région sont rentrés au fur et à mesure par l'utilisateur. Vous devez mettre à jour les résultats par candidat en utilisant la structure de données la plus adaptée parmi celles vues en cours.

Exemple d'entrée

```python
Norcam  1201
El Nep 324
Fachon 17
Norcam 2443
El Nep 4567
```

Exemple de sortie

```python
Norcam : 12567, El Nep 5678, Fachon : 3456
```

## 2. Ecrire un programme plus complexe

Pour cette partie, vous devez "découper" chaque programme en plusieurs fonctions. Avant de commencer à coder, vérifiez avec votre chargé de TD que votre
choix de fonctions est correct.


### 1. Fréquence des lettres dans la langue française

A partir d'un texte en langue française, vous analyserez le nombre d'occurrences de chaque lettre, qu'elle soit majuscule ou minuscule. En utilisant une structure de données adaptée, vous devez faire obtenir un affichage comme ci-dessous:  

```python
   A : 18 fois
   B: 3 fois
   C: 5 fois
   ...
```  

Ensuite, vous calculerez la fréquence des lettres en pourcentage. Ecrivez une fonction qui prend un argument un texte, calcule la fréquence des lettres et la compare à la fréquence des lettres en langue française:

https://fr.wikipedia.org/wiki/Fr%C3%A9quence_d%27apparition_des_lettres

Testez votre programme sur des textes de plus en plus longs. Que constatez vous?

### 2. Fréquence d'un mot dans un texte

On souhaite maintenant analyser la fréquence des mots dans un texte.
Le texte, composé de mots séparés par un espace, est entré sur une seule ligne (et lu en une seule fois). Pour chaque mot du texte, il faut compter et afficher le nombre d’occurrences préalables de ce mot (i.e., le nombre de fois qu’il est déjà apparu à gauche, avant le mot courant).

En entrée

```python
one two one two three two four three
```

En sortie:

```python
0 0 1 1 0 2 0 1
```

Dans un deuxième temps vous afficherez les mots et leur fréquence en suivant leur ordre d'apparition dans un dictionnaire:

En sortie:

```python
four : 1
one  : 2
three : 2
two : 3
```
