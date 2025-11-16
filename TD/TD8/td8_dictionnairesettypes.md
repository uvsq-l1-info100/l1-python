#  TD 8 : Dictionnaires, annotations de type



Lors de cette séance nous aurons besoin d'installer mypy.
Pour cela, il faut avoir sur vos machines une version Python 3.9 ou plus récente et une connexion internet.

Pour installer en ligne de commande :

```python
$ python3 -m pip install mypy
```

Une fois l'outil installé, vous pouvez tester votre programme en ligne de commande, avec la commande

```python
$ mypy program.py
```

Une fois l'outil installé, vous pouvez l'utiliser depuis Visual Code Studio en installant l'extension Mypy (onglet Extensions dans la barre à gauche, chercher Mypy et installer)

## Exercice n°1 — Double hachage

Le double hachage est l’une des meilleures méthodes connues pour l’adressage ouvert.  
Il utilise une fonction de hachage de la forme :

$h : \mathbb{N} \times \mathbb{N} \longrightarrow [0, m-1]$

$(k, i) \longmapsto (h_1(k) + i \times h_2(k)) \mod m$

où $h_1$ et $h_2$ sont des fonctions de hachage.  
La variable *i* prend les valeurs suivantes :

- Par défaut, *i = 0*.
- S’il y a collision, on incrémente *i* de *1, jusqu’à ne plus avoir de collision pour la clé considérée.
- Il reprend la valeur 0 pour la clé suivante…

---
### Q1

Programmez les fonctions suivantes en utilisant une seule ligne de code, en utilisant des fonctions lambda:

- $h_1(k) = k \mod 13$
- $h_2(k) = 1 + (k \mod 12)$

---

### Q2.
Insérer les clés :  
**5, 28, 19, 15, 20, 33, 12, 17, 10**  
dans un tableau de taille **m = 13** avec les fonctions de l'exercice précédent.

---

### Q3.
Proposer une fonction en **Python** qui prend en argument une clé `c` (entier) et la taille `m` de la table, et renvoie la valeur de `h(c)`.

---

### Q4.
Dans un fichier part, reprendre l'exercice et reécrire toutes les fonctions en rajoutant les annotation de type. A chaque exécution, Testez votre code avec mypy.


## Exercice n°2 — Problème de Syracuse

Reprendre le code de l'exercice 2 du TD 5. Rajoutez des annotations de type pour toutes les fonctions et testez votre code avec mypy.
