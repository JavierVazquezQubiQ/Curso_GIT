# Documentación

Como usar protocólo SSH para clonar repositorios.

1. Primero tendremos que conocer la clave pública de nuestro dispositivo, para ello tendremos que ejecutar el siguiente comando en la terminal "ssh keygen -b 2048 -t rsa". A continuación la terminal nos comunicara que escribamos un nombre para ese archivo pero nosotros pulsaremos -ENTER- y continuaremos, si nos pide algo más le damos igualmente a enter hasta que nos la cree. A continnuación nos movemos a la ruta donde se haya creado esta clave con el comando "cd", posteriormente con el comando "ls" podemos ver el contenido de ruta y copiamos las palabras "id_rsa.pub" para finalmente poner el siguiente comando en la terminal y que nos aparezca esta clave pública "cat id_rsa.pub". Copiamos la clave pública y pasamos al siguiente paso.

2. Ahora debemos enlazar la clave pública con GIT, para ello pinchamos en la etiqueta de nuestro perfil (arriba a la derecha) vamos al apartado settings, bajamos y marcamos en "SSH and GPG keys" -> "New SSH key". Ponemos título que queramos y en el siguiente cuadro copiamos la clave pública del paso 1.

3. Para clonar repositorios marcamos en GIT la opción de "Code" y copiamos URL del protocolo SSH. A continuación abrimos la terminal y nos movemos desde la consola al directorio donde queremos clonar ese proyecto con el comando "cd" un ejemplo sería "cd proyectos". Una vez que estamos en el directorio deseado simplemente utilizaremos el siguiente comando y el repositorio se clonará en la ruta elegida "git clone <URL con protocolo SSH copiada en la página de GIT>.