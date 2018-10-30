## Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos

### Zonas de Git
1. Directorio de trabajo
2. Area de preparacion
3. Directorio Git

### Flujo de trabajo basico en git
1.Modificas
2.Preparas los archivos
3.Confirmas

###Configurando Git por primera vez
```
git config --global user.name "Cesar Castillo"
git config --global user.email "alexander_4_11_4@hotmail.com"
git config --global core.editor subl
git config --list
```
## Configuración SSH en Windows
Usando Git Bash seguimos los siguientes pasos:

1. Creamos una carpeta llamada 'llaves-ssh' en el disco 'C' para evitar problemas de rutas.

2. Ejecutamos el comando 'ssh-keygen -t rsa -C "mi-correo@ejemplo.com"'.
El correo debe ser el mismo con el que nos registramos en Github para evitar posibles problemas.
Dejamos el passphrase vacio y damos enter.
Cuando nos pida la ruta escribimos '/c/llaves-ssh/github_rsa'.

3. Iniciamos ssh-agent en background ejecutando el comando 'eval "$(ssh-agent -s)"'.

4. Agregamos  la llave ssh generada a ssh-agent ejecutando el comando 'ssh-add /c/llaves-ssh/github_sra'.

5. Desde ahora podemos hacer pull y push sin que Github nos esté pidiendo los datos de acceso.