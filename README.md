# GIT
__Quelques commandes:

- git init
- git config user.name
- git config user.email
- git status
- git add (--all) (-A) nomFichier
- git commint (-am "commentaire") (--amend)
- git rm (remove) nomDuFichier
- git show (tag) (id d'un commit)
- git tag (nomDuTag) (-a -m "commentaire') (id_commit) --list nX (X: numéro dans la liste)
- git reset --hard
- git blame
- git diff (nomDuFichier) id_duCommit id_duCommit2 (ou tag(s))
- git log --oneline -3
- git help commande (nom de ma commande)
- git checkout
- git branch nomDeLaBranchACreer (creer une branche)
- git branch -v (verbose)
- git branch (voir les branches)
- git checkout nomDeLaBranch (change de branch)  / git checkout -b nomDeLaNouvelleBranch (Change et crée une branche)
- git nomDeLaBranch -d (--delete) (nécéssite de changer de branch avant de la delete)
- nota bene: Si vous créer un fichier sur la nouvelle branch et switchez sur le master par la suite, le fichier va disparaître de votre fichier en local
// Un git log vous donnera l'historique de l'ensemble des branches
- nota bene 2: Bien commit avant de changer de branch pour ne pas impacter les des deux branches.
- git merge nomDeLaBranch (va Merge les fichiers sur la branche actuel s'il n'y a pas de conflit: fusion des fichiers)
- Visuel: ![alt text](https://i.ibb.co/LnQ9RVD/Capture2.png)

__Best Practice

- Pour faire un checkout sur un commit précédent il est préférable de créer un branch (ex: git checkout 2fcf -b testOldBranch
Switched to a new branch 'testOldBranch')
- On peut check l'historique des branches ensuite: git log --oneline --all --graph
![alt text](https://i.ibb.co/2k76DWs/Capture.png)
- On commit toujours sur la branche principale (du plus éloigné vers le master)
- Supprimer la branch qui à fait l'objet d'une fusion (merge): git branch nomBranchADelete -d
- Ne pas laisser vivre une branch trop longtemps (risque de conflit)
- visuel: ![alt text](https://i.ibb.co/tpnqH2c/Capture3.png)

__Autres commandes utiles hors GIT:

- cd "chemin du fichier"
- .gitignore
