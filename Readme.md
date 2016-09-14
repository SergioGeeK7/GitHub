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
$git clean -f -d -n -> remove untracked files after git checkout HEAD


$editor path/to/file
$git-add path/to/file
$git-commit -v --amend



 <br />
$ http://codehero.co/git-desde-cero-manejo-de-ramas-remotas/  ->  7
