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

__Autres commandes utiles hors GIT:

- cd "chemin du fichier"
- .gitignore
