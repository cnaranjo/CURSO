# Clase 4

## Ramas (branches)

```sh
git branch # muestra las ramas
git branch rama1 # crea una rama
git switch rama1 # cambio de rama
```

## para mezclar ramas (parado en la rama hacia donde se quiere traera lo de la otra rama)

```sh
git merge rama1
```

## para eliminar ramas

```sh
git branch -d rama1
```

## para clonar repo

```sh
git clone [url repo git]
```

## muestra el log con un mini grafico de la union de ramas

```sh
git log --oneline --graph --all --decorate
```

## subir rama

```sh
git push -u origin rama1
```

## traer metadata del repo remoto

```sh
git fetch --all
```