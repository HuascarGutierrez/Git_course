# Git_course
Los primero que hay que hacer en git es configurar el alias y el correo electronico

3 tipos de jerarquias 
- sistema
- global
- local

local es solo para un repositorio, global en para todos los repositorios dentro de un usuario, mientras que sistema es para todos los usuarios

git config (accede a las configuraciones ) 

git config --global (accede a las configuraciones globales) (existen, system, global y local)

git config --global user.name (usuario.nomre es coomo el atributo(nombre) del usuario)

git config --global user.email 

git config --list (nos muestra como esta configurado nuestro git, aqui podemos ver nuestro nombre como email)

git config --global --list (configuracion del git a nivel global)

clear (limpia la pantalla)

git config --global core.editor "code --wait" (esto lo enlaza al visual studio code y espera a que el git se cierre(tiene que ver con los commits))

git config --global color.ui true (da color a los que sale por el terminal)

git config --global core.autocrlf true (soluciona los problemas de compatibilidad entre linux y windows (\r\n))

(cuando estamos en mac, linux o UNIX, entonces cambiamos el true a input)

## REPOSITORIO
el repositorio es el lugar donde guardamos todo y donde tenemos todo para poder administrarlo 
AREAS
- Area de trabajo
- Stagging area (donde subimos los cambios que posteriormente enviaremos al repositorio)
- repositorio

comandos de linux
- mkdir (crear carpeta)
- rmdir (eliminar carpeta)
- ls (lista)
- ls -a (lista con los elementos oculto)
- pwd (muestra la dirrecion o path)

comandos de git (aparte de la configuracion inicial)
- git add archivo (si quieres cargar todos los archivos, entonces pones .) (lo envias al stagging area) (si quieren agregar mas de un archivo solamente le dan espacio al primero y continuan con le siguiente ej. git add archivo1.txt archivo2.txt)
- git status (muestra la rama y los commits - informacion del area de trabajo y la preparacion)
- git rm --cached archivo (lo quita del changes to be committed) (puedes hacer lo mismo que el add para eliminar varios archivos)
- git commit (hace lo mismo que el de abajo, solamente que con un mensaje largo)
    
/*  
    # Please enter the commit message for your changes. Lines starting
    # with '#' will be ignored, and an empty message aborts the commit.
    #
    # On branch master
    # Changes to be committed:
    #	modified:   hola_mundo.txt
    #
*/
te sale algo asi, cuando es commit en el editor que haya puesto (en =mi caso visual code), puedes eliminarlo y poner el mensaje, no te olvidesa de guardar el mensaje

- git commit -m "message" -a (el -a es opcional, se cra un commit, lo cual esta en el repositorio)
- git commit -a (hace un salto directo del area de trabajo al repo)
ejemplo en el repo git_ejemplo

la rama MASTER esta como estandar

Existen dos tipos de archivos para los commits
- untracked files (archivos que no se cargartan al stagging area)
- changes to be commited (archivos que si se cargaran al stagging area)
