# OpenclassroomsProject
Faire des tests d'apprentissage


# D'abord se positioner sur son répertoire de travail
mkdir premierProjet
cd premierProjet

git config --global user.name "SaisirMonNom"
git config --global user.email "SaisirMonAdresseEmail"

# Configuer les couleurs par défaut
git config --global color.diff auto
git config --global color.status auto
git config --global color.branch auto

# Configuer l'éditeur de text 
git config --global core.editor vim

# Configuer l'éditeur de text 
git config --global merge.tool vimdiff


# Unitialiser le dépot, ce qui création un dossier local .git
git init
# ou
git config --global init.defaultBranch main

# Création de nouveau fichier 
touch index.html 

# Indexer un nouveau fichier
git add index.html

# Voir le status du dépôt local pour savoir s'il y a des modifications en attente d'indexer
git status

git commit -m "Ajout du fichier index.html"


# Création de nouveau fichier 
touch styles.css 

# Indexer les modifications ou ajout de nouveaux fichier
git add index.html styles.css


# Passer les données d'index en repositorie local
git commit -m "Ajout des fichiers html et css de base"


# Voir le status du dépôt local pour savoir s'il y a des modifications en attente d'indexer
git status


# Rélier ledépot local au depot distance
git remote add origin https://github.com/MikeAbdoul/OpenclassroomsProject.git


git branch -M main
 
git push -u origin main
