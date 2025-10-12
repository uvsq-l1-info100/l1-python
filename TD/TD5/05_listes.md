# TD 5: Listes

---

## 1. Débuts avec les listes

 En plus du cours, n'hésitez pas à consulter la documentation (tutoriel) Python sur les listes [ici (introduction aux listes)](https://docs.python.org/fr/3.6/tutorial/introduction.html#lists) et [ici (complément sur les listes)] (https://docs.python.org/fr/3/tutorial/datastructures.html#more-on-lists).

1. Créer la liste `3, 5, 10`, l'affecter à une variable, puis l'afficher.


2. Ajouter ensuite 12 et 17 à la fin puis afficher à nouveau la liste.


3. Changer le 10 en -7.


4. Avec une boucle `for`, écrire le double de chaque élément de la liste. Cela doit afficher `[6, 10, -14, 24, 34]`. La liste doit être modifiée.


5. A l'aide d'une boucle `for`, ajouter  la valeur `i` à l'élément d'indice `i` de la liste. Cela doit afficher `[6, 11, -12, 27, 38]`. La liste doit être modifiée.


6. Tirer 10 nombres à 2 chiffres au hasard et les mettre dans une nouvelle liste (vide au départ), puis afficher la somme des entiers de la liste et le plus grand de ces entiers.



7. A partir de la liste choisie au hasard, créer une liste qui contient les éléments pairs et une deuxième liste qui contient les éléments impairs.


8. Créer la liste des entiers de 1 jusqu'à 52. Ces entiers représentent les cartes d'un paquet de 52 cartes.


9. Couper le jeu de carte revient à choisir un indice `i` entre 0 et 51, et à passer toutes les cartes allant des indices 0 à i-1 à la suite des cartes qui vont des indices i à 51. Ecrire le code qui effectue une coupe choisie au hasard.
---

## 2. Problème de Syracuse

Cette partie est à traiter dans un script que vous pouvez appeler, par exemple, `syracuse.py`.

En partant d'un entier `n` de départ, on définit une suite d'entiers en obtenant chaque nouveau terme à partir du précédent soit en le divisant par 2 s'il est pair, soit en le multipliant par 3 et en ajoutant 1 s'il est impair.

1. Sans écrire de programme, calculer les premières valeurs de la suite en choisissant `n = 3`.

2. Ecrire la fonction qui, à partir d'un entier initial, renvoie la liste des valeurs successives jusqu'à ce que la valeur `1` soit atteinte (le dernier élément de la liste est donc toujours 1).


```python
def syracuse(n):
    """ Retourne la liste des valeurs de la suite en partant de n jusqu'à 1 """
    pass

print(syracuse(3))
```

3. Le problème de Syracuse affirme que, quel que soit l’entier `n` que l’on choisisse au départ, on finit toujours par arriver à 1 (ce résultat est une *conjecture*, c'est-à-dire qu'il n'a pas été démontré, mais qu'il n'existe pas de contre-exemple connu). Écrire une fonction qui, en appelant la fonction précédente, va vérifier si la conjecture est vraie pour `n` de 1 à `n_max`, où `n_max` est un paramètre de la fonction.

*Remarque*: si tout se passe bien, la fonction doit juste se terminer et renvoyer `True` par exemple. Sinon, c’est qu’on sera entré dans une boucle infinie.


```python
def testeConjecture(n_max):
    """ Teste la conjecture de Collatz pour toutes les valeurs de 1 à n_max """
    pass

print(testeConjecture(10000))
```

4. On appelle *temps de vol* de l’entier `n` le nombre d’étapes pour aller de `n` jusqu’à 1. Le temps de vol de 1 est 0, le temps de vol de 3 est 7. Écrire une fonction qui, étant donné un paramètre `n`, renvoie son temps de vol.


```python
def tempsVol(n):
    """ Retourne le temps de vol de n """
    pass

print("Le temps de vol de", 3, "est", tempsVol(3))
```

5. Ecrire une fonction qui, étant donné un paramètre `n_max` renvoie la liste des temps de vol de tous les entiers de 1 à `n_max`. *Indication*: utiliser une liste en compréhension.


```python
def tempsVolListe(n_max):
    """ Retourne la liste de tous les temps de vol de 1 à n_max """
    pass

print(tempsVolListe(100))
```

6. Déterminer quel entier entre 1 et 10000 a le plus grand temps de vol (réponse 6171 qui a le temps de vol 261).

7. L’altitude maximale de l'entier `n` est la plus grande valeur par laquelle passe `n` au cours de son vol. Déterminer quel entier entre 1 et 10000 a la plus grande altitude maximale (réponse 27114424, atteint par l'entier 9663). Ne pas hésiter à écrire de nouvelles fonctions pour cela.

---

## 3. Carré magique

*Définition* extraite de [l'article Wikipedia sur le carré magique](https://fr.wikipedia.org/wiki/Carr%C3%A9_magique_(math%C3%A9matiques)): en mathématiques, un carré magique d’ordre $n$ est composé de $n^2$ entiers strictement positifs, écrits sous la forme d’un tableau carré. Ces nombres sont disposés de sorte que leurs sommes sur chaque rangée, sur chaque colonne et sur chaque diagonale principale soient égales. On nomme alors *constante magique* la valeur de ces sommes.

Un exemple de carré magique:

$$\begin{bmatrix} 4 & 14 & 15 & 1 \\ 9 & 7 & 6 & 12 \\ 5 & 11 & 10 & 8 \\ 16 & 2 & 3 & 13 \end{bmatrix}$$

1. Sans écrire de programme, vérifier qu'il s'agit bien d'un carré magique, et donner sa constante magique.

Les questions qui suivent doivent être traitées dans un script, qui peut s'appeler `carre_magique.py`. Pensez à utiliser [PythonTutor](http://pythontutor.com/) et les outils de programmation pour résoudre les problèmes qui pourraient survenir.

2. Créer une liste à deux dimensions affectée à  la variable `carre_mag` contenant ce carré magique.

3. Créer une deuxième liste affectée à la variable `carre_pas_mag` qui ne soit pas magique à partir du carré magique en changeant le 3 en 7.

4. Créer une fonction qui affiche la liste comme un carré.


```python
def afficheCarre(carre):
    """ Affiche la liste à 2 dimensions carre comme un carré"""
    pass

afficheCarre(carre_mag)
afficheCarre(carre_pas_mag)

```

5. Ecrire une fonction qui teste si les lignes du carré ont toutes la même somme. Cette fonction renvoie cette somme si c'est le cas, et `-1` sinon.


```python
def testLignesEgales(carre):
    """ Renvoie la somme des éléments d'une ligne de la liste 2D carre si toutes les lignes ont la même somme, et -1 sinon """
    pass

print(testLignesEgales(carre_mag))
print(testLignesEgales(carre_pas_mag))

```

6. Même question mais en testant les colonnes.


```python
def testColonnesEgales(carre):
    """ Renvoie la somme des éléments d'une colonne de la liste 2D carre si toutes les colonnes ont la même somme, et -1 sinon """
    pass

print(testColonnesEgales(carre_mag))
print(testColonnesEgales(carre_pas_mag))
```

7. Même question mais en testant les 2 diagonales.


```python
def testDiagonalesEgales(carre):
    """ Renvoie la somme des éléments d'une diagonale de la liste 2D carre si les 2 diagonales ont la même somme, et -1 sinon """
    pass

print(testDiagonalesEgales(carre_mag))
print(testDiagonalesEgales(carre_pas_mag))
```

8. Créer une fonction qui teste si un carré est magique. Elle retourne `True` si c'est le cas et `False` sinon.


```python
def estCarreMagique(carre):
    """ Renvoie True si c'est un carre magique et False sinon"""
    pass

print(estCarreMagique(carre_mag))
print(estCarreMagique(carre_pas_mag))
```

9. Un carré d'ordre $n$ est *normal* s'il contient tous les entiers de 1 à $n^2$. Ecrire une fonction qui teste si un carré est normal (pas nécessairement magique).


```python
def estNormal(carre):
    """ Retourne True si contient toutes les valeurs de 1 à n^2 où n est la taille
        du carré, et False sinon """
    pass

print(estNormal(carre_mag))
print(estNormal(carre_pas_mag))
```
