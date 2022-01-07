## Algunos comandos en github
1. Para crear una rama, se debe estar ubicado en main
```
git checkout -b nombre_rama
```
2. Para navegar entre ramas
```
git checkout nombre_rama
```
3. Para conocer todas las ramas
```
git branch
```
4. Para borrar una rama, debo hacerlo desde el main
```
git branch -D nombre_rama
```
5. Para sincronizar la rama que no está en local, pero si está en el servidor remoto (github).
```
git fetch
```
Luego se escribe:
```
git checkout nombre_rama_arriba_en_servidor
```
6. Para hacer rebase, se ubica uno en la rama original, ejemplo: suponga que está en la rama model_poll; en consola escriba
```
git rebase master
```
Luego
```
git push origin model_poll:model_poll -f
```
Después se ubica en el master y hace
```
git pull origin master
```
7. Para saber el status, asuntos pendientes para adicionar o hacer commit
```
git status
```
8. Para agregar los cambios en una rama
```
git add .
```
9. Para hacer commit
```
git commit -m "Acá se coloca información del commit" 
```
10. Para actualizar una rama con el master, Me ubico en la rama que quiero actualizar
```
git rebase master
```
A veces se requiere forzar el rebase, entonces, una vez seguro de ello
```
git rebase master -f
```
11. 