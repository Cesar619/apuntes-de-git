### git log
Muestra todo el historial de commits del proyecto

git log --pretty=format:"%h - %an, %ar : %s"
Muestra el historial con el formato que le indicamos.

####Limitar la salida del historial
`git log -n`: Cambiamos la n por cualquier numero entero, por ejemplo:`git log -2` nos mostrara los 2 commits mas recientes.

`git log --after="2018-09-27 00:00:00"` : Muestra los commits realizados despues de la fecha especificada.

`git log --before="2018-09-29 00:00:00"` : Muestra los commits realizados antes  de la fecha especificada.

Las banderas del comando `git log` se pueden usar juntas segun nos convenga, por ejemplo:

`git log --after="2018-09-27 00:00:00" --before="2018-09-29 13:00:00"`
