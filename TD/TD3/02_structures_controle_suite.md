## 1. Premiers exercices avec les structures itératives

**Exercice 3 :** Suivi de consommation d'eau

Une famille souhaite suivre sa consommation d'eau pendant plusieurs jours.
Le programme demande à l'utilisateur de saisir le nombre de jours à analyser.Pour chaque jour, l'utilisateur saisit la quantité d'eau consommée en litres.

Le programme doit ensuite déterminer :

- la consommation totale pendant la période ;
- la consommation moyenne par jour ;
- le nombre de jours où la consommation a dépassé **150 litres** ;
- la plus grande consommation enregistrée.

### Partie 1

Écrire une solution en utilisant une boucle `for`. Le programme doit fonctionner pour un nombre de jours quelconque.

Par exemple, pour 5 jours :

Jour 1 : 120
Jour 2 : 180
Jour 3 : 140
Jour 4 : 200
Jour 5 : 160


Le programme doit afficher :

Consommation totale : 800 litres
Consommation moyenne : 160 litres
Nombre de jours dépassant 150 litres : 3
Plus grande consommation : 200 litres

### Partie 2

Écrire une deuxième solution permettant d'obtenir les mêmes résultats, mais en utilisant une boucle `while` à la place de la boucle `for`.

### Partie 3

Modifier le programme afin de signaler également si la consommation moyenne de la famille est :

- inférieure ou égale à 120 litres : **« Consommation faible »** ;
- supérieure à 120 litres et inférieure ou égale à 150 litres : **« Consommation normale »** ;
- supérieure à 150 litres : **« Consommation élevée »**.

Faire les calculs à la main pour l'exemple avant d'écrire le programme.


**Exercice 2 :**: Gestion d'un distributeur de billets

On souhaite simuler le fonctionnement simplifié d'un distributeur de billets.

Le distributeur dispose initialement de :

- 100 billets de 10 € ;
- 50 billets de 20 € ;
- 30 billets de 50 €.

Un client peut effectuer plusieurs retraits successifs.

Pour chaque retrait, le programme demande la somme souhaitée.

La somme doit respecter les règles suivantes :

- elle doit être strictement positive ;
- elle doit être un multiple de 10 ;
- le retrait ne peut pas dépasser 500 €.

Si la somme demandée n'est pas valide, le programme affiche un message d'erreur et demande une nouvelle somme.

Lorsque la somme est valide, le distributeur doit déterminer combien de billets de 50 €, de 20 € et de 10 € sont nécessaires pour constituer la somme demandée.

Le programme doit également vérifier que le distributeur possède suffisamment de billets.

Après chaque retrait accepté, les quantités de billets disponibles sont mises à jour.

Le client peut ensuite effectuer un nouveau retrait.

Lorsqu'il saisit `0`, le programme s'arrête et affiche :

- le nombre de retraits effectués ;
- le montant total distribué ;
- le nombre de billets de 10 €, 20 € et 50 € restant dans le distributeur.

Exemple de déroulement :

Montant du retrait : 120

Retrait accepté.
Billets distribués :
2 billet(s) de 50 €
1 billet(s) de 20 €
0 billet(s) de 10 €

Montant du retrait : 70

Retrait accepté.
Billets distribués :
1 billet(s) de 50 €
1 billet(s) de 20 €
0 billet(s) de 10 €

Montant du retrait : 0

Nombre de retraits : 2
Montant total distribué : 190 €

Question de réflexion :

Avant d'écrire le programme, déterminer à la main les billets utilisés pour les retraits suivants :

40 €
80 €
130 €
270 €
500 €

Puis déterminer l'état du distributeur après avoir effectué successivement :

80 €
130 €
50 €
0

"""

**Exercice 3 :** Supposons que vous souhaitiez développer un programme permettant à un élève de première année de s'entraîner à la soustraction. Le programme génère de manière aléatoire deux entiers d'un seul chiffre, number1 et number2, avec number1 >= number2, et pose à l'élève une question telle que "Quel est 9 - 2 ?" Après que l'élève ait saisi la réponse, le programme affiche un message indiquant si elle est correcte. Ecrire un programme qui génère cinq questions et, après qu'un élève y ait répondu, rapporte le nombre de réponses correctes. Le programme affiche également le temps passé sur le test, comme le montre l'exécution d'exemple. Pour mesurer le temps, il faut importer la bibliothèque *Time* (exemple d'utilisation: temps_de_depart = time.time()).



**Exercice 2 :**  L'exemple précédent exécute la boucle cinq fois. Si vous souhaitez que l'utilisateur décide s'il souhaite prendre une autre question, vous pouvez proposer une confirmation à l'utilisateur (en tapant 'Y' pour continuer).



**Exercice 3 :**  (Trouver les nombres divisibles par 5 et 6) Écrivez un programme qui affiche, dix nombres par ligne, tous les nombres de 100 à 1 000 qui sont divisibles par 5 et 6. Les nombres sont séparés par exactement un espace.



**Exercice 4 :**  Écrivez un programme qui joue au populaire jeu ciseaux-pierre-papier. (Un ciseau peut couper du papier, une pierre peut écraser un ciseau, et du papier peut envelopper une pierre.) Le programme génère aléatoirement un nombre 0, 1 ou 2, représentant respectivement ciseaux, pierre et papier. Ensuite, le programme demande à l'utilisateur d'entrer un nombre 0, 1 ou 2, puis affiche un message indiquant si l'utilisateur gagne, perd ou obtient un match nul par rapport à l'ordinateur. Le programme  permet à l'utilisateur de jouer en continu jusqu'à ce que l'utilisateur ou l'ordinateur gagne plus de deux fois.



**Exercice 5 :** Écrivez un programme pour vérifier la validité des mots de passe saisis par les utilisateurs. Supposons que les mots de passe doivent contenir:

    -Au moins 1 lettre entre [a-z] et 1 lettre entre [A-Z].
    -Au moins 1 chiffre entre [0-9].
    -Au moins 1 caractère parmi [$#@].
    -Longueur minimale de 6 caractères.
    -Longueur maximale de 16 caractères.

1. Faites l'exercice en utilisant seulement la syntaxe vue en cours.     

2. Proposez en deuxième programme en utilisant cette fois la fonction *re.search()* du module *re* en Python. Cette fonction est utilisée pour rechercher un motif (expression régulière) dans une chaîne de caractères. Voici la syntaxe simplifiée de re.search() : re.search(pattern, string)

    -pattern : C'est le motif (expression régulière) que vous souhaitez rechercher dans la chaîne de caractères.
    -string : C'est la chaîne de caractères dans laquelle vous souhaitez effectuer la recherche.

La fonction re.search() renvoie un objet de correspondance (match object) si le motif est trouvé dans la chaîne de caractères. Si le motif n'est pas trouvé, elle renvoie None.    

**Exercice 6 :** Écrivez un premier programme qui permet de chiffrer une chaîne de caractères en utilisant un décalage de x lettres vers la droite dans l'ordre de l'alphabet. Attention, x est un entier dont les valeurs sont comprises entre 0 et 25.

    Exemple : Si on fait un décalage de 3, le mot "bonjour" devient "erqmrxu"

Dans un deuxième temps, écrivez également le programme qui déchiffre le mot, en retrouvant le mot initial à partir d'un mot chiffré et de l'entier utilisé pour le décalage.
