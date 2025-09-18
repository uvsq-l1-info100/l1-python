# Environnement de TPs Python pour les L1 UVSQ

## Prérequis
L'utilisation de ce projet avec votre ordinateur personnel suppose que vous avez suivi la procédure d'installation des différents outils.
Cette procédure est détaillée dans le document [INSTALL.md](INSTALL.md).

Si vous utilisez le cartable numérique, vous devez suivre la courte procédure détaillée dans le document [CARTABLE_NUM.md](CARTABLE_NUM.md).

## Utilisation du projet avec [Visual Studio Code](https://code.visualstudio.com/)
Toutes les manipulations de cette section sont à effectuer dans Visual Studio Code.
Il faut donc lancer VSCode et ouvrir le répertoire local du projet.

> ⚠️ **_Utilisation avancée (si vous utilisez _git/github_)_**
> ### Récupérer les mises à jour à partir de `github`
> Il est utile à chaque début de session de travail de rappatrier les éventuelles modifications se trouvant sur votre compte `github`.
> Ce cas peut se produire si vous avez travaillé sur le projet sur une machine et que vous continuiez depuis une autre.
> C'est également nécessaire en travaillant à plusieurs sur un projet.
> 
> 1. Cliquer sur l'icone en forme de graphe à 3 noeuds à gauche de l'écran (*Source Control* ou *Ctrl+Shift+G*)
> 1. Cliquer sur "..." (*Views and more Actions...*) en haut à gauche de *SOURCE CONTROL*
> 1. Sélectionner *Pull, Push* et enfin *Sync*

### Vérifier l'environnement utilisé
1. Dans la liste "EXPLORER" à gauche de l'écran, sélectionner le fichier "examples/hello/hello.py"
1. Vérifier dans la barre d'état en bas à gauche que l'environnement est bien "Python 3.X"
    * si ce n'est pas le cas, sélectionner l'interpréteur approprié en cliquant en bas à gauche dans la barre d'état ou *Ctrl+Shift+P* puis sélectionner "Python: Select Interpreter")
    * ⚠️ **_Utilisation avancée (si vous utilisez un environnement virtuel)_** L'interpréteur à sélectionner est celui de l'environnement _l1-python_ (par exemple "Python 3.9.X XX-bit ('l1-python': conda)")

### Exécuter un programme
* Hello
  1. Dans la liste "EXPLORER" à gauche de l'écran, ouvrir `examples/hello/hello.py`
  1. Cliquer sur le triangle gris en haut à droite de la fenêtre de l'éditeur Python
* explot (test de `matplotlib`)
  1. Dans la liste "EXPLORER" à gauche de l'écran, ouvrir `examples/explot/explot.py`
  1. Cliquer sur le triangle gris en haut à droite de la fenêtre de l'éditeur Python
* Kata _Fizzbuzz_ (avec tests unitaires)
  1. Dans la liste "EXPLORER" à gauche de l'écran, ouvrir `examples/fizzbuzz/test_fizzbuzz.py` ou `examples/fizzbuzz/fizzbuzz.py`
  1. Cliquer sur le triangle gris en haut à droite de la fenêtre de l'éditeur Python
* Interface graphique (test de `tkinter`)
  1. Dans la liste "EXPLORER" à gauche de l'écran, ouvrir `examples/gui/example01.py`, `examples/gui/example02.py` ou `examples/gui/example03.py`
  1. Cliquer sur le triangle gris en haut à droite de la fenêtre de l'éditeur Python
* Notebook Jupyter
  1. Dans la liste "EXPLORER" à gauche de l'écran, ouvrir `examples/exjupyter/exjupyter.ipynb`
  1. En haut à droite de la fenêtre du notebook, cliquer sur "Select Kernel" et choisir "Python 3.9.X XX-bit ('l1-python': conda)" 
  1. Cliquer sur les deux petits triangles (*Run All*) à gauche de la barre d'icones du notebook

### Faire un exercice
1. Dans le répertoire `exercises`, ouvrir le `README.md` de l'exercice à faire (par exemple, [exercises/hello/README.md](exercises/hello/README.md))
1. Ouvrir la prévisualisation du fichier en cliquant en haut à droite de la fenêtre (*Open Preview to the Side* ou *Ctrl+K V*)
1. Répondre aux questions en créant ou en complétant les fichiers de ce répertoire (dans l'exemple, compléter [exercises/hello/hello.py](exercises/hello/hello.py))

### Faire un exercice dans un notebook
Il suffit pour cela d'ouvrir le notebook contenant l'exercice (par exemple [exercises\exjupyter\exjupyter.ipynb](exercises\exjupyter\exjupyter.ipynb)) et de compléter directement le notebook. A la première ouverture d'un notebook, il faut cliquer sur "Select Kernel" en haut à droite de la fenêtre et choisir "Python 3.9.X XX-bit ('l1-python': conda)".

> ⚠️ **_Utilisation avancée (si vous utilisez _git/github_)_**
> ### Sauvegarder les changements sur son compte `github` (via l'interface graphique VSCode)
> Cette procédure vous permettra de conserver vos modifications entre les séances en les sauvegardant sur `github`.
> 
> 1. Cliquer sur l'icone en forme de graphe à 3 noeuds à gauche de l'écran (*Source Control* ou *Ctrl+Shift+G*)
>     * La liste des fichiers modifiés (*M* en fin de ligne) ou ajoutés (*U* en fin de ligne) s'affiche
> 1. Cliquer sur le *+* (*Stage Changes*) en fin de ligne pour chaque fichier *modifiés ou ajoutés* à sauvegarder sur `github`
> 1. Taper un message de *commit* pour indiquer ce qui a changé (par exemple "Termine l'exercice 2") dans la zone de texte à gauche juste au dessus de *Staged Changes*
> 1. Cliquer sur l'icone "✔" (*Commit*) en haut à gauche à côté de *SOURCE CONTROL*
> 1. Envoyer les *commits* vers `github`
>     1. cliquer sur "..." (*Views and more Actions...*) en haut à gauche de *SOURCE CONTROL*
>     1. sélectionner *Pull, Push* et enfin *Sync*
>     1. vérifier que les changements ont bien été pris en compte sur votre compte github

### Remarque
* Pour ouvrir un *REPL Python* dans l'environnement courant, il faut ouvrir la *Command Palette* (`Ctrl+Shift+P`), puis taper *Python: Start REPL*.

## Utilisation du projet dans un terminal
Pour cette section, il faut ouvrir un terminal dans le répertoire du projet.

### Récupérer les mises à jour à partir de `github`
Taper dans le terminal :
```bash
git pull origin master
```

> ⚠️ **_Utilisation avancée (si vous utilisez _git/github_)_**
> #### Intégrer les mises à jour du projet original
> Cette étape n'est pas à effectuer à chaque fois mais quand un enseignant vous le demande.
> Elle va permettre de mettre à jour votre copie locale du projet à partir du dépôt `github` original.
> 
> 1. Créer un lien nommée `upstream` vers le dépôt d'origine
>     ```bash
>     git remote add upstream https://github.com/uvsq-info/l1-python
>     ```
> 1. Récupérer les modifications de ce dépôt
>     ```bash
>     git fetch upstream
>     ```
> 1. Se placer localement sur la *branche principale*
>     ```bash
>     git checkout master
>     ```
> 1. Intégrer la branche principale de `upstream` à la branche locale
>     ```bash
>     git merge -Xtheirs upstream/master
>     ```
> 1. Envoyer les modifications vers votre dépôt `github`
>     ```bash
>     git push -f origin master
>     ```

> ⚠️ **_Utilisation avancée (si vous utilisez un environnement virtuel)_**
> ### Activation de l'environnement
> Il est nécessaire d'activer l'environnement du projet pour avoir accès à la version adéquat de Python ainsi qu'à toutes les bibliothèques.
> 
> ```bash
> conda activate l1-python
> ```

### Exécuter un programme
* Hello
  ```bash
  python examples/hello/hello.py
  ```
* explot (test de `matplotlib`)
  ```bash
  python examples/explot/explot.py
  ```
* Kata _Fizzbuzz_ (avec tests unitaires)
  ```bash
  python examples/fizzbuzz/test_fizzbuzz.py
  python examples/fizzbuzz/fizzbuzz.py
  ```
* Interface graphique (test de `tkinter`)
  ```bash
  python examples/gui/example01.py # dessiner dans la fenêtre
  python examples/gui/example02.py # dessiner dans la fenêtre
  python examples/gui/example03.py
  ```

### Validez un programme
Certains outils assistent le développeur dans l'écriture de programmes.
Ces outils forment la catégorie des *linters*.
Il en existe plusieurs pour la plupart des langages de programmation.
Il est bien entendu fortement recommandé d'utiliser ces outils pour vérifier ses programmes.

Deux d'entre eux sont disponibles dans cet environnement :
* [flake8](https://flake8.pycqa.org/en/latest/) qui valide en particulier le respect du style de codage [PEP 8](https://www.python.org/dev/peps/pep-0008/)
* [mypy](http://mypy-lang.org/) qui valide statiquement les types utilisés

Pour les exécuter sur un fichier Python :
```bash
flake8 examples/fizzbuzz/fizzbuzz.py
mypy examples/fizzbuzz/fizzbuzz.py
```

> ⚠️ **_Utilisation avancée (si vous utilisez _git/github_)_**
> ### Sauvegarder les changements sur son compte `github` (via le terminal)
> Cette procédure vous permettra de conserver vos modifications entre les séances en les sauvegardant sur `github`.
> 
> 1. Afficher la liste des fichiers modifiés ou ajoutés
>     ```bash
>     git status
>     ```
> 1. Marquer chaque fichier *modifiés ou ajoutés* comme à sauvegarder sur `github`
>     ```bash
>     git add hello.py # à faire pour chaque fichier à sauver
>     ```
> 1. Valider les changements à sauvegarder en créant un nouveau *commit* avec un message d'explication
>     ```bash
>     git commit -m "Termine l'exercice 2"
>     ```
> 1. Récupérer les éventuelles mises à jour puis envoyer les *commits* vers `github`
>     ```bash
>     git pull origin master # mises à jour en provenance de github
>     git push -u origin master # sauvegarde des modifications locales
>     ```

## Références
### Python
* [Site officiel](https://www.python.org/)
* [Documentation](https://docs.python.org/fr/3/) en français
* [Carte de référence](https://perso.limsi.fr/pointal/python:abrege), ensemble de [liens](https://perso.limsi.fr/pointal/liens:python_links), L. Pointal
* [Cours de Python](https://python.sdv.univ-paris-diderot.fr/), Patrick Fuchs et Pierre Poulain

### Git
* [Site officiel](https://git-scm.com/)
* [Documentation](https://git-scm.com/doc)
* Carte de référence (en français) ([web](https://training.github.com/downloads/fr/github-git-cheat-sheet/), [pdf](https://training.github.com/downloads/fr/github-git-cheat-sheet.pdf))
* Le livre [Pro Git](https://git-scm.com/book/fr/v2) (*Scott Chacon et Ben Straub, Apress*) en français

### Visual Studio Code
* [Site officiel](https://code.visualstudio.com/)
* [Documentation](https://code.visualstudio.com/docs) (en anglais)
* [Python in Visual Studio Code](https://code.visualstudio.com/docs/languages/python)
* Extension [Microsoft Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) ([tutoriel](https://code.visualstudio.com/docs/python/python-tutorial))
