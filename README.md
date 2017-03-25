Git se diferencia de otro sistema de control de versiones, en el fondo no va guardando diferencias sino que va creando archivos 


*** 1. Para trabajar en Git lo que basicamente necesitamos es un Repositorio ***

- git init

Una de las cosas mas importantes es crear una carpeta de proyecto y acceder a ella


>Para crear un repositorio Git debemos estar dentro de la carpeta en donde lo crearemos

1.  mkdir -> Nombre de Carpeta, esta instrucción nos permite crear una carpeta a traves de la linea de comendos del terminal

>dentro de la carpeta creada inicializamos el ** git init **

2. Una vez que estamos dentro inicialiamos git que viene de cajón en Mac, una vez que inicilizamos usamos el comando 

	* ls -la -> para lograr ver los ficheros ocultos

3. con eliminar la carpeta .git se elimina el repositorio

***

# Git esta compuesto de 3 zonas



### esto es lo que lo hace distinto de otro sistema de control de versiones

***


1. Working copy -> es el directorio en el que estamos trabajando 
2. Staging Area -> donde vamos a ir colocando los archivos (index o caché)
3. Repository -> es donde se van a guardar los cambios

> lo primero que debemos saber es ¿Cómo esta mi repositorio?
- git status
> como pasamos un archivo del "Working copy" -> "Staging Area"
- git add <Nombre del archivo>
- git add <Nomnre de carpeta si tuvieramos una carpeta con modificaciones>
- git add * "y de aqui en adelante la extension -> .md / .swift / .java"
> como pasamos del staging Area -> Repositorio 
- git commit -> es un paqueta que contiene uno o mas "Hunks" -> diff (diferencia)
	- un commit va a tener uno o mas Hunks pero es un commit por archivo
    - un commit tiene un mensaje que describe que cambios van en ese commit -> debemos colocar buenos mensaje, decribir, cambios correctamente, para encontrar en el tiempo la recuperacion de un fichero
    - un commit tiene un hash (SHA) -> para identificar el commit
    - un commit tiene un enlace siempre con su padre
- git log -> asi podemos ver los commits desde el pabre al hijo


*** PANDOC ***
A traves del Terminal invocamos pandoc y el fichero .md que hemos construido, esto nos trasnforma el .md en html
- prompt / pandoc leeme.md
y esto nos saca la vision html que hemos escrito

- a traves del siguiente comando podemos transformar el .md en html 
- prompt / pandoc README.md > README.html --> esto nos creara otro fichero README en formato html

>Borra un fichero tambien es un cambio de cara a Git, asi que debemos ser concientes de esos cambios y como los interpreta GIT

- cuando borramos un fichero podemos hacerlo de varias formas
1. fisicamente desde el Finder
2. a traves del terminal con rm <Nombre del fichero>
3. git rm <nombre del fichero> -> este ultimo ademas de eliminar ficho fichero lo desplaza al Staging Area y lo saca del Working copy








