# Clase 6

## TAGS

* Son punteros que sirven para por ejemplo marcar diferentes versiones o puntos especificos en que se cambio algo importante en un commit y luego poder ejecutar comandos git sobre ese puntero en vez de buscar el tag


```sh
git tag puntero-tag (hash commit) # si no se le agrega el hash lo pone en el ultimo commit de la rama en que estoy
git tag -a v1.0.1 -m "Prueba de tag" # -a es el puntero
git tag -d (puntero) # borra el tag
git tag # lista los tag
```

mostrar info de un commit

```sh
git show (tag/hash)
```

subir tag a repo remoto

```sh
git push origin (tag)
```

borrar puntero del repo remoto

```sh
git push --delete origin (tag)
```

## FORK: agregar repo repoto extra del mio para poder trabajar en proyectos colaborativos (el fork se hace desde el repo colavorativo al mio)

```sh
git remote add upstream (repo remoto al hacer fork) # es lo mismo que unir un repo local con el mio remoto solo que este le agrega otro que no es mio y donde tengo que pedir que hagan el merge en git
git pull upstream main # sincroniza cambios del remoto colavorativo a mi local
```

## Punteros
- Estaticos: branch, Tags
- Dinamicos: HEAD

## REBASE
igual que el merge, trae lo de la rama seleccionada a la rama actual pero si tiene que aplicar merges no crea commits nuevos como el merge

```sh
git rebase rama2
```

rebase interactivo: muestra un editor que permite separar commits, corregir nombres etc

```sh
git rebase -i (hash) # hash hasta donde editare los commits
```