# Git-GitHub-Crash-Course




### Git-Guide-tutorial.
#### Learn GitHub basic commands - Step by Step. (for beginners from scratch) | Definitive guide tutorial project.


##### PRIMERA PARTE: 

- abrir git bass....

- en la consola de git irse adentro de la carpeta del proyecto:  cd desktop/"my proyecto(folder)"

- iniciar epositorio: git init

- hacer listado: ls -l    or  ls.

- git status (ver que archivos tenemos sin agrega a nuestro repo)

- git add  (para empezar a agregar nuestros archivos al repo local)

- git status (despues de añadirlos, vemos los cambios con este comando)

- Crear ".gitignore": para explicarle que archivos, como dependencias, etc... no queremos que suba...

- primer git snapshot:

     git config --global user.email "myemail@myemail.com"

     git config --global user.name "your username"

- Sincronizar general:  
git commit -m 'type a message here' or en el editor VSCode (guardar los cambios en nuestro repo / con este comando hacemos o tomamos nuestro snapshot)

- git status (para ver todos los cambios que hemos hecho)

- git log (para ver las "fotos" or "Snapshot" que hemos hecho hasta ahora)

---------------------------------------------------------------------------------------------------------------
##### Nota: hasta aqui los 3 comandos basicos son...

- git add
- git commit-m 'text here...'
- git status
----------------------------------------------------------------------------------------------------------------


##### SEGUNDA PARTE:


Luego si descargamos, y estamos editando un proyecto o el mismo proyecto que hemos creado y estamos trabajando hasta este punto ...

1). si quisieramos añadir cambios a  los archivos de un proyecto o repo en git que esta en nuestro local:

- (producimos los cambios al codigo en nuestro editor VSCode y guardamos)

- git status (para ver los cambios hechos en el repo)

- git diff (para ver las diferencias cuando hemos modificado un archivo)

- git checkout   --"nombre del archivo ejm: index.html" (para descartar o remover los cambios hechos a calquier archivo)

- git commit  -m or git commit  -m 'type text-message here'  (para guardar los cambios en nuestro repo / es decir tomar un snapshot)

- git log (nuevamente, para ver las "fotos" or "Snapshot" que hemos hecho hasta ahora)


 ##### TERCERA PARTE:

Añadir el archivo ".gitignore"

- Creamos en nuestro proyecto un archivo: .gitignore  (es un archivo al cual le dare nombres de carpetas y archivos que ignores)

- Creado el archivo (".gitignore") le escribimos en el los nombres de los archivo y de las carpetas que queremos que ignore

- git status (observamos que ya no aparece la carpeta que ignoramos, pero si aparece el archivo ".gitignore")

- git add .gitignore (para añadir el archivo con los ambios hechos a nuestro repo)

- git status (ver los cambios)

- gt commit  -m "type text-message here" (parra hacer un snapshot o foto del proyecto guardando, sincronizando o añadiendo os nuevos cambios hasta ahora del proyecto con el archivo ".gitignore" que acabamos de añadir)


---------------------------------------------------------------------------------------------------------------
##### Nota: 

hasta ahora lo mas imporante es conocer que estamos trabajando con un proyecto con multiples archivos, y cuando estamos trabajando en un proyecto y quisieramos alterar esos archivos, para obtener una mini version de como alteramos el codigo...

Si queremos ignorar una carpeta o folder  con todos los archivos dentro ponemos "nombrecarpeta/".
Para ignorar un archivo en especifico dentro de una carpeta ponemos: "NombreCarpeta/NombreArchivo"
Para ignorar un archivo basta con poner solamente tal cual el nombre del archivo que queremos ignorar

----------------------------------------------------------------------------------------------------------------


##### CUARTA PARTE:

Hacer una miniversion del projecto original, principal o master. Para trabajar en los cambios que haremos antes de añadirlo o enviarlo al projecto original o master... (hay que recordar que git funciona por ramas, la rama master o rama principal, luego las subramas que son las copias que se bajan los desarrolladores y estan trabajando en su entorno local de trabajo, para luego una vez hecho los cambios, trabajo, modificacion del codigo, etc... se añada al codigo principal global o proyecto general "master", paraposteriormente salir a produccion...)


- git branch  (ademas de la original o principal, muestra las ramas o versiones alternativasque tenemos)

- git branch (nombre dela version alternativa, ejm: "login") (con este comando creamos una nueva version alternativa del proyecto)

- git checkout (nombre dela version alternativa, ejm: "login") (para movernos dentro de la nueva version alternativa que acabamos de crear o a la que hemos ingresado con el mismo comando, usamos ese comando). (asi, qe ahora nos dira que estamos dentro de la rama que acabamos de crear la rama "login")

- git branch (ahora nos muestra que tenemos dos ramas la principal u original: "master", y la que recien hemos creado: "login"

- git add (nombre de la carpeta/archivo) or git add . (guardamos todos los nuevos archivos que acabamos de añadir al proyecto y si fuesemos a guardar multiples archivos simplemente es decir: "git add ." con este comando guardamos multiples archivos a la vez)

- git status  (vemos los archivos que hemos añadido como el ".gitignore" y el "app.py", tambien no observamos las carpetas que hemos creado: "login y autentification" porque esta vacia y no sirven para nada, asi que es por eso que git ya las ignora, por eso aparece en nueva fila añadida el ".gitignore", al darle al git status)

- git commit -m type text-message here: 'para version alternativa con un nuevo login' (ahora podemos hacer un commit: para guardar los cambios en nuestro repo / es decir tomar un snapshot. Y crear una otra, nueva version, con los camios que deseemos hacer ahora...)

- git log (y ahora con este comando vemos las multiples fotos o snapshot que hemos hecho en neustro proyecto, pero en la rama login)

- git branch (vamos a pararnos en el inicio del proyecto y cambiamos a la rama master)

- git chekout 'master' (para cambiar a la rama master y ver los cambios de que ya no tenemos los archivos que habiamos añadido en la rama de la version login) (ahora hemos cambiado a la version de la rama master)

- git log (si presionamos este comando vemos como no tenemos todos los commits/snapshot que faltan, que anteriormente habiamos hecho en la version de la rama login.)


---------------------------------------------------------------------------------------------------------------
##### Nota: 

Entonces, resumiendo esta 4a. parte, vemos que es una manera de poder jugar con versiones alternativas, esa es la magia o la verdadera ensencia de git. 
Asi que esto es lo tipico cuando trabajamos con un repositorio de codigo. Por lo tanto podemos entender que git es un repositorio para control de versiones para nuestros proyectos. 
Siendo el original,principal y/o global el "master", y desprendiendosen como ramas desde ahi cuantas infinitas versiones queramos "todas ellas de diferente tipo y naturaleza", 
que cada desarrollador enfocado en esa rama, pueda clonar/escargar, trabajar, adaptar a su entorno especial de trabajo y añadir los cambios a la otras versione principales o rama master directamente...

----------------------------------------------------------------------------------------------------------------


##### QUINTA PARTE: 

Crear y Subir repo a GitHub or GitLab:

#ejemplo de los comandos basicos dados cuando creamos nuestro nuevo repo:

Quick setup — if you’ve done this kind of thing before...

Link del WebSite or URL donde estara neustro Repo: https://github.com/brianparkerin/git-guide-tutorial.git

 …or create a new repository on the command line

echo "# git-guide-tutorial" >> README.md

git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/brianparkerin/git-guide-tutorial.git
git push -u origin master

…or push an existing repository from the command line
git remote add origin https://github.com/brianparkerin/git-guide-tutorial.git
git push -u origin master

…or import code from another repository

You can initialize this repository with code from a Subversion, Mercurial, or TFS project.


 - Subir Repositorio a GitHub:

1). git remote add origin https://github.com/brianparkerin/git-guide-tutorial.git (copiamos del repositorio este comando y lo insertamos y le damos enter...)

- git status (para ver los cambios que han sucedido)

- git remote -v (este comando nos indica todos los remotes que hay, y nos muestra que ya esta apuntando a origin remote en GitHub, GitLab o Bitbucket)

2). git push -u origin master (ahora con este otro comando como tal vamos a subir/empujar nuestro codigo al repositorio en GitHub or GitLab)


---------------------------------------------------------------------------------------------------------------
##### Nota: 

Basicamente en GitHub como en GitLab son 2 comandos, que haran que enviemos todo el codigo a nuestro repo en github: 

1). Mensaje remote origin command: (asociar en Git la URL del repo en github con los archivos que acontinuacion vamos a enviar)... git remote add origin https://github.com/brianparkerin/git-guide-tutorial.git

2). Push Command: (empujar los archivos al repo en GitHub) git push -u origin master 

... y por ultimo si nos aparece un login en una ventana emergente pidiendonos autentificarnos, lo hacemos. Ahora si refrescamos la pagina o la URL de nuestro repo podemos apreciar que ya se ha importado en el todo el proyecto con nuestro codigo o cambios que hemos a la pagina de GitHub.

----------------------------------------------------------------------------------------------------------------


Made with ❤ by...


##### Brian Pulgarin.

Ceo & Co-founder of underfix.com
