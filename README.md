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

**git commit -m ["mensaje"]:** Nos permite confirmar los cambios realizados.

**git commit -m ["mensaje"] --amend:** Nos permite concatenar nuevos cambios al último y también podemos cambiar el mensaje de dicho *commit* si así lo deseamos.

**git log:** Nos permite ver el historial de todos los *commits*.

**git tag:** Sirve para etiquetar confirmaciones.


> **Untracked files:** Son archivos que están en nuestro *Working Directory*


<br><br>

### Notas y ejemplos ###

**git add:** <br>
![git add](images/git-add.jpg)

**git tag:**

`git tag -a [1.x] -m "[descripcion]"` Registra un tag. <br>
`git tag -l` Lista los tags existentes. <br>
`git tag [1.x] [HASH commit]` Agrega un tag a un **commit** en especifico por medio de su **HASH.** <br>
`git tag -f -a [1.x] -m "[description...]" [Commit HASH]` Permite renombrar un tag. <br>
`git tag -d [1.x]` Elimina un tag.

**Alias - git superlog**

`git config --global alias.superlog "log --graph --abbrev-commit --decorate --date=relative --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"`


<br><br>

### Enlaces de interes ###

[Emulador de terminal para Windows](http://cmder.net/) <br>
[Empezando con GIT](https://git-scm.com/book/es/v1/Empezando) <br>
[Documentation GIT](https://git-scm.com/doc) <br>
[Reference GIT](https://git-scm.com/docs) <br>
