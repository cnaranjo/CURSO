Configurar GIT Global para todos los repos (en cualquier momento antes de hacer el primer commit):

```sh
git config --global user.name "Carlos Naranjo"
git config --global user.email "carlos.naranjo@opens.cl"
```

Configurar GIT Local (debe ser despues de iniciar el repo):

```sh
git init
git config --local user.name "Carlos Naranjo"
git config --local user.email "carlos.naranjo@opens.cl"
```

Lista de commits:

```sh
git log
```