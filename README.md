# GITPassport
Pasaporte de git

### Lista de correos
Correo de los integrantes del pasaporte </br>
[Lista](https://docs.google.com/spreadsheets/d/1w9ELsgnD8ex27fF88WIL0UhM5rGU1ftTxDXpZT4gaBM/edit?usp=sharing)


### Clases
[Clase 1](https://youtu.be/RmA4RKaR6oU)

[Clase 2](https://www.youtube.com/watch?v=eNXxlCBr0yE)


Comandos clave:
</br>

```
git init
```
Para iniciar proyecto git
</br>
```
git status
```
Para mirar los cambios actualues y el stage area 
</br>
```
git add .
```
Para agregar al stage area
</br>
```
git commit -m "Mensaje"
```
Para crear un commit
</br>
```
git log --oneline
```
Para ver el historial
</br>
```
git log --oneline --graph
```
Para ver el historial, pero más gráficamente
</br>

```
git reset .
```
Para deshacer el registro de cambios del stage area
</br>

```
git checkout .
```
Para deshacer los cambios que aún no están en el stage area
</br>

```
git checkout <commitID>
```
Para mirar una versión sin modificar la versión ni el historial
</br>



```
git reset --hard <commitID>
```
Para viajar en el tiempo e ir a este commit específico. Cambia el historial y cambia el código
</br>

```
git reset --soft <commitID>
```
Permite modificar el historial, de modo que este regresa al commit específico, pero el código permanece intacto. Además soft, deja estos cambios ya de una vez agregados al stage area.
</br>

```
git reset <commitID>
```
Permite modificar el historial, de modo que este regresa al commit específico, pero el código permanece intacto. Los cambios quedan registrados, pero aún no se encuetran en el stage area.
</br>

```
git revert <commitID>
```
Permite deshacer el commit seleccionado
</br>
