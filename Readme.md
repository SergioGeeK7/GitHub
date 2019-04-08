#Comandos mas usados

$ git reset --hard -//> before checkout use this to ignore changes
$ git commit --amend --no-edit # Dejamos el mismo mensaje <br />
$ git commit --amend -m "Nuevo mensaje para el cambio" <br />
$ git checkout -- README.md -//>  <br />
$ git add --all -//> to staged files,prepare files <br />
$ git reset HEAD README.md -//>  unstage the file after add <br />
$ git checkout -b primera-rama <br />
$ git checkout master -//> cambiarme de rama <br />
$ git checkout Capitulo-X -//>tag <br />
$ git merge segunda-rama -//> make sure you where are you . git checkout master <br />
$ git branch -//> list branchs
$ git branch --r -//> list remote brenchs
$ git branch -d segunda-rama -//> ELIMINAR RAMA or -D <br />
$ git checkout --track origin/serverfix
$ git checkout -b sf origin/serverfix -//>rama local sf va a llevar (push) y traer (pull) hacia o desde origin/serverfix.
$ git branch -v -//> lista todas las branch existentes <br />
$ git push origin duplicada-de-arreglos-varios:arreglos-varios -//> rare <br />
$ git log -//> listar commits author y fecha <br />
$ git log -p -1 -//> listar lineas de codigo <br />
$ git remote -v -//> listar los repos <br />
$ git checkout --track origin/arreglos-varios -//> seguir una rama diferente a master <br />
$ git push origin :arreglos-varios -//> eliminar una rama <br />
$ git remote add servidor-de-pruebas https://github.com/albertogg/tutorial-git.git -//> añadir un repo <br />
$ git push origin master -//> [repo] [rama] <br />
$ git push origin master --tags -//> subir tags <br />
$ git tag -//> listar versiones <br />
$ git tag [name] -//> crear tag <br />
$git commit -m "Mensaje corregido" --amend  --//> you forgot to add a modification to a file <br />
$git remote -v  <br />
$git reset HEAD jedi.js  <br />
$git checkout HEAD jedi.js <br />
$git reset --//> hard <br />
$git stash --//> save <br />
$git stash apply -->rest <br />
$git diff 0da94be 59ff30c <br />
$git stash -> save without commit <br>
$git stach pop -> restore <br>
$git reset --soft HEAD^1 -> leave the changes made <br>
$git reset HEAD file -> detach add <br>
$git clean -f -d -n -> remove untracked files after git checkout HEAD  <br>
$git pull -s recursive -X theirs <remoterepo or other repo>  <br> 
$git fetch && git rebase <remote>/branch && git rebase --continue  <br>
$git push -d origin <branch_name>  <br>
$git branch -d <branch_name>  <br>
$git reset filename.txt  <br> /undo add
$git reset --soft // after you've shited allows you to go back one commit and re-commit <br> 
$git reset --hard // [SHA 1]: goes back to a commit [SHA 1] and deletes files from working directory and staging <br>
$git diff version1 version2 <br>
$git log --oneline <br>
#### Merge feature branch to master
git checkout master
 
git pull --rebase origin master

git checkout feature1

git rebase master

fix any conflicts

git checkout master

git rebase feature1 // will rebase with no conflicts since you fixed them previously.

----- undo your commit 
git reset HEAD~2        # undo last two commits, keep changes
git reset --hard HEAD~2 # undo last two commits, discard changes  

git commit --amend                  # start $EDITOR to edit the message
git commit --amend -m "New message" # set the new message directly
#or
git add forgotten_file 
git commit --amend

git rebase --interactive origin branch # edit lots of commits name, change `pick` for `reword` or `r`
 git revert c761f5c              # reverts the commit with the specified id
 git revert HEAD^                # reverts the second to last commit
 git revert develop~4..develop~2 # reverts a whole range of commits
 
 man githooks
 https://help.github.com/articles/remove-sensitive-data/
 git config --global rerere.enabled true

git reset --soft HEAD~1 // keep changes in index
git cherry-pick <commit-hash> // merge just one commit, not branch
 
 
 remove sensitive data
 `git filter-branch --force --index-filter \
  'git rm --cached --ignore-unmatch secrets.txt' \
  --prune-empty --tag-name-filter cat -- --all`
 -----
 
 git reset filename          # or
 echo filename >> .gitingore # add it to .gitignore to avoid re-adding it
 
The working tree/working directory/workspace is the directory tree of (source) files that you see and edit.
The index/staging area is a single, large, binary file in /.git/index, which lists all files in the current branch, their sha1 checksums, time stamps and the file name - it is not another directory with a copy of files in it.
HEAD is a reference to the last commit in the currently checked-out branch.

 
 <br>
$editor path/to/file
$git-add path/to/file
$git-commit -v --amend
 <br />

git diff -r d930b7b44339b003931e1eae5adaad6dccd754ab
<br/>
git reset --hard c86e238f8ae199be2a26588067d86deacae4d1c1

 <br />
$ http://codehero.co/git-desde-cero-manejo-de-ramas-remotas/  ->  7
<br/>
--------
git rebase -I commitNumber .....

### merge one commit 

git checkout master

git merge --squash branchName

git commit

git reset --hard commitNumber --> **return to a specific commit**

git revert commitNumber


HEAD -- means where you're pointing
