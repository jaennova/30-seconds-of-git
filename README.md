# 30 seconds of git

Fragmentos cortos de git para todas sus necesidades de desarrollo, inspirado en [30-seconds-of-code](https://github.com/30-seconds/30-seconds-of-git).
## Indice

- [Configurar tu usuario y corrreo en Git][git config]
- [Inicializar un repositorio en un directiorio local][git init]
- [Crear una copia local de un repositorio existente][git clone]
- [Crear un commit en una fecha en especifico][git date]
- [Editar ultimo commit][git commit amend]

## Fragmentos

## Configurar tu usuario y correo en Git

los siguientes son comandos para configurar tu nombre y correo en git para identificarte en tus commits. La opción --global hace que la configuración sea para todos los proyectos en tu equipo.

```shell
git config --global user.name "tu_nombre"
git config --global user.email "tu_correo@ejemplo.com"
```

#tags: configuracion, indentificacion, autor, global, email.

## Inicializar un repositorio en un directorio local

`git init` es un comando que se utiliza para iniciar un nuevo repositorio de Git en la carpeta actual, creando una carpeta oculta llamada ".git" para llevar un seguimiento de los cambios en los archivos. Es el primer paso para comenzar a trabajar con Git en un nuevo proyecto.

```shell
git init
```

#tags: crear repositorio, inicializar git, nuevo proyecto, crear carpeta .git.

## Crear una copia local de un repositorio existente

git clone es un comando para crear una copia local de un repositorio de git existente en otra ubicación, ya sea en un servidor remoto o en otra computadora local. Es utilizado para tener una copia local de un repositorio remoto.

```shell
git clone https://github.com/username/myproject.git
```

En este ejemplo se está clonando el repositorio "myproject" del usuario "username" en Github, en la ruta actual de la computadora local. Una vez ejecutado este comando, se habrá creado una carpeta llamada "myproject" con todos los archivos y la historia de commits del repositorio original.

Otra forma de usarlo seria:

```shell
git clone https://github.com/username/myproject.git myproject-local
```

En este caso se estaría clonando el repositorio en una carpeta llamada "myproject-local"

Es importante mencionar que para clonar un repositorio es necesario tener acceso de lectura al mismo, si es un repositorio público no se necesita autenticación, en cambio si es privado es necesario tener los credenciales necesarias para acceder al mismo.

#tags: clonar repositorio, copia local, descargar repositorio

## Crear un commit en una fecha en especifico

Para hacer un commit con una fecha específica en Git, puedes usar el siguiente comando:

```bash
GIT_AUTHOR_DATE="YYYY-MM-DDTHH:MM:SS" GIT_COMMITTER_DATE="YYYY-MM-DDTHH:MM:SS" git commit -m "mensaje"
```
Donde YYYY-MM-DD es la fecha y HH:MM:SS es la hora. 

Por ejemplo, si deseas hacer un commit el 11 de enero de 2022 a las 10:00 AM, el comando sería:

```bash
GIT_AUTHOR_DATE="2022-01-11T10:00:00" GIT_COMMITTER_DATE="2022-01-11T10:00:00" git commit -m "mensaje"
```

Recuerda reemplazar git commit con tus propios mensajes de commit y opciones.

## Editar el ultimo commit

Si deseas editar el último commit que realizaste, puedes hacerlo utilizando el comando:
```bash
git commit --amend
```

Este comando te permitirá hacer cambios en el último commit, ya sea para agregar o modificar archivos o para cambiar el mensaje de confirmación.



<!-- 

### git add [archivo]



### git add .



### git commit -m "mensaje del commit"



### git status



### git log



### git diff



### git show [hash del commit]



### git branch



### git branch [nombre de la rama]



### git checkout [nombre de la rama]



### git merge [nombre de la rama]



### git pull



### git push



### git remote



### git remote -v



### git remote add [nombre del remoto] [url del repositorio]



### git fetch [nombre del remoto]



### git remote rename [nombre actual del remoto] [nuevo nombre del remoto]



### git remote remove [nombre del remoto]



### git tag



### git tag -a [nombre de la etiqueta] -m "mensaje de la etiqueta"



### git tag -d [nombre de la etiqueta]



### git push [nombre del remoto] [nombre de la rama]



### git push --tags



### git push [nombre del remoto] :[nombre de la rama]



### git stash



### git stash list



### git stash apply [número del stash]



### git stash drop [número del stash]



### git stash pop [número del stash]



### git stash branch [nombre de la rama] [número del stash]



### git config --global alias.[alias del comando] [comando]



### git config --global color.ui auto



### git config --global core.editor [nombre del editor de texto]



### git config --global merge.tool [nombre de la herramienta de merge]



### git config --global push.default [simple/matching/current]



### git config --global core.autocrlf [true/input/false]



### git config --global core.filemode [true/false]



### git config --global core.whitespace [trailing-space/space-before-tab/indent-with-non-tab/


cr-at-eol]
### git config --global core.excludesfile [ruta del archivo de exclusiones]



### git config --global core.attributesfile [ruta del archivo de atributos]



### git config --global core.sparsecheckout [true/false]



### git config --global core.preloadindex [true/false]



### git config --global core.fscache [true/false]



### git config --global gc.auto [número]



### git config --global gc.autopacklimit [número] -->


[git config]: #configurar-tu-usuario-y-correo-en-git
[git init]: #inicializar-un-repositorio-en-un-directorio-local
[git clone]: #crear-una-copia-local-de-un-repositorio-existente
[git date]: #crear-un-commit-en-una-fecha-en-especifico
[git commit amend]: #editar-el-ultimo-commit
