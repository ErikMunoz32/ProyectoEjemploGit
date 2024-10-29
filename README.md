# Proyecto de Ejemplo Git

## Descripción
Este proyecto es una tarea de introducción a Git en la cual se crea un repositorio, se suben archivos, y se realiza el seguimiento de cambios. El programa principal es `HolaMundo.java`, un programa simple en Java que imprime un mensaje en pantalla. Además, se implementa un archivo `.gitignore` para ignorar archivos de prueba.

## Instrucciones de Uso
1. Compila el programa con el siguiente comando:
   ```bash
   javac HolaMundo.java

## Comandos utilizados
1. Codigo usado en git bash
   ```bash
   cd "C:\Users\Jessica\Documents\Fundamentossof\ProyectoEjemploGit"
   git init
   git remote add origin https://github.com/ErikMunoz32/ProyectoEjemploGit.git
   git add -A
   git commit -m "Se agregó el programa Hola Mundo en Java"
   git push origin master
   touch .gitignore
   git add -A
   git commit -m "Se agregó el archivo .gitignore"
   git push origin master
   git add -A
   git commit -m "Se actualizó el mensaje en HolaMundo.java"
   git push origin master
## Notas sobre el archivo .gitignore
El archivo .gitignore se creó para excluir archivos innecesarios o temporales que no deben incluirse en el repositorio. En este caso, los archivos con la extensión .log, como debug.log, están ignorados, lo que permite mantener el repositorio limpio.

## Salida esperada
1. Al ejecutar el programa HolaMundo.java, se debe mostrar el mensaje:
    ```bash
    Hola Git
## Comprobar que no se subio los .log
1. Para confirmar que debug.log no se subió al repositorio remoto, revisa el contenido del repositorio en GitHub, donde no debe aparecer este archivo entre los elementos listados.
2. Ademas de que tambien  se puede verificar ejecutando git status, donde debug.log no aparece entre los archivos sin seguimiento (untracked), lo cual indica que Git está ignorando correctamente este archivo.
