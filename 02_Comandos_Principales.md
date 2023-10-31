# Resumen de comandos más utilizados:

echo "Test" >> test.txt

echo "Lo_Que_Queremos_Escribir_Dentro_Del_Documento" >> "Nombre_Documento"."Formato_Documento"

Crea un documento de texto en el proyecto con una linea dentro que pone "Test" y nombre del archivo "test.txt". Este comando crea un documento en el formato que le especifiquemos como por ejemplo ".md", ".csv" o lo que sea.

------------------------------------------------------------------------------------------------------------------

git --help

Nos da un listado de comandos con una descripción de lo que hace cada uno:

------------------------------------------------------------------------------------------------------------------

git branch

Consultar el listado de ramas:

------------------------------------------------------------------------------------------------------------------

git checkout "Nombre_Rama"

Cambiar de rama, si la rama no existe devuelve un error:

git checkout -b "Nombre_Nueva_Rama"

Cambia de rama y si no existe esta rama creamela:

------------------------------------------------------------------------------------------------------------------

git status

Nos dice en que rama estamos y si tenemos algún commit pendiente de subir:

------------------------------------------------------------------------------------------------------------------

git add "Nombre_Documento_Concreto"

Agrega cambios al proceso de validación previo a la subida y actualización del repositorio (del área de trabajo o working directory al área de preparación o stagint area):

git add .

Agrega cambios al proceso anteriormente descrito masivamente de todos los archivos modificados:

------------------------------------------------------------------------------------------------------------------

git commit

Para validar lo cambios añadidos en el proceso add luego añadimos nombre para nombrar este proceso:

git commit -m "Nombre_Proceso"

También podemos unir los dos pasos anteriores en uno con el siguiente comando:

------------------------------------------------------------------------------------------------------------------

git log

Ver el historial de commits:

------------------------------------------------------------------------------------------------------------------

git push

Subir cambios al servidor remoto:

git push --set-upstream origin "Nombre_Rama"

Al ser la primera vez que creamos una rama debemos  vincular rama al servidor:

------------------------------------------------------------------------------------------------------------------

git reset HEAD "Nombre_Documento_Concreto"

Restrocede el documento concreto del área de preparación (staging area) al área de trabajo (working area). Lo que significa revertir el paso realizado con git add.

git reset HEAD .

Restrocede masivamente todos los documentosd del área de preparación (staging area) al área de trabajo (working area). Lo que significa revertir el paso realizado con git add.

------------------------------------------------------------------------------------------------------------------

git commit -am "Nombre_Proceso"

Unifica el paso de git add y git commit en uno solo lo que pasa nuestros cambios directamente del área de trabajo a confirmado.

------------------------------------------------------------------------------------------------------------------

git reset HEAD~"Número_Commit_Que_Queremos_Reiniciar"

Podemos revertir el número de commits que queramos para restablecer los cambios realizador.

------------------------------------------------------------------------------------------------------------------

