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

