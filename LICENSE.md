GPL V2

#Comandos mas usados
$ git commit --amend --no-edit # Dejamos el mismo mensaje
$ git commit --amend -m "Nuevo mensaje para el cambio"
$ git checkout -- README.md -//> 
$ git add --all -//> to staged files,prepare files
$ git reset HEAD README.md -//>  unstage the file after add
$ git checkout -b primera-rama
$ git checkout master -//> cambiarme de rama
$ git checkout Capitulo-X -//>tag
$ git merge segunda-rama -//> make sure you where are you . git checkout master
$ git branch -d segunda-rama -//> ELIMINAR RAMA or -D
$ git branch -v -//> lista todas las branch existentes
$ git push origin duplicada-de-arreglos-varios:arreglos-varios -//> rare
$ git log -//> listar commits author y fecha
$ git log -p -1 -//> listar lineas de codigo
$ git remote -v -//> listar los repos
$ git checkout --track origin/arreglos-varios -//> seguir una rama diferente a master
$ git push origin :arreglos-varios -//> eliminar una rama
$ git remote add servidor-de-pruebas https://github.com/albertogg/tutorial-git.git -//> añadir un repo
$ git push origin master -//> [repo] [rama]
$ git push origin master --tags -//> subir tags
$ git tag -//> listar versiones
$ git tag [name] -//> crear tag

#Seguir
http://codehero.co/git-desde-cero-manejo-de-ramas-remotas/   -> 7
