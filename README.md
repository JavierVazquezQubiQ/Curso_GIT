# Curso_GIT

# GIT es un sistema de control de versiones, nos permite gestionar los cambios que habido en uno o varios documentos.

En este curso vamos a aprender a usar la operatica principal de GIT además de todas las interactuacciones posibles con esta plataforma como subir repositorios, modificar repositorios, añadir ramas modificar ramas desde la terminal, fusionar ramas añadidas a la rama máster (MAIN), etc...

### Un repositorio es un esoacio virtual donde almacenamos un proyecto.

### Una rama es un espacio de trabajo dentro del repositorio. Trabajar con ramas nos permite trabajar de forma independiente. GIT nos permite duplicar estos espacios de trabajo y realizar cambios para que varias personas puedan trabajar de forma paralela.

### COMMIT: Actualización de cambió en alguna rama. Cada rama tiene un histórico de commits o cambios. Con este sistema de control de versiones podemos hacer y desacer cambios concretos. Los commits guardan la información de los cambios que hemos realizado en una rama.

### Como usar protocólo SSH para clonar repositorios.

1. Primero tendremos que conocer la clave pública de nuestro dispositivo, para ello tendremos que ejecutar el siguiente comando en la terminal "ssh keygen -b 2048 -t rsa". A continuación la terminal nos comunicara que escribamos un nombre para ese archivo pero nosotros pulsaremos -ENTER- y continuaremos, si nos pide algo más le damos igualmente a enter hasta que nos la cree. A continnuación nos movemos a la ruta donde se haya creado esta clave con el comando "cd", posteriormente con el comando "ls" podemos ver el contenido de ruta y copiamos las palabras "id_rsa.pub" para finalmente poner el siguiente comando en la terminal y que nos aparezca esta clave pública "cat id_rsa.pub". Copiamos la clave pública y pasamos al siguiente paso.

2. Ahora debemos enlazar la clave pública con GIT, para ello pinchamos en la etiqueta de nuestro perfil (arriba a la derecha) vamos al apartado settings, bajamos y marcamos en "SSH and GPG keys" -> "New SSH key". Ponemos título que queramos y en el siguiente cuadro copiamos la clave pública del paso 1.

3. Para clonar repositorios marcamos en GIT la opción de "Code" y copiamos URL del protocolo SSH. A continuación abrimos la terminal y nos movemos desde la consola al directorio donde queremos clonar ese proyecto con el comando "cd" un ejemplo sería "cd proyectos". Una vez que estamos en el directorio deseado simplemente utilizaremos el siguiente comando y el repositorio se clonará en la ruta elegida "git clone <URL con protocolo SSH copiada en la página de GIT>.

Resumen de comandos más utilizados:

Nos da un listado de comandos con una descripción de lo que hace cada uno:

git --help

Cambiar de rama, si la rama no existe devuelve un error:

git checkout "nombre"

Cambia de rama y si no existe esta rama creamela:

git checkout -b "nombre"

Nos dice en que rama estamos y si tenemos algún commit pendiente de subir:

git status