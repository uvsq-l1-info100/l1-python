# Guide d'installation de l'environnement de TPs Python

## Installer Python
Python est un langage de programmation *interprété*.
Pour exécuter un programme écrit dans ce langage, il faut disposer d'un *interpréteur Python* ainsi que de certaines bibliothèques installées sur la machine.

Nous utiliserons la version 3 de Python.
En 2025, la [version 3.13](https://docs.python.org/fr/3.13/whatsnew/3.13.html) est la plus récente disponible sur la plupart des architectures de machine.

Pour simplifier l'installation des outils nécessaires, nous allons utiliser une *distribution Python*.
Cette dernière regroupe des outils (interpréteur Python, gestionnaire de paquets, …) et des bibliothèques (numpy, …).
Il en existe plusieurs mais nous nous appuyerons sur la distribution [Miniconda](https://docs.conda.io/en/latest/miniconda.html) qui est une version allégée de la distribution [Anaconda](https://www.anaconda.com/products/individual).

### Installer la distribution **Miniconda**
1. Télécharger la version de [Miniconda](https://docs.conda.io/en/latest/miniconda.html) pour **Python 3.X** et **adaptée à votre système**. La plupart des machines ont des processeurs de 64-bits.
    * pour Windows, télécharger [Miniconda3 Windows 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe)
    * pour Mac OS, télécharger [Miniconda3 MacOSX 64-bit pkg](https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.pkg)
    * pour Linux, télécharger [Miniconda3 Linux 64-bit](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh)
1. Installer Miniconda
    * pour Windows, double-cliquer sur le fichier `.exe` téléchargé précédemment puis suivez la procédure suivante :
      - accepter la licence ("I Agree")
      - "Install for", "Just Me (recommended)" ("Next")
      - "Choose Install Location", Si votre nom d'utilisateur Windows contient des accents (par exemple C:\Users\Théo) **choisissez un autre répertoire d'installation** (par exemple C:\Users\Public), ("Next")
      - "Register Miniconda3 as my default Python 3.X", ("Install")
      - "Installation Complete", ("Next")
      - "Completing Miniconda3...", **décocher tout** ("Finish")
    * pour Mac OS, double-cliquer sur le fichier `.pkg` téléchargé précédemment puis accepter les choix par défaut
    <!-- TODO : détailler la procédure pour Mac OS -->
    * pour Linux, ouvrir un terminal dans le répertoire où se trouve le fichier téléchargé et taper :
        ```bash
        sh Miniconda3-latest-Linux-x86_64.sh
        ```
        À l'affichage de :
        ```
        Welcome to Miniconda3 py39_4.10.3

        In order to continue the installation process, please review the license
        agreement.
        Please, press ENTER to continue
        >>>
        ```
        Appuyer sur la touche ENTRÉE, puis la licence du logiciel va s'afficher :
        ```
        [...]
        Do you accept the license terms? [yes|no]
        [no] >>> yes
        ```
        Taper *yes*, puis à la question :
        ```
        Miniconda3 will now be installed into this location:
        /home/user/miniconda3

        - Press ENTER to confirm the location
        - Press CTRL-C to abort the installation
        - Or specify a different location below

        [/home/user/miniconda3] >>>
        ```
        Accepter le choix par défaut, enfin, répondre *yes* à
        ```
        Do you wish the installer to initialize Miniconda3
        by running conda init? [yes|no]
        [no] >>> yes
        ```
        Fermer ensuite votre terminal.

1. Tester l'installation
    * sous Windows, ouvrir un *Anaconda Prompt*; sous Mac OS ou Linux, ouvrir un terminal et taper :
        ```bash
        conda list
        ```
        doit afficher une liste de bibliothèques :
        ```bash
        # packages in environment at /home/user/miniconda3:
        #
        # Name                    Version                   Build  Channel
        brotlipy                  0.7.0           py39h2bbff1b_1003
        ca-certificates           2021.7.5             haa95532_1
        certifi                   2021.5.30        py39haa95532_0
        cffi                      1.14.6           py39h2bbff1b_0
        chardet                   4.0.0           py39haa95532_1003
        conda                     4.10.3           py39haa95532_0
        conda-package-handling    1.7.3            py39h8cc25b3_1
        console_shortcut          0.1.1                         4
        cryptography              3.4.7            py39h71e12ea_0
        idna                      2.10               pyhd3eb1b0_0
        [...]
        ```
        Pour vérifier la version de Python, taper :
        ```bash
        python -V
        ```
        qui doit afficher (*les derniers nombres peuvent varier*) :
        ```
        Python 3.13.7
        ```

Plus d'informations (en anglais) peuvent être trouvées sur le site officiel de Miniconda ([Installation pour Windows](https://conda.io/projects/conda/en/latest/user-guide/install/windows.html), [installation pour Max OS](https://conda.io/projects/conda/en/latest/user-guide/install/macos.html), [installation pour Linux](https://conda.io/projects/conda/en/latest/user-guide/install/linux.html)).

## Installer un éditeur de texte
De nombreuses applications peuvent être utilisées pour saisir un document textuel sur un ordinateur ([LibreOffice Writer](https://www.libreoffice.org/discover/writer/), [Notepad++](https://notepad-plus-plus.org/), ...).
Dans le contexte de la programmation, il est important que le texte du programme ne soit pas modifié par des informations de mise en forme comme le ferait un logiciel de *traitement de texte* comme LibreOffice Writer.

Il faut donc choisir un logiciel dans la catégorie des [éditeurs de texte](https://fr.wikipedia.org/wiki/%C3%89diteur_de_texte) ou des [environnement de développement intégré](https://fr.wikipedia.org/wiki/Environnement_de_d%C3%A9veloppement) (*integrated development environment* ou *IDE* en anglais).
Les différents outils de ce type varient beaucoup en terme de fonctionnalités et de complexité d'usage.

Nous avons choisi le logiciel [Visual Studio Code](https://code.visualstudio.com/).
Il est un bon compromis entre fonctionnalités et complexité tout en étant disponible pour les principales architectures et systèmes d'exploitation.

### Installer Visual Studio Code
1. Télécharger la version de [Visual Studio Code](https://code.visualstudio.com/) adaptée à votre système
1. Lancer l'installation du programme à partir du fichier téléchargé ([pour Windows](https://code.visualstudio.com/docs/setup/windows), [pour Mac OS](https://code.visualstudio.com/docs/setup/mac), [pour Linux](https://code.visualstudio.com/docs/setup/linux))

Nous ne détaillons pas ici la procédure d'installation car elle ne présente pas de difficulté majeure.

> ⚠️ **_Installation avancée (optionelle)_** Si vous souhaitez utiliser _git/github_, suivez les étapes d'installation se trouvant dans [INSTALL_ADV.md](INSTALL_ADV.md#install_git).

## Récupérer le projet localement
1. Télécharger, avec votre navigateur, une archive du l'environnement de TD à partir de https://github.com/uvsq-info/l1-python.
    * pour cela, cliquer sur le bouton vert _<> Code_ et sélectionner _Download ZIP_
1. Décompresser l'archive dans le répertoire de votre choix.
1. Ouvrir ensuite dans VSCode le répertoire créé ci-dessus

## Finaliser l'installation de Visual Studio Code
### Choisir le *shell* de commande par défaut
Cette étape précise à VSCode quel *shell* utiliser pour le terminal.

1. Appuyer sur *Ctrl+Shift+P* pour ouvrir la palette de commandes
1. Taper "Terminal: Select Default Profile"
1. Sélectionner
    * "Command Prompt" sous Windows
    * "bash" sous Mac OS ou Linux

> ⚠️ **_Installation avancée (optionelle)_** Si vous souhaitez isoler l'environnement Python avec un environnement virtuel, suivez les étapes d'installation se trouvant dans [INSTALL_ADV.md](INSTALL_ADV.md#install_virt).

### Finaliser l'installation de VSCode
1. Dans la liste "EXPLORER" à gauche de l'écran, sélectionner le fichier "examples/hello/hello.py"
    * accepter l'installation de l'extension [Microsoft Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
1. Sélectionner l'interpréteur Python 3.X
    * cliquer en bas à gauche dans la barre d'état ou *Ctrl+Shift+P* puis sélectionner "Python: Select Interpreter"
    * si vous avez créé un environnement virtuel, le sélectionner (par exemple l1-python "Python 3.9.X XX-bit ('l1-python': conda)")
1. Activer les outils de vérification statique (*Linters*)
    1. Ouvrir la palette de commande (*Ctrl+Shift+P*)
    1. Sélectionner la commande "Python: Select Linter"
    1. Choisir `flake8` dans la liste

## Utiliser le projet
Pour utiliser le projet, consulter le [README.md](README.md) du projet.

## Dépannage des problèmes d'installation
### Le *shell* est `zsh`
Les MacOS récents (depuis Catalina en 2019) n'utilisent plus le shell `bash` mais `zsh`. Cela pose des soucis lors de l'installation de miniconda.
Une solution est décrite dans [Installing miniconda with zsh](https://stackoverflow.com/questions/50336405/installing-miniconda-with-zsh) :
1. Modifier la variable d'environnement `PATH` dans le `~/.zshrc` :
    ```bash
    export PATH="~/miniconda3/bin:$PATH"
    ```
1. Ouvrir un terminal et taper :
    ```bash
    cd ~/miniconda3/bin && conda update conda
    conda init zsh
    ```

### Guide pour les anciennes versions du cartable numérique
Le guide d'utilisation est se trouve dans [CARTABLE_NUM.md](CARTABLE_NUM.md).
