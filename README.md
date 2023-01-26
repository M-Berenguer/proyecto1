# Este es el primer proyecto del curso

## Creacion de repo:
git init

## Añadir un fichero
git add <nombre_fichero>    # Añadir un fichero
git add *                   # Añadir todos los ficheros del directorio. NO AÑADE OCULTOS
git add .                   # Añadir todos los ficheros del directorio. SI AÑADE OCULTOS
Empezar a controlar el fichero...
Pasar el fichero al área de STAGING

# Qué guarda GIT?
Git sólo guarda ficheros, NO GUARDA DIRECTORIOS

# OBJETOS EN GIT
## Workspace:
La carpeta en la que tengo mi proyecto, en la que trabajo
## Staging
Es un fichero que se guarda dentro de la carpeta .git, que va anotando los cambios
que se van a mandar al REPO desde el área de STAGING
## Repo
La carpeta .git

## Información del estado del proyecto
git status

## Qué es un commit??
Un >>>paquete de cambios<<< que se registra en el repo
Los commits (paquetes de cambios) se aplican de forma INCREMENTAL

## Sacar un fichero del área de STAGING
git rm --cached <nombre_fichero>

## Borra el fichero
- del WORKSPACE
- En el staging se le dice que en el proximo paquete de cambios, se elimine el fichero
git rm <nombre_fichero>

# Mandar los cambios que hay apuntados en el AREA de STAGING al repo
git commit -m 'mensaje'

git config --global user.name "Your Name"
git config --global user.email you@example.com
Esto "toca" el archivo interno .git/config

# Ver lo que hay en el repositorio
git ls-files

# Hacer un add automatico de los cambios de los ficheros QUE YA SE ESTAN CONTROLANDO
  y de esos cambios se hace un COMMIT
  
git commit -am 'Superheroes DC'