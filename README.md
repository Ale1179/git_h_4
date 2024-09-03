# HACK - GIT 4

##### ### ## EXTRAER ARCHIVO DEL STAGE.

Crear un nuevo repositorio en github nombre: git_h_4

Crear un repositorio local

-git init
-Registrar el repositorio remoto con tú repositorio local
-git remote add origin (pegar_la_ruta_del_repositorio_local)
-Verificamos la ruta remota
-git remote -v
-Crear 3 archivos foo.txt | bar.txt | qux.txt
-touch foo.txt
-touch bar.txt
-touch qux.txt
-Comprobar que estan creados en nuestro local
-ls -l
-Toca ver el stage
-git status
-Anexamos los 3 archivos al stage
-git add .
-Examinamos el stage
-git status
-10 Ahora toca extraer a "qux.txt" del stage y dejar los otros 2 archivos

-git reset -- qux.txt

11. Indagamos que "qux.txt" no esta en el stage

-git status

12. Resulta que ahora no queremos ninguno de los 2 archivos restante en el stage
-git reset --

13. Volvemos a observar el status del stage
-git status

14. Adjuntamos un cuarto archivo llamado "octocat.txt" 
-touch octocat

15. Cuando se revisa de nuevo el stage debemos mirar los 4 archivos, que no estan seleccionados
-git status

16. Los adjuntamos al stage para genrar el commit
-git add . git status git commit -m "feat: add 4 files"

17. Resulta que se nos olvido agregar un 5 archivo llamado "delta.txt"
-touch delta.txt

18. Bien, debemos agregar el archivo "delta.txt" al commit que se acaba de crear, esto lo podemos verificar 
-git log --oneline

19. Agregamos el archivo al commit
git add delta.txt git commit --amend -m "feat: add 5 files"

20. Listo ahora se analiza el commit de vuelta y se hace push 
```diff
git log --oneline
git push -u origin master
Observar el repositorio remoto


##  FIN.



