## Repositorio devjumpers
* git clone https://github.com/MGonzalezx/repositorio-devjump.git

## README

* touch README.md

## Commit inicial
* git add .
* git commit -m "commit inicial"

## Push inicial
* git push

## Ignorar archivos

### El .gitignore

El archivo .gitignore es un archivo de texto que le dice a Git qué otros archivos y carpetas de un proyecto debe ignorar.

Un archivo .gitignore local se coloca normalmente en el directorio de origen de un proyecto. También puedes crear un archivo .gitignore global y cualquier entrada que contenga será ignorada en todos tus repositorios Git por igual.



* touch privado.txt
* mkdir privada
* touch git.txt

------
Usé el cmd para cambiar el nombre y extensión del archivo de la siguiente manera: rename git.txt .gitignore
Dentro del .gitignore, escribo las siguientes líneas para ignorar el archivo privado.txt y la carpeta privada:
#### /privada
#### privado.txt
------

## Añadir fichero
* touch 1.txt

## Crear una rama v0.2
* git checkout -b v0.2
* touch 1.txt
* touch 2.txt

## Crear rama remota
* git push origin v0.2
* git push --set-upstream origin v0.2
* git add .
* git commit -m "Creación de rama v0.2 con su respectivos archivos y carpetas junto con un .gitignore"
* git push

## Merge directo
* git checkout main
* git merge v0.2
* git push

## Merge con conflicto
* git add .
* git commit -m "Escribir Hola en el archivo 1.txt"
* git checkout v0.2
* git add .
* git commit -m "Escribir Hola en el archivo 1.txt de la branch v0.2"
* git checkout main
* git merge v0.2

## Listado de ramas

### Investigar los comandos: --merged--no-merged

Para averiguar el estado de las ramas, filtrarlas y mostrar solo aquellas que han sido fusionadas (o que no lo han sido) con la rama actualmente activa. Para ello, Git dispone de las opciones --merged y --no-merged.

* git branch --merged
* git branch --no-merged

## Arreglar conflicto
* Edite el 1.txt dejando lo que estaba en HEAD.
* git add .
* git commit -m "Resolviendo conflictos con branch v0.2"
* git push

## Borrar rama
* git branch -d v0.2

## Listado de cambios
 
 ![alt text](https://github.com/MGonzalezx/repositorio-devjump/blob/main/Screenshot_3.png)

