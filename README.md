Projet SGU — Système de Gestion des Urgences
============================================

Collaboration sur la branche "dev"
----------------------------------

Ce projet est développé en équipe dans le cadre du module de CPP.  
Toutes les contributions doivent être faites sur la branche `dev`.  
La branche `main` est réservée à la version stable finale du projet.

1. Clonage du projet
--------------------

Fork le projet sur Github (fork main et dev)

Ouvrez un terminal et entrez :

    git clone https://github.com/[votre nom user]/Projet_SGU.git
    cd Projet_SGU

2. Travailler sur la branche "dev"
----------------------------------

Avant toute modification, assurez-vous d'être sur la bonne branche :

    git checkout dev
    git pull origin dev

3. Ajouter ou modifier du code
------------------------------

Vous pouvez créer un nouveau fichier ou modifier ceux déjà présents.

    touch src/mon_module.cpp
    echo "// début du code" > src/mon_module.cpp     # pas forcément nécessaire

4. Ajouter et valider les changements
-------------------------------------

    git add .
    git commit -m "Ajout du module mon_module"

5. Pousser sur la branche "dev"
-------------------------------

    git push origin dev

6. Mettre à jour votre dépôt local
----------------------------------

Avant chaque nouvelle session de travail, pensez à récupérer les dernières modifications :

    git checkout dev
    git pull origin dev          #Pour actualiser votre projet par rapport au github du groupe

Utilisation avec Visual Studio Code (VScode / VSCodium)
--------------------------------------------------------

Nous recommandons l’usage de Visual Studio Code ou VSCodium pour le développement.

### Ouvrir le projet

Dans un terminal :

    code Projet_SGU/
    # ou si vous êtes déjà dans le dossier
    code .

Si la commande `code` ne fonctionne pas :
- Ouvrez VScode
- `Ctrl+Shift+P` → `Shell Command: Install 'code' command in PATH`

### Créer / modifier un fichier

- Dans l'explorateur (barre de gauche), clic droit sur `src/` → *Nouveau fichier*.
- Donnez un nom comme `mon_module.cpp`, puis commencez à coder.
- Sauvegardez avec `Ctrl+S`.

### Terminal intégré

Utilisez le terminal intégré de VScode (`Ctrl+``) pour exécuter toutes les commandes Git :

    git checkout dev
    git pull origin dev
    git add .
    git commit -m "Ajout/modif"
    git push origin dev

### Extensions recommandées

- **C/C++** (Microsoft)
- **GitLens**
- **Doxygen Documentation Generator**
- **CMake Tools** (si vous utilisez CMake)

Règles importantes
------------------

- Ne poussez **rien** directement sur la branche `main`.
- Travaillez **exclusivement sur `dev`**.
- Communiquez avec le groupe si vous faites de grosses modifications.
- Utilisez des messages de commit clairs et précis.

Organisation du dépôt
---------------------

    Projet_SGU/
    ├── src/         -> code source principal
    ├── include/     -> fichiers d’en-tête (.h)
    ├── test/        -> tests unitaires
    ├── docs/        -> documentation Doxygen
    ├── data/        -> données éventuelles
    ├── build/       -> répertoire de compilation
    ├── README.md    -> ce fichier
    └── .gitignore   -> fichiers ignorés par Git

Auteurs
-------

- Ankoudy Yassir  
- Cheikh Tourad Wedou  
- Duquesnoy Samuel  
- Guissou Dakisaglogo  

Bon code à tous 🚀
