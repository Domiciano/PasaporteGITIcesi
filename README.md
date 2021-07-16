# GITPassport
Pasaporte de git

## Lista de correos
Correo de los integrantes del pasaporte </br>
[Lista](https://docs.google.com/spreadsheets/d/1w9ELsgnD8ex27fF88WIL0UhM5rGU1ftTxDXpZT4gaBM/edit?usp=sharing)

## Solucionarios

[Solucionario Taller 1B](https://youtu.be/Rxi8SLDELXs)<br>
[Solucionario Taller 2B](https://youtu.be/FVzl4HLe_yk)



## Clases 2021-1
[Clase 1](https://youtu.be/RmA4RKaR6oU)

[Clase 2](https://www.youtube.com/watch?v=eNXxlCBr0yE)

[Clase 3](https://youtu.be/zdag9QIMY-0)


## Comandos clave:
</br>

```
git init
```
Para iniciar proyecto git
</br></br>
```
git status
```
Para mirar los cambios actualues y el stage area 
</br></br>
```
git add .
```
Para agregar al stage area
</br></br>
```
git commit -m "Mensaje"
```
Para crear un commit
</br></br>
```
git log --oneline
```
Para ver el historial
</br></br>


```
git log --oneline --graph
```
Para ver el historial, pero más gráficamente
</br></br>

```
git reset .
```
Para deshacer el registro de cambios del stage area
</br></br>

```
git checkout .
```
Para deshacer los cambios que aún no están en el stage area
</br></br>

```
git checkout <commitID>
```
Para mirar una versión sin modificar la versión ni el historial
</br></br>



```
git reset --hard <commitID>
```
Para viajar en el tiempo e ir a este commit específico. Cambia el historial y cambia el código
</br></br>

```
git reset --soft <commitID>
```
Permite modificar el historial, de modo que este regresa al commit específico, pero el código permanece intacto. Además soft, deja estos cambios ya de una vez agregados al stage area.
</br></br>

```
git reset <commitID>
```
Permite modificar el historial, de modo que este regresa al commit específico, pero el código permanece intacto. Los cambios quedan registrados, pero aún no se encuetran en el stage area.
</br></br>

```
git revert <commitID>
```
Permite deshacer el commit seleccionado
</br></br>



### Remotos
```
git remote -v 
```
Permite listar los remotos de nuestro repositorio local
</br></br>


```
git remote add <nombreRemoto> <URLremoto> 
```
Permite agregar un remoto con un nombre específico
</br></br>


```
git remote rm <nombreRemoto> 
```
Permite quitar un remoto
</br></br>


### Operaciones con remotos

```
git push <nombreRemoto> <nombreBranch> 
```
Permite actualizar un remoto con el trabajo hecho en el repositorio local
</br></br>

```
git pull <nombreRemoto> <nombreBranch> 
```
Permite actualizar una rama local usando una rama remota como fuente de actualización. Tener en cuenta que debemos estar parados en una rama local homónima a la que estamos invocando con el comando, porque si no, estamos mezclando las ramas
</br></br>

```
git fetch -p 
```
Permite actualizar las ramas respecto al repositorio remoto
</br></br>

```
git push --delete origin <nombreDeRama> 
```
Permite eliminar la rama nombreDeRama del remoto
</br></br>


### Branches

```
git branch <nombreBranch>
```
Permite crear una nueva rama
</br></br>

```
git checkout -b <nombreBranch>
```
Permite crear una nueva rama y pararse en ella en un sólo comando
</br></br>

```
git branch -a
```
Listar todas las ramas
</br></br>

```
git merge <nombreRama>
```
Permite mezclar la rama nombreRama en la rama en la que estemos parados. Hay 3 posibilidades: fast-fordward, recursive strategy o conflictos. En los dos últimos casos tendremos un commit específico que representa la mezcla.
</br></br>

```
git branch -d
```
Permite eliminar una rama local
</br></br>

```
git branch -D
```
Permite eliminar una rama local a la fuerza
</br></br>


```
git stash
```
Algunas veces no podrá viajar entre branches porque hay cambios NO commiteados. Para evitar crear un commit innecesario use git stash. Es un guardado rápido. Al hacerlo, puede viajar tranquilamente al otro branch.


```
git stash apply
```
Al volver, puede recuperar lo que dejó en el stash usando este comando



### Tags


```
git tag -a <version> <commitID> -m "Mi descripcion del tag"
```
Permite taggear un commit específico
</br>

```
git push origin <version>
```
Permite subir el tag <versión>
</br>


```
git push origin --tags
```
Permite subir todos los tags
</br>


```
git tag
```
Permite listar los tags
</br>


