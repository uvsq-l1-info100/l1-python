#  TD 9 : Modules



## Exercice 1: Le module math

1. Créez une liste qui contient les racines carrées de toutes les entiers de 1 à 10.

2. En utilisant la fonction `ceil` du module math faites afficher la liste des parties entiers des racines carrées calculées à la question précédente.

3. Créez une matrice `4x4`  qui contient toutes les racines carrées de nombres allant de 1 à 16. Ainsi, la première ligne contient les racines carrées des entiers de 1 à 4, la deuxième ligné les racines des entiers de 5 à 8 etc.


## Exercice 2: Probabilité et fréquence - somme de 2 dés égale à 6 - simulation

On lance deux dés non truqués à 6 faces numérotées de 1 à 6. On s'intéresse à la probabilité que la somme des dés soit égale à 6.

1. Écrire un programme en Python qui simule 100 lancers et affiche la fréquence d'apparition de la somme des dés égale à 6.

2. Modifier le programme pour que l'utilisateur puisse choisir le nombre de lancers.


## Exercice 3: Le module time

Pour cette exercice, il faudra consulter la [documentation du module time](https://docs.python.org/3/library/time.html).
Écrire un programme permettant d'afficher l'heure courante, et d'indiquer le nombre de minutes passées depuis le début du TP.
Attention, la fonction `time()` renvoie le temps en secondes depuis un moment nommé epoch, qui correspond à 1 Janvier 1970 00:00:00 (UTC).


## Exercice 4 : Un premier module

1. Dans un fichier nommé mon_module.py écrire une fonction qui, à partir d'une liste d'entiers, calcule le min de la liste et renvoie sa valeur ainsi que son indice dans la liste.
2. Rajoutez une fonction calculant le max d'une liste et une fonction calculant la moyenne des éléments dans la liste.
3. Créer un fichier exo4.py. Dans ce fichier déclarez une liste. Dans le programme dans exo4.py, appelez les fonctions de mon_module.py. Que faudrait-il faire?
