# Notas GIT

### Estados de los archivos ###

- **Committed:** Es la parte en la que nuestra información está segura alojada en nuestras bases de datos.

- **Modified:** En esta parte hemos realizado cambios en nuestros archivos, pero aún no se ven reflejados en nuestra base de datos.

- **Staged:** En esta parte marcamos nuestros archivos modificados dejándolos listos para confirmarlos.


### ¿Qué es un Sistema de Control de Versiones? ###

Un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo. Este tipo de sistemas nos permiten volver en el tiempo y salvar nuestro trabajo. <br>

**Los tipos de sistemas de control son:**

**Local Computer:** Solo vive en nuestro computador. <br>
**Centralizado:** No depende únicamente de un computador en el que se trabaja, sino que depende del súper servidor en donde se almacena la información. El servidor provee las copias a sus hijos, pero solo guarda los cambios en un solo lugar. <br>
**Sistema de control distribuidos:** Cada uno de los que participan en el proyecto, tienen copia del proyecto que se realiza, por eso no dependemos de un solo computador que almacene toda la información.

> Git es un Sistema de Control de Versiones Distribuido.


### Los tres estados de Git ###

**Working Directory:** Es al lugar donde se trabajan los archivos. <br>
**Staging Area:** Es el área de preparación de los archivos que serán registrados en el repositorio. <br>
**Git Repository:** Es el lugar donde se almacena el código de forma segura.


### Comandos de Git ###

**git init:** Nos crea un repositorio de manera local y lo hará en la carpeta donde estamos posicionados o se le puede pasar ***[nombre_carpeta]*** y creará la carpeta con ese nombre.

**git status:** Muestra el estado de los archivos y directorios, los que estén en *verde* se encuentran en el *Staging Area* y los que estén *rojo* se encuentran en el *Working Directory*.

**git add [file or directory]:** Agregar un archivo o una carpeta al *Staging Area*.

**git add -A:** Agregar todos los *untracked files* al *Staging Area*

**git add .:** Agregar todos los *untracked files* al *Staging Area*

**git rm --cached [file or directory]:** Elimina un archivo o carpeta del *Staging Area* y lo deja en el *Working Directory*.

**git rm -f [file or directory]:** Fuerza la eliminación de un archivo o carpeta del *Staging Area* y del *Working Directory*.

**git checkout [file or directory]:** Revierte los cambios en un archivo o directorio dentro del *Working Directory*.

> **Untracked files:** Son archivos que están en nuestro *Working Directory*



### Enlaces de interes ###

[Emulador de terminal para Windows](http://cmder.net/)