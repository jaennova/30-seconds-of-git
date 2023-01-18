# 30 seconds of git

Fragmentos cortos de git para todas sus necesidades de desarrollo, inspirado en [30-seconds-of-code](https://github.com/30-seconds/30-seconds-of-git).
## Indice

- [Configurar tu usuario y corrreo en Git][git config]
- [Inicializar un repositorio en un directiorio local][git init]

## Fragmentos

### Configurar tu usuario y correo en Git

los siguientes son comandos para configurar tu nombre y correo en git para identificarte en tus commits. La opción --global hace que la configuración sea para todos los proyectos en tu equipo.

```shell
git config --global user.name "tu_nombre"
git config --global user.email "tu_correo@ejemplo.com"
```

#tags: configuracion, indentificacion, autor, global, email.

### Inicializar un repositorio en un directorio local

`git init` es un comando que se utiliza para iniciar un nuevo repositorio de Git en la carpeta actual, creando una carpeta oculta llamada ".git" para llevar un seguimiento de los cambios en los archivos. Es el primer paso para comenzar a trabajar con Git en un nuevo proyecto.

```shell
git init
```

#tags: crear repositorio, inicializar git, nuevo proyecto, crear carpeta .git.


[git config]: #configurar-tu-usuario-y-correo-en-git
[git init]: #inicializar-un-repositorio-en-un-directorio-local