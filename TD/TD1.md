
#TD1: Prise en main de Python



## 1.Vérification de l'installation de l'environnement de programmation
---------------------------------------------------------------------------------------------------------------------------------------------------

Avant de débuter ce td, vous devez avoir suivi la procédure d'installation [INSTALL.md](https://github.com/uvsq-l1-info100/l1-python/blob/main/INSTALL.md) si vous utilisez votre ordinateur personnel. Si vous rencontrez des problèmes, appelez un enseignant. Sur votre machine, créez un répertoire local, nommé TD, dans lequel vous sauvegardez tout le travail. Dans ce répertoire, créez le sous-répertoire TD1. Il contiendra un fichier hello.py comme sur le site du cours. Toutes les manipulations de cette section sont à effectuer dans Visual Code Studio. Il faut donc lancer VSCode et ouvrir le répertoire local pour les TD. Si vous n'arrivez pas à travailler sur Visual Code Studio, vous pouvez travailler en utilisant un [notebook en ligne](https://colab.research.google.com/notebooks/intro.ipynb). Le notebook en ligne est aussi une solution pour programmer depuis chez vous si vous n'avez pas installé l'environnement correctement. Mais la solution privilégiée reste d'installer l'environnement.

1.  Dans la liste "EXPLORER" à gauche de l'écran, sélectionner le fichier "TD/TD1/hello.py"

2.  Vérifier dans la barre d'état en bas à gauche que l'environnement est bien "Python". Si ce n'est pas le cas, sélectionner l'interpréteur approprié en cliquant en bas à gauche dans la barre d'état ou Ctrl+Shift+P puis sélectionner "Python: Select Interpreter".

3.  Cliquer sur le triangle gris en haut à droite de la fenêtre de l'éditeur Python. Vous devriez voir le message "hello world" s'afficher dans la console.


## 2.Variables
-------------------------------------------------

1.  Affectez le résultat de l'expression `1 + 1` à une variable notée `a`. Affichez maintenant la valeur de la variable `a`. Nous rappelons que vous pouvez utiliser la _fonction native_ `print()`. L'ensemble de ces fonctions est [disponible ici](https://docs.python.org/fr/3.5/library/functions.html).

2.  Augmentez de 1 la valeur de `a`. L'expression doit donner le bon résultat quelle que soit la valeur de la variable. Vérifiez en affichant la valeur de `a`.

3.  Ré-évaluez toutes les cellules où vous avez affiché la valeur de `a`. Que remarquez-vous? On voit ici que ce qui compte dans le notebook est _l'ordre d'évaluation_ et non pas _l'ordre d'apparition_ des cellules. Ce comportement est source d'erreur, il faut donc bien y faire attention.


4.  Sans écrire de code supplémentaire, augmentez encore de 1 la valeur de `a`, et vérifiez que ça a bien fonctionné.


5.  Affectez la valeur 5 à la variable `a` et la valeur 2 à la variable `b`, puis afficher les 2 valeurs avec l'expression `print(a, b)`.


6.  Ecrivez le code qui permet d'échanger la valeur des variables `a` et `b`. Puis affichez leurs valeurs.

7.  Pour enrichir l'affichage, recopiez l'expression `print("a vaut", a, "et b vaut", b)`.

8.  Recopiez l'affectation suivante `a = "hello world"`, puis affichez la valeur de `a` et le type de la variable.

**Note**: la variable `a` contenait un entier, et maintenant une chaîne de caractères. En Python les variables ont un _type dynamique_ contrairement au type statique où le type des variables est défini une fois pour toutes. De plus ce typage est _implicite_, c'est-à-dire qu'il est déterminé par les objets auxquels les variables font référence sans avoir besoin de l'écrire explicitement.

* * *

3.Types de données
-----------------------------------------------

En Python, toute variable ou expression possède un _type_ qui définit, entre autres, les opérations que l'on peut lui appliquer. Parmi les types natifs on peut citer les nombres entiers, les nombres flottants, les chaînes de caractères (string en anglais) et les booléens (Vrai ou Faux).

1.  Prédisez le type de chacune des expressions suivantes. Vérifiez le à l'aide de la fonction `type()`:

*   `5`
*   `5.0`
*   `"5"`
*   `-5`
*   `5 / 2`
*   `5 // 2`
*   `5 == 2`
*   `5 = 2`

Ce sont les types de base du langage Python que nous allons étudier dans la suite. Notez que les nombres flottants s'écrivent avec un point et non avec une virgule.

2.  Faites la même chose avec les expressions suivantes:

*   `(5, 2)`
*   `[5, 2]`
*   `{5, 2}`

Ce sont des types avancés, qui permettent de construire des structures de données plus complexes, que nous apprendrons à manipuler plus tard. Pouvez-vous trouver une expression ayant un autre type? Vous pouvez consulter la [documentation Python sur les types](https://docs.python.org/fr/3/library/stdtypes.html).

3.  Maintenant, affectez une valeur à une variable `x`, et écrivez le code qui affiche, par exemple, `le type de x est <class 'int'>` si jamais la valeur stockée dans `x` est un entier.

### 3.1 Type numérique entier

1.  Affectez une valeur entière à une variable `v`.

2.  Ecrivez le résultat de la division entière de `v` par 11. Par exemple, si `v` vaut 149, le résultat affiché doit être de la forme:

`149 = 13 x 11 + 6`

3.  Prédisez le résultat des expressions suivantes, puis évaluer le code:

*   `3 * (10 / 3)`
*   `3 * (10 // 3)`
*   `(3 * 10) // 3`

5.  Le résultat change-t'il si on retire les parenthèses des expressions précédentes?

6.  Affectez un nombre entier à une variable, puis écrivez une expression qui affiche `True` si la variable est paire et `False` sinon.

7.  L'opérateur puissance s'écrit `**`. Par exemple, 2 à la puissance 10 s'écrit `2 ** 10`. Affichez la valeur de 2 puissance 256. Combien de chiffres a ce nombre (en évitant de compter sur l'écran)?

**Note**: les nombres entiers ont une précision arbitraire.

Ecrire l'expression qui donne le dernier chiffre du nombre référencé par la variable `a`.

Ecrire l'expression qui donne l'avant-dernier chiffre du nombre référencé par la variable `a`.

### 3.2 Nombres flottants

1.  L'expression `0.2 + 0.4` est-elle égale, supérieure ou inférieure à `0.6`?

2.  Affectez la valeur 0.5 à une variable `x`. Multipliez `x` par $2^{30}$ puis convertissez le résultat obtenu en valeur entière (utilisez la fonction `int()`) puis divisez le résultat par $2^{30}$ (faire une division flottante).

3.  Remplacez la valeur de `x` par 0.1 et refaites le calcul.

4.  Pouvez-vous trouver d'autres valeurs de `x` pour lesquelles l'expression calculée redonne la valeur de `x`?

**Note**: les nombres flottants que l'on manipule sont en fait une approximation de ces nombres. Pour plus de détails, vous pouvez consulter [cet article](https://docs.python.org/fr/3.8/tutorial/floatingpoint.html).

### 3.3 Chaînes de caractères

1.  Affectez les variables `a` à "hello" et `b` à 'world'. Affichez le résultat de l'expression `a + b`, et de `b + a`

**Note**: les chaînes de caractères peuvent s'écrire avec des guillemets simples ou doubles (d'autres formes existent). L'opération d'addition de chaînes est appelée _concaténation_.

2.  Affichez à nouveau en ajoutant un espace entre `hello` et `world`, mais sans modifier les variables.

3.  Avant d'afficher le résultat, prédire ce que valent `a * 3` et `(a + b) * 2`?

4.  On peut appliquer des _méthodes_ (ce sont des fonctions qui s'appliquent à un certain type d'objets) à une chaîne de caractères. Par exemple tester ce que vaut `a.upper()`.

Vous pouvez voir la liste des méthodes associées aux chaînes de caractères (ainsi que sur les autres types natifs) sur [cette page](https://docs.python.org/fr/3/library/stdtypes.html#string-methods).

5.  La variable `a` a-t'elle été modifiée?

6.  Que vaut `a > b`? Quelle est la signification de cette comparaison?

### 3.4 Conversions

1.  Affectez `a` à '64'. Devinez ce que vaut `a * 2` avant de l'afficher.

2.  Utilisez la fonction de conversion `int()` pour obtenir le résultat de la multiplication de nombres entiers (64 ici).

3.  Ecrivez l'expression `s = input("Tape quelquechose au clavier")` puis affichez `s`. Que se passe-t'il?

4.  Recopiez le code de la question précédente. Cette fois, l'utilisateur doit saisir un nombre entier puis vous affichez ce nombre multiplié par 2.

5.  ́Ecrivez le code qui demande son âge à l’utilisateur et répond en utilisant sa réponse au milieu d’une phrase, comme par exemple en lui donnant l’âge qu’il aura en 2031 le même jour.

* * *

Exercices supplémentaires
-------------------------------------------------------------

1.  Parmi les chaînes de caractères suivantes, lesquelles peuvent être des noms de variable?

*   `f`
*   `l`
*   `f2`
*   `2f`
*   `totolehero`
*   `toto_le_hero`
*   `import`
*   `toto2-le-retour`

Et parmi les noms corrects, lesquels ne sont pas recommandés (voir la [PEP8](https://www.python.org/dev/peps/pep-0008/#naming-conventions))?

2.  Demandez à l'utilisateur de rentrer un nombre, puis afficher sa racine carrée en faisant une phrase.

3.  Ecrivez le code qui affiche:

*   la chaı̂ne ”aaaaaa...” (250 ”a”)
*   la chaı̂ne ”bbbb....a” (250 ”b” suivis d’un ”a”)
*   la chaı̂ne ”bbbb....aaabbb...” (250 ”b” suivis d’un ”a” suivi de 100 b)
*   50 fois ”bonjour” en allant à la ligne à chaque fois (utilisez ”\\n”)

4.  Evaluez chaque expression numérique étape par étape selon la priorité des opérateurs.
    *   a) 3 + 4 \* 6
    *   b) 3 \* 4 / 6 + 6
    *   c) 2 \* 3 / 12 \* 8 / 4
    *   d) 10 \* ( 1 + 7 \* 3 )
    *   e) 20 - 2 / 6 + 3
    *   f) ( 20 - 2 ) / ( 6 + 3 )
    *   g) 10 + 15 % 2 + 4.3
    *   h) 3 \* 4 / 6 + 6

5.  Saisir, Calculer et Afficher

    *   (1) Ecrire un code qui permet de faire les tâches suivantes :

        *   a) Saisir deux variables, a et b, de type entier.
        *   b) Calculer la somme de ces deux variables.
        *   c) Affecter le résultat dans la variable « Somme ».
        *   d) Calculer le quotient de ces deux variables.
        *   e) Affecter le résultat dans la variable « Quotient ».
        *   f) Afficher les valeurs des variables « Somme » et « Quotient ». Le message doit être sous la forme suivante «La somme de 3 et 1 est 4 et le quotient de 3 sur 1 est 3 »
    *   (2) Quel est le nombre total de variables utilisées pour cet algorithme ?

    *   (3) On veut, maintenant, minimiser le nombre de variables utilisées par le code précédent.

        *   a) Quel est le nombre maximal de variables qu’on peut supprimer ?
        *   b) Quel est le nombre minimal de variables qu’on peut supprimer ?
    *   (4) Ecrire le code correspondant à 3.a.


6.  Ecrire un code qui permet de calculer le diamètre, le périmètre et la surface d’un cercle. Pour ce faire nous allons procéder comme suit :
    *   a) Déclarer la variable constante 𝝅 et la variable Ray contenant la valeur 10.
    *   b) Déclarer trois variables DM, PR et SR.
    *   c) Affecter respectivement à DM, PR et SR les valeurs du diamètre, du périmètre et de la surface d’un cercle dont le rayon est Ray.
    *   d) Afficher le message suivant "Le cercle de rayon AA a pour diamètre BB, pour périmètre CC et pour surface DD".
