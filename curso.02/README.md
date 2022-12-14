# Clase 2

Configurar GIT Global para todos los repos (en cualquier momento antes de hacer el primer commit):

```sh
git config --global user.name 'Carlos Naranjo'
git config --global user.email 'carlos.naranjo@opens.cl'
```

Configurar GIT Local (debe ser despues de iniciar el repo):

```sh
git init
git config --local user.name 'Carlos Naranjo'
git config --local user.email 'carlos.naranjo@opens.cl'
```

Crear commit de cambios en stage:

```sh
git commit -m 'Comentario'
git commit --amend # agrega nuevas modificaciones en stage al ultimo commit ya ingresado
```

Lista de commits:

```sh
git log
git log --oneline
```

Compara y muestra diferencias entre el repo y los archivos locales modificados sin agregar al stage:

```sh
git diff
```

Para unir un repo remoto creado con el local:

```sh
git remote add origin https://github.com/cnaranjo/CURSO.git
git push -u origin main # origin es el alias que se puso en el comando anterior, en caso de clon por defecto tambien es origin pero se puede ver con el comando de abajo, main seria la rama local, la primera vez este comando pedira el password para conectarse al repo
```

Muestra alias del repo remoto:

```sh
git remote -v
```