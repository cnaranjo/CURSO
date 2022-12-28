# Clase 5

## Tipos de Merge

*Fast-Forward (sin conflicto y no agrega commit)
*Recursivo (realiza la union de código automaticamente)
*Manual (hay que resolver los conflictos a mano)

## abortar ultimo merge

```sh
git merge --abort
```


## volver a la ultima rama

```sh
git switch -
```

## crea nueva rama y se mueve a ella

```sh
git switch -c rama2
```

## STASH (permite guardar cambios en local sin que se suban o se sobre escriban si uno baja lo del remoto, o sea es como bloques temporales en local que se almacenan en formato "pila" para guardar los cambios actuales sin borrarlos pero permitir trabajar en otros cambios sin nada de lo que se guardo en el stach, al realizar el comando guarda los cambios y los borra para dejar los archivos como antes de los cambios)

```sh
git stash # crea el stach
git stash list # muestra la lista de stach
git stash pop # recupera el ultimo stach
git stash apply stash@{0} # si no se le pone el numero, recupera el ultimo, si no, recupera el que se le indica por el numero sacado con list
git stash drop stash@{0} # si no se le pone el numero, borra el ultimo, si no, borra el que se le indica por el numero sacado con list
```