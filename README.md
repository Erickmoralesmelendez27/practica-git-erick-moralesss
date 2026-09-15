Práctica de Git y GitHub

Datos del estudiante

Nombre completo: Erick Morales Melendez

Matrícula: 2630308

Nombre de la práctica: Creación y sincronización de un repositorio Git con GitHub



Objetivo de la práctica

El objetivo de esta práctica es aprender a crear un repositorio local utilizando Git, registrar cambios mediante commits, vincular el repositorio local con un repositorio remoto en GitHub y sincronizar información en ambos sentidos.

Durante la práctica se trabajó con el flujo de cambios desde el repositorio local hacia GitHub y también desde GitHub hacia el repositorio local.



Descripción del procedimiento realizado

Primero se creó una carpeta llamada practica-git-erick-morales y se abrió PowerShell dentro de ella. Se inicio un repositorio Git utilizando git init.



Después se configuró la rama principal con el nombre main y se crearon los archivos README.md y datos.txt. En datos.txt se agregó un texto inicial relacionado con la práctica.



Luego se revisó el estado del repositorio utilizando git status. Los archivos fueron agregados al área mediante git add . y finalmente se creó el primer commit utilizando git commit.



Después se creó un repositorio público en GitHub con el mismo nombre del repositorio local. El repositorio de GitHub se dejó vacío para que los archivos fueran enviados inicialmente desde la computadora.



El repositorio local se vinculó con GitHub mediante el comando git remote add origin. Después se utilizó git push -u origin main para enviar los archivos locales al repositorio remoto.





Comandos de Git utilizados

git init

Crea un repositorio Git dentro de la carpeta actual. A partir de este momento Git comienza a controlar las versiones de los archivos o archivo del proyecto.



git branch -M main

Hace el nombre de la rama principal como main.



git status

Muestra el estado actual del repositorio. Permite saber qué archivos fueron modificados, cuáles están preparados para un commit y cuáles todavía no han sido registrados.



git add .

Agrega los archivos y cambios al área de preparación o Staging Area. Esto indica a Git qué cambios queremos incluir en el siguiente commit.



git commit -m "Primer commit"

Crea un punto de control en el historial del repositorio con los cambios que se encontraban en el Staging Area.



git remote add origin URL

Vincula el repositorio local con un repositorio remoto de GitHub. origin es el nombre utilizado normalmente para identificar el repositorio remoto principal.



git remote -v

Muestra las direcciones del repositorio remoto configurado y permite comprobar que la conexión con GitHub se realizó correctamente.



git push -u origin main

Envía los commits de la rama main desde el repositorio local hacia GitHub. La opción -u establece la relación entre la rama local y la rama remota para facilitar futuros push y pull.



git pull origin main

Descarga los cambios realizados en el repositorio remoto y los integra en el repositorio local.



Creación del repositorio local

El repositorio local se creó mediante una carpeta llamada practica-git-nombre-apellido. Dentro de esta carpeta se ejecutó git init, con lo cual Git creó la estructura necesaria para comenzar a controlar las versiones del proyecto.



Después se creó la rama principal llamada main, se agregaron los archivos necesarios y se realizó el primer commit.



Vinculación del repositorio local con GitHub

Se creó un repositorio público en GitHub utilizando el mismo nombre que el repositorio local.



Al crear el repositorio remoto no se agregaron automáticamente archivos como README, .gitignore o licencia, ya que los archivos iniciales debían provenir del repositorio local.



Posteriormente se utilizó git remote add origin para establecer la conexión entre el repositorio local y el repositorio de GitHub.



Sincronización Local → GitHub

Para comprobar la sincronización desde el repositorio local hacia GitHub, primero se creó un commit con los archivos iniciales.



Después se utilizó:



git push -u origin main



Este comando envió los commits y archivos del repositorio local hacia GitHub. Al actualizar la página del repositorio fue posible comprobar que README.md y datos.txt aparecieron en GitHub.



Sincronización GitHub → Local

Para comprobar el flujo contrario, se modificó directamente el archivo datos.txt desde la página de GitHub.



Se agregó la siguiente línea:



Este archivo fue modificado desde GitHub.



Después de realizar el commit en GitHub, desde PowerShell se ejecutó:



git pull origin main



Este comando descargó los cambios realizados en GitHub y los incorporó al repositorio local.



Al abrir nuevamente datos.txt se pudo comprobar que el cambio realizado desde GitHub también estaba disponible en la computadora.



Segundo cambio desde el repositorio local

Después de comprobar el funcionamiento de git pull, se modificó nuevamente datos.txt desde la computadora.



Se agregó la siguiente línea:



Este archivo fue modificado desde el repositorio local.



Posteriormente se comprobó el estado del repositorio con git status, se agregaron los cambios con git add ., se creó un nuevo commit y finalmente se enviaron los cambios a GitHub utilizando git push.



Archivos contenidos en el repositorio

README.md

Contiene la documentación de la práctica, incluyendo los objetivos, procedimiento, comandos utilizados y explicación del funcionamiento de Git y GitHub.



datos.txt

Contiene información relacionada con la práctica y se utilizó para comprobar la sincronización de cambios entre GitHub y el repositorio local.



Flujo de trabajo utilizado

El flujo general utilizado durante la práctica fue:



Working Directory → Staging Area → Local Repository → GitHub



Los cambios se realizaron inicialmente en los archivos del proyecto. Después se agregaron al Staging Area mediante git add, se registraron en el repositorio local mediante git commit y finalmente se enviaron a GitHub mediante git push.



Para obtener cambios realizados en GitHub se utilizó git pull, permitiendo sincronizar nuevamente el repositorio local.



Conclusión

Esta práctica permitió comprender el funcionamiento básico de Git y GitHub y la diferencia entre un repositorio local y uno remoto. También permitió practicar el uso del Staging Area, los commits y los comandos push y pull.



Se comprobó que los cambios pueden enviarse desde la computadora hacia GitHub mediante git push y también pueden descargarse desde GitHub hacia la computadora mediante git pull.



El ejercicio ayudó a comprender la importancia del control de versiones para mantener un historial de los cambios realizados en un proyecto y trabajar de manera organizada con repositorios remotos
