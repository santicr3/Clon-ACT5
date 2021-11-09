# Ejercicios de creación y actualización de repositorios

## Ejercicio 1

1. Crear un repositorio nuevo con el nombre libro y mostrar su contenido.
2. Configurar Git definiendo el nombre del usuario, el correo electrónico y activar el coloreado de la salida. Mostrar la configuración final.

~~~
mkdir libro
cd libro
ls -la
git init
ls -la
~~~

Nombre de usuario:
~~~~
git config --global user.name "Nombre"
~~~~
Correo electronico del usuario:
~~~~
git config --global user.email "email"
~~~~
Activar coloreado:
~~~~
git config --global color.ui auto
~~~~
Mostrar configuración
~~~~
git config --list
~~~~

## Ejercicio 2

1. Comprobar el estado del repositorio.
~~~~
git status
~~~~
2. Crear un fichero indice.txt con el siguiente contenido:
   
    ![ejercicio1.2](imagenes/ejercicio12.png)

1. Comprobar de nuevo el estado del repositorio.
2. Añadir el fichero a la zona de intercambio temporal.
3. Volver a comprobar una vez más el estado del repositorio.

~~~~
nano indice.txt
git status
git add
~~~~

## Ejercicio 3

Realizar un commit de los últimos cambios con el mensaje “Añadido índice del libro.” y ver el estado del repositorio.

~~~
git commit -m "Añadido índice del libro."
~~~

## Ejercicio 4

1. Cambiar el fichero indice.txt para que contenga lo siguiente:

    ![ejercicio1.2](imagenes/ejercicio14.png)

 
2. Mostrar los cambios con respecto a la última versión guardada en el repositorio.
3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3 sobre gestión de ramas”.

~~~
nano indice.txt
git diff
git add .
git commit -m "Añadido capítulo 3 sobre gestión de ramas”
~~~

## Ejercicio 5

1. Mostrar los cambios de la última versión del repositorio con respecto a la anterior.
2. Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.”
3. Volver a mostrar los últimos cambios del repositorio.

~~~
git diff
git commit --amend -m "Añadido capítulo 3 sobre gestión de ramas al índice."
git show
~~~


## Ejercicio 6

Indica a Git que quieres que ignore todos los ficheros que empiecen per “dam”, todos los que 
tengan la extensión out y las imágenes (jpg, png, bmp y gif). 

No lo he encontrado


