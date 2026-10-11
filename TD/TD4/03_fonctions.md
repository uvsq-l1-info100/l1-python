# TD 4: Fonctions en Python


## Instructions Générales

Les deux premiers exercices seont à corriger au tableau, avec le chargé de TD. Pour trouver les réponses, vous n'avez pas le droit d'utiliser une machine. 
Les autres exercices seront réalisés en créant un fichier td3.py, que vous éditerez dans VSCode. Vous respecterez au mieux les règles de bonne pratique en matière d'écriture de code : chaque fonction devra comporter un docstring, des commentaires si nécessaire, et les noms de variables devront être explicites quant à leur usage.

## Revision sur les structures itératives 

Qu'affiche ce programme? 

```python
1. for i in range(5):
            j = i + 1
            i+=j
            print("i et j valent: ", i, j)

2.  for i in range(5):
        for j in range(5):
            for k in range(5):
                print("i+j+k")

```

## Comprendre les fonctions 

Qu'affichent les  programmes suivants? 

```python
1.  def mul2(a):
        return a * 2

    def div2(a):
        return a // 2

    a = 8
    v1 = mul2(a)
    v2 = div2(a)
    print(a, v1, v2)
    a = mul2(a)
    a = div2(a)
     print(a)
  

2.  a = 100
    b = 1000


   def fun1(a):
       a+=1
       return a

   def fun2(a):
       b=3
       a += b
       return a
   
   def fun3(a):
       global b
       a += b
     return a

   fun1(a)
   print("a =", a)
   a = fun2(a)
   print("a et b valent", a, "et", b)
   a = fun3(a)
   print("a =", a)
```

## Gestion du temps

Nous allons créer un petit logiciel de gestion du temps et des dates.
Pour cela nous aurons besoin de créer un certain nombre de fonctions utilitaires.

Un temps a le format suivant: (jour: int, heure: int, minute: int, seconde: int).
C'est un tuple de 4 éléments. Par exemple (4, 3, 13, 20) correspond à 4 jours, 3 heures, 13 minutes et 20 secondes.
Si on a une variable temps = (4, 3, 13, 20), pour accéder au premier élément on fait temps\[0\] ce qui donne 4,
le nombre de jours.

1. Créer la fonction qui prend comme argument le temps et renvoie le nombre de seconde total correspondant à ce temps.
2. Créer la fonction qui prend un nombre de secondes et renvoie le temps correspondant.


```python
#temps[0] : jours, temps[1]: heures, temps[2]: minutes, temps[3]: secondes

def tempsEnSeconde(temps):
    """ Renvoie la valeur en seconde de temps donné comme jour, heure, minute, seconde."""
    pass

temps = (3,23,1,34)
print(type(temps))
print(tempsEnSeconde(temps))   

def secondeEnTemps(seconde):
    """Renvoie le temps (jour, heure, minute, seconde) qui correspond au nombre de seconde passé en argument"""
    pass

temps = secondeEnTemps(100000)
print(temps[0],"jours",temps[1],"heures",temps[2],"minutes",temps[3],"secondes")
```

3. Créer une fonction d'affichage d'un temps `afficheTemps`. Attention, les mots jour, heure et seconde doivent être au pluriel s'il y en a plusieurs. S'il y en a zéro, ils ne doivent pas apparaître.
`print(message, end="")` permet de ne pas sauter une ligne après un print.
Vous pouvez écrire une fonction qui affiche un mot au pluriel ou non, appelée ensuite plusieurs fois par `afficheTemps` pour simplifier votre code.



```python
#fonction auxiliaire ici

def afficheTemps(temps):
    pass

afficheTemps((1,0,14,23))
```

4. Ecrire une fonction qui demande à l'utilisateur de rentrer un nombre de jours, d'heures, de minutes et
de secondes et qui renvoie un temps. Attention, si l'entrée utilisateur n'est pas correcte, par exemple 80 minutes,
afficher un message d'erreur et s'arrêter.

(Optionnel) Au lieu d'arêter le programme, demander de rentrer une nouvelle valeur, tant que
ce n'est pas une valeur correcte.


```python
def demandeTemps():
    pass

afficheTemps(demandeTemps())
```

5. On veut être capable d'additionner deux temps. Donner une fonction qui fait ce calcul,
en utilisant les fonctions précédentes.


```python
def sommeTemps(temps1,temps2):
    pass

sommeTemps((2,3,4,25),(5,22,57,1))
```

6. On veut maintenant calculer un pourcentage d'un temps. Par exemple, 20% de
2 jours et 36 minutes correspond à 9 heures, 43 minutes et 12 secondes.

Implémenter la fonction `proportionTemps` puis appeler cette fonction en échangeant l'ordre des arguments mais en les nommant.


```python
def proportionTemps(temps,proportion):
    pass
afficheTemps(proportionTemps((2,0,36,0),0.2))
#appeler la fonction en échangeant l'ordre des arguments
```


7. On veut maintenant afficher un temps sous forme de date, en supposant
que le temps 0 est le 1 janvier 1970 à 00:00:00.

* Implémenter une fonction `tempsEnDate`qui donne la date sous la forme (année, jour, heure, minute, seconde).
* Implémenter la fonction `afficheDate`qui affiche la date.
* (Optionnel) Gérer également les mois.


```python
def tempsEnDate(temps):
    pass

def afficheDate(date = -1):
    pass

temps = secondeEnTemps(1000000000)
afficheTemps(temps)
afficheDate(tempsEnDate(temps))
afficheDate()
```

8. Il existe des fonctions dans la librairie `time` pour la gestion du temps. En particulier, il existe
une fonction `time` qui donne le temps écoulé depuis 1970 en secondes.
La trouver avec la [documentation python](https://docs.python.org/fr/3/library/time.html#module-time) et la tester en utilisant `afficheDate`.
Tester de la même manière la fonction `time.gmtime` qui réalise une tâche similaire à `tempsEnDate`.
Que constatez vous ?


9. Attention, tous les 4 ans les années sont bisextiles (un jour de plus) sauf les multiples de 100 qui ne sont pas des multiples de 400.
Donner un code qui prend un nombre de jours et affiche toutes les années bisextiles depuis 1 janvier 1970 à 00:00:00 jusqu'à la fin de ces jours.


```python
def bisextile(jour):
    pass

bisextile(20000)
```

Implémenter une fonction `nombreBisextile` qui calcule le nombre d'années bisextiles pour un nombre de jour donnés pour corriger votre fonction de calcul de la date.


```python
def nombreBisextile(jour):
    pass

def tempsEnDateBisextile(temps):
    pass

temps = secondeEnTemps(1000000000)
afficheTemps(temps)
afficheDate(tempsEnDateBisextile(temps))
```

10. Ajouter des valeurs par défaut dans le code de `afficheDate` afin de pouvoir ommettre
l'argument de ces fonctions. Dans ce cas là, on affichera la date actuelle en utilisant la fonction `time`.


11. Donner une fonction qui vérifie la charge horaire d'un employé, donnée sous forme d'une liste de temps travaillé en une semaine. Il ne faut pas dépasser 35h par semaine. 


```python
def verifie(liste_temps):
    pass


liste_temps = [1,4,7,8,0,1,9]
verifie(liste_temps)
```

12. (Pour aller plus loin) S'adapter à une liste qui peut contenir plusieurs semaines. Il ne faut pas dépasser 140h par mois (qu'on considère ici de 4 semaines). Le programme s'arrete dès que la limite par semaine est dépassée et affichera : "Dépassement du nombre d'heures réglémenté par semaine!". Si la limite du nombre d'heures par semaine est atteinte, il affichera : "Dépassement du nombre d'heures réglémenté par mois!". 
 
