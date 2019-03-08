# GIT
__Quelques commandes:

- git init
- git config user.name
- git config user.email
- git status
- git add (--all) (-A) [file name]
- git commint (-am "commentaire") (--amend)
- git rm (remove) [file name]
- git show (tag) (id d'un commit)
- git tag [tag name] (-a -m "commentaire') (id_commit) --list nX (X: numéro dans la liste)
- git reset --hard
- git blame
- git diff [file name] id_duCommit id_duCommit2 (ou tag(s)) (ex: git diff dev master <= compare les modification entre la branch dev et master)
- git log --oneline -3
- git help commande (nom de ma commande)
- git checkout
- git branch [branch name to create] (creer une branche)
- git branch -v (verbose)
- git branch (voir les branches)
- git checkout [branch name] (change de branch)  / git checkout -b [branch name to create] (Change et crée une branche)
- git [branch name] -d (--delete) (nécéssite de changer de branch avant de la delete)
- nota bene: Si vous créer un fichier sur la nouvelle branch et switchez sur le master par la suite, le fichier va disparaître de votre fichier en local
// Un git log vous donnera l'historique de l'ensemble des branches
- nota bene 2: Bien commit avant de changer de branch pour ne pas impacter les des deux branches.
- git merge [branch name] (va Merge les fichiers sur la branche actuel s'il n'y a pas de conflit: fusion des fichiers)
![alt text](https://i.ibb.co/LnQ9RVD/Capture2.png)
- git stash (va mettre en remise toute les modifications en cours "Saved working directory and index state WIP on [branch name]", sans commit // Utiliser avec parcimonie)
- git stash list (vérifier le contenu de la remise)
-// Ex: stash@{0}: WIP on dev: 625f875 Add html link
- git stash show stash@{0} (vérifier le contenu de la remise, celui en haut de la liste est le plus récent)
-// contact.html | 1 +
-// 1 file changed, 1 insertion(+)
- git stash apply (Va permettre de récupérer les modification sur la branch ou l'on se trouve, // faire git stash list<= pour vérifier ou se trouve le stash)
- git stash drop (Dropped refs/stash@{0} [commit id] <= va supprimer la remise en haut de la liste)
- git stash clear (Clear l'ensemble des stash)
- git stash pop (va faire apply + drop <= supprime et applique le contenu de la remise du dernier stash)
- git stash pop [select a stash id] (sur un stash spécifique)

__Github

- git remote add origin [Adresse du projet sur github]
- git push origin [branch name] (master)

__Best Practice

- Pour faire un checkout sur un commit précédent il est préférable de créer un branch (ex: git checkout 2fcf -b testOldBranch
Switched to a new branch 'testOldBranch')
- On peut check l'historique des branches ensuite: git log --oneline --all --graph
![alt text](https://i.ibb.co/2k76DWs/Capture.png)
- On commit toujours sur la branche principale (du plus éloigné vers le master)
- Supprimer la branch qui à fait l'objet d'une fusion (merge): git branch [branch name to delete] -d
- Ne pas laisser vivre une branch trop longtemps (risque de conflit)
![alt text](https://i.ibb.co/tpnqH2c/Capture3.png)
- En cas de conflit lors d'une merge: il faudra solutionner le conflit

__Autres commandes utiles hors GIT:

- cd "chemin du fichier"
- .gitignore
