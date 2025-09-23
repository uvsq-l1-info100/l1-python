---

## 1. Premiers exercices avec les structures conditionnelles

**Exercice 1:**

1. Soit *num1 = 15* et *num2 = 5*. Ecrire un programme qui affiche *Factors!* si l'un des nombres est un facteur de l'autre (c'est-à-dire qu'il divise l'autre nombre). Si aucun des nombres n'est un facteur de l'autre, le programme n'affiche rien.
2. Changer le code que vous avez écrit de telle sorte qu'il affiche toujours *Factors!* si un nombre est un facteur de l'autre, mais qui affiche aussi *Not factors!* si aucun des nombres n'est un facteur de l'autre.


**Exercice 2:**

Soit *state = "Georgia"*. Ecrire un programme qui permet d'afficher un message spécifique en fonction de la variable *state* :  
* "School isn't cancelled." si nous sommes à New Jersey,  
* "School is postponed." si nous sommes à North Carolina,
* "School is cancelled!" si nous sommes à Georgia,  
* "School's status is unknown" si nous ne sommes pas dans un des trois états précédemment mentionnés.



**Exercice 3:**

Ecrire un programme pour découvrir le signe du zodiaque chinois pour une année donnée. Le signe du zodiaque chinois est basé sur un cycle de 12 ans et chaque année de ce cycle est représentée par un animal :
* 0: monkey
* 1: rooster
* 2: dog
* 3: pig
* 4: rat
* 5: ox
* 6: tiger
* 7: rabbit
* 8: dragon
* 9: snake
* 10: horse
* 11: sheep

La valeur de l'année % 12 détermine le signe du zodiaque. Par exemple, 1900 est l'année du *rat* puisque 1900 % 12 est 4.



**Exercice 4:**

Soit *temperature = -3.7* et *celsius = True*. *celsius* est une variable booléenne qui indique si la température est en Celsius; si c'est *False*, alors la température donnée est en Fahrenheit. Ecrire un premier programme en utilisant *if-else* seulement qui permet d'afficher *Freezing* si les valeurs données représentent une température très basse, et *Not freezing* si ce n'est pas le cas. En Celsius, on considère qu'il fait très froid lorsque la température est inférieure ou égale à 0 degré. En Fahrenheit, on considère qu'il fait très froid lorsque la température est inférieure ou égale à 32 degrés. Proposer une seconde solution en utilisant *if-elif-else* à ce même problème.


**Exercice 5:**

Ecrire un programme qui permet de déterminer si une année est bissextile ou non en utilisant une seule instruction *if-else*. Une année *A* est bissextile si *A* est divisible par 4. Elle ne l’est cependant pas si *A* est un multiple
de 100, à moins que *A* ne soit multiple de 400.    



**Exercice 6:**

Ecrire un programme qui affiche “Hello” si un nombre donné par l‘utilisateur est un multiple de 5, sinon il affiche « Bye »



**Exercice 7:**

Ecrire un programme qui accepte 2 nombres et un opérateur mathématique (+, -, *, /) de la part de l’utilisateur, et exécute l’opération correspondante.


**Exercice 8:**

Ecrire un programme qui accepte l’âge, le genre (« M », « F »), le nombre de jour, et affiche le salaire. Si l’âge ne figure pas dans l’intervalle, alors le programme affiche le message suivant « donner l’ âge approprié »



| age  | Sex | Salaire/Jour |
|:--------:|:--------:|:--------:|
|  >=18 & < 30   |  M   |  700   |
|                |  F  |  750   |
|  >=30 & <=40   |  M   |  800  |
|                |  F  |  850   |



**Exercice 9:**

Ecrire un programme qui accepte 3 nombres et affiche le 2ème grand nombre.


**Exercice 10:**

Ecrire un programme qui accepte les longueurs de trois côtés d'un triangle et vérifie si le triangle est possible ou non



## 2. Premiers exercices avec les structures itératives

**Exercice 11:**

1. Ecrire un programme qui permet d'afficher tous les nombres entre 1 et 10 (bornes incluses).
2. Ecrire un programme se limitant à la boucle *for* qui permet d'afficher tous les nombres pairs entre 1 et 20 (bornes incluses). Proposer une deuxième solution en incluant une structure conditionnelle.


**Exercice 12:**

1. Ecrire un programme qui demande à l'utilisateur de saisir *n* nombres, *n* étant choisi par l'utilisateur, puis d'afficher la moyenne de ces nombres.

2. Même question, mais l'utilisateur ne choisit pas à l'avance le nombre *n*, la procédure s'arrête quand il saisit le nombre -1.



**Exercice 13:**

Ecrire un programme qui permet de calculer le factoriel d'un nombre positif donné par l'utlisateur selon la formule suivante :
n! = 1 x 2 x ... x n.  

1. Une première version en utilisant la boucle *for*
2. Une seconde version en utilisant la boucle *while*



## 3. Pour aller plus loin

**Excercice 14:**

Ecrire un programme qui permet de connaître le jour de naissance de l'utilisateur en posant cinq questions.
Chaque question demande si le jour est dans l'un des cinq ensembles suivants :

* Set 1: \[1 3 5 7 9 11 13 15 17 19 21 23 25 27 29 31\]
* Set 2: \[2 3 6 7 10 11 14 15 18 19 22 23 26 27 30 31\]
* Set 3: \[4 5 6 7 12 13 14 15 20 21 22 23 28 29 30 31\]
* Set 4: \[8 9 10 11 12 13 14 15 24 25 26 27 28 29 30 31\]
* Set 5: \[16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31\]


Le jour de naissance est la somme des premiers nombres dans les ensembles où le jour apparaît. Par exemple,
si le jour de naissance est 19, il apparaît dans Set 1, Set 2 et Set 5. Les premiers chiffres de ces trois ensembles sont 1, 2 et 16. Leur somme est 19.



**Excercice 15:**

Ecrire un programme qui permet de génèrer de manière aléatoire un nombre à deux chiffres, invite l'utilisateur à saisir un nombre à deux chiffres et détermine si l'utilisateur gagne selon les règles suivantes :
* Si l'entrée de l'utilisateur correspond à la loterie (le nombre généré aléatoirement) dans l'ordre exact, la récompense est de 10 000€.
* Sinon, si les deux chiffres entrés par l'utilisateur correspondent aux deux chiffres du numéro de loterie, la récompense est de 3 000€.
* Sinon, si un chiffre dans l'entrée de l'utilisateur correspond à un chiffre dans le numéro de loterie, la récompense est de 1 000€.

**Astuce :** Utiliser la fonction **random.randint(0, 99)** pour génèrer de manière aléatoire un nombre à deux chiffres. Cette fonction doit être accompagné par **import random** comme première instruction dans le code.



**Exercice 16:**

Ecrire un programme qui permet de calculer la somme des chiffres d'un entier *n* donné. Le nombre *n* doit être compris entre 10 et 20 (bornes incluses).



**Exercice 17:**

1. Ecrire un programme qui permet de générer aléatoirement deux nombres entre 0 et 9, de calculer leurs différences (en valeur absolue), puis d'inviter l'utilisateur à répondre à la question suivante *que vaut abs(number1 - number2)?*. Le programme doit permettre à l'utilisateur de répondre plusieurs fois jusqu'à la saisie de la bonne réponse.
2. Modifier le programme précédent de telle sorte qu'il génère cinq occurences à la suite invitant à répondre à la question précédente. A la fin, le programme affiche le nombre moyen de tentatives qu'il a fallu à l'utilisateur pour répondre à une question.



**Exercice 18:**

Ecrire un programme qui permet de calculer le nombre de mots dans une phrase saisie par l'utilisateur.



## 4. Pour s'entraîner

**Exercice 19:**

Soit la variable my_input = "zoophysiology". Ecrire un script qui permet d'afficher l'un des messages suivants en fonction du nombre maximum de *o* consécutifs dans la variable *my_input*. Par exemple, le script doit afficher "I like studying birds! I want to become an ornithologist!" parce qu'il y a deux *o* consécutifs, même s'il y a aussi des *o* individual.
Ignorer les *o* majuscules - recherchez que les *o* minuscules.

* Si "o" apparaît trois fois ou plus de suite, afficher le message "I like going to the zoo!"  
* Si "o" apparaît deux fois, afficher le message "I like studying birds! I want to become an ornithologist!"  
* Si "o" apparaît une seule fois, afficher le message "I like studying fish! I want to become an ichthyologist!"  
* Si "o" n'apparaît pas dans la variable *my_input*, afficher le message "I miss going to the zoo!"  

**Astuce :** Utiliser l'opérateur **in** qui renvoie **True** si la première chaîne se trouve dans la deuxième chaîne.



**Exercice 20:**

Créer quatre variables nommées *team_1* et *team_2*, représentant deux noms d'équipes, et *team_1_score* et *team_2_score*, représentant les scores de ces deux équipes.
Une équipe gagne si son score est supérieur à l'autre score de l'autre équipe.

Ecrire un premier script qui permet d'afficher les messages suivants selon les valeurs entrées, ceci en utilisant seulement les quatres variables créées :
* Si une équipe bat l'autre, affichez: "\[winner\] beat \[loser\] by \[margin\]"
* Si aucune des équipes n'a gagné, affichez: "\[team_1\] played \[team_2\] and it was a tie"

Ecrire un deuxième script qui permet d'afficher les mêmes messages mais en ajoutant trois variables de plus :
* La variable *winner* pour définir l'équipe gagnante  
* La variable *loser* pour définier l'équipe perdante  
* La variable *margin* pour définir la différence entre les deux scores



**Exercice 21:**

L'Indice de Masse Corporelle (IMC) permet d'estimer le poids idéal en fonction de la taille. Son calcul correspond au poids en kilogrammes divisé par le carré de la taille en mètre (IMC = poids en kg/taille² en m). Le chiffre obtenu permet d'estimer la corpulence et éventuellement le surpoids ou l'obésité chez l'adulte, homme ou femme.
L'interprétation de l'IMC pour les personnes de 16 ans et plus est la suivante :
* Moins de 18.5: Underweight
* Entre 18.5 et 24.9: Normal
* Entre 25.0 et 29.9: Overweight
* Plus que 30.0: Obese

Ecrire un programme qui permet de saisir un poids en *pounds* et une taille en *inches*, de calculer et d'afficher l'IMC à deux valeurs après la virgule, et d'afficher l'interprétation la plus adéquate. Notez qu'un *pound* équivaut à 0,45359237 kilogrammes et qu'un *inch* équivaut à 0,0254 mètre.  

**Astuce :** Pour afficher deux valeurs après la virgule, utilisez la fonction **format(nom_variable, ".2f")**. Exemple : **print('La moyenne est :', format(moyenne, ".2f"))**



**Exercice 22:**

Ecrire un programme qui affiche un triangle d'étoiles de taille donnée, par exemple si on entre 6, le programme affiche:
```
*
**
***
****
*****
******
```



**Exercice 23:**

Même exercice mais cette fois la sortie est
```
     *
    **         
   ***
  ****
 *****
******


**Exercice 24:**

Ecrire un programme qui calcule, étant donné un entier *n* rentré par l'utilisateur, la plus grande puissance de *n* inférieure à un million.
