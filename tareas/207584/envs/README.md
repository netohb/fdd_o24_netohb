# Virtualenv
Debes crear un virtualenv en tu local siguiendo las siguientes instrucciones. Investiga las instrucciones y adaptalas al repositorio actual. 

## Ejercicio
Crea un pyenv para este repo y anota las instrucciones en formato de codigo de markdown en este README (abajo), tanto para instalar el env como para activarlo. La idea es que si se te olvida o alguien mas descarga este repo puedas copiar y pegarlas sin ningun problema. No hagas `add` o `commit` por que falta crear los `ignores` (instrucciones mas adelante).  

Para asegurarte que funciono correctamente debe ser capaz de ejecutar `python app.py` sin problemas.

### Instrucciones
#### Instalacion
`Ya viene instalado junto con python`
#### Activar virtualenv
`ctrl+shift+P` abre la command palette y se sigue la opcion de crear un Virtual Env...

# Conda
Instrucciones para crear un ambiente de conda `environment.yml.` Adapta las instrucciones al repositorio actual, no son exactas.

## Ejercicio
Crea un conda env para este repo y anota las instrucciones en formato de codigo de markdown en este README (abajo), tanto para instalar el env como para activarlo. La idea es que si se te olvida o alguien mas descarga este repo puedas copiar y pegarlas sin ningun problema. No hagas `add` o `commit` por que falta crear los `ignores` (instrucciones mas adelante).  

Para asegurarte que funciono correctamente debe ser capaz de ejecutar `python app.py` sin problemas.


### Instrucciones
#### Instalacion
`wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh` descarga Miniconda

`bash Miniconda3-latest-Linux-x86_64.sh` corre el instalador
#### Activar conda env
`conda init `


# .gitignore
Algunos ambientes virtuales como `pyenv` pueden crear carpetas, asegurate de no subir estas carpetas. Esto lo puedes lograr omitiendo el add a estas careptas y aregandolas al .gitignore.  
No se aceptaran tareas que traigan archivos binarios de python, solo debe subirse el codigo. Tambien debe evitarse subir tus archivos `.env` o claves en general por ello es necesario incluir estos archivos en el gitignore, pero agregar un ejemplo al github para que se pueda replicar en el local en este caso lo llamos `.env_ejemplo`.

## Ejercicio
Crea tu `.gitignore` en tu copia de esta carpeta en tu folder de tareas verifica como funciona el wild card notation para lograr que aplique a todas tus subcarpetas.
*Tienes que investigar, inferir, googlear que carpetas son creadas para agregarlas al .gitignore*
Asegurate de agregar todas las cosas necesarias a tu `.gitignore` para que no suba archivos de los envs de python ni de conda a github

# .dockerignore
Igual que git, docker tiene su archivo .gitignore. Y dado que el punto de construir `build` un contenedor es hacer replicable todo dentro del mismo por lo que copiar estos archivos es mala practica por que peude provocar errores o aumentar la memoria.  Por lo mismo es necesario crear un  `.dockerignore`

## Ejercicio
Crea tu `.gitignore` en tu copia de esta carpeta en tu folder de tareas verifica como funciona el wild card notation para lograr que aplique a todas tus subcarpetas.
*Tienes que investigar, inferir, googlear que carpetas son creadas para agregarlas al .dockerignore*
Asegurate de agregar todas las cosas necesarias a tu `.gitignore` para que no suba archivos de los envs de python ni de conda a tu imagen de dockerhub.

# Docker
Ahora tienes que crear un docker que utilice `virtualenv` (no pipenv sino virtual env) para instalar los paquetes. Modifica el `Dockerfile.ejemplo` para que instale las cosas correspondientes y pueda ejecutar `python app.py` sin problemas.  

# Entrega de Ejercicios
Una vez que esten los ejercicios listos, sube tu imagen de docker a tu repositorio de docker hub y agrega la liga de ese contenedor aqui:  
## Docker
https://hub.docker.com/layers/brauliopm/itam/envs/images/sha256-04eea8bbe6670249356500e9f025501e4b008e60726825fe40a07cabb8d864d4?context=repo 
## Github
Pide un pull request con las modificaciones necesarias.