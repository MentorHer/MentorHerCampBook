# Primeros pasos con [Github](https://github.com)

En esta lección aprenderás como usar github pero primero te explicaré que es git.

En el desarrollo Web o cualquier tipo de desarrollo en general, uno de los problemas que tenemos en común es el control del desarrollo que estamos realizando.
 
Muchos de nosotros seguramente tuvimos varios directorios que se llamaban por ejemplo: **Proyecto final**, **Proyecto final de verdad**, etc.

Esto con el fin de tener un **historial** de los cambios que hemos realizado a nuestro proyecto.

Incluso algunas veces seguro hemos querido llorar por un archivo que se nos **pierde** y era muy **importante** para el desarrollo.

Estos problemas se  resuelven al usar un **controlador de versiones** y es en eso que **GIT** nos ayuda a simplificarnos la vida.

Lo primero que tenemos que hacer es instalar git en nuestro ordenador.

Iniciamos ejecutando el siguiente comando en consola para saber si ya tenemos instalado git:

``` git --version ```

Si lo tendrían instalado les saldría un mensaje como el siguiente:

![Git version][git]

[git]: http://i65.tinypic.com/34j2npc.png

Si es el caso que no tendrían instalado vamos a ir a la Web de git para instalarlo según el **sistema operativo** de nuestro ordenador.

[Click aquí para ir a GIT](https://git-scm.com)

Tendría que mostrarles la siguiente página:

![Home git][home]

[home]: http://i68.tinypic.com/2ry21z5.png 

Estando ahí vamos a hacer click en **Documentatión**, como indica la imagen.

Nos mostrará la siguiente página:

![Documentation][doc]

[doc]: http://i68.tinypic.com/2w684sh.png

Estando ahí vamos a hacer click en **Book**, como indica la imagen.

Nos mostrará la siguiente página:

![Book][book]

[book]: http://i65.tinypic.com/2w562k7.png

Y por último vamos a hacer click en **Installing Git**, como indica la imagen.

Nos mostrará la siguiente página:

![Installing Git][Install]

[Install]: http://i64.tinypic.com/2i1l3yt.png

Como puedes ver en esta página nos explica como poder instalar git según el **Sistema Operativo** que tengamos.

Para los usuarios que usen **Linux** tanto en distribución basadas en red hat como es **fedora**:

``` sudo dnf install git-all ```

como en distribución basadas en Debian como es **Ubuntu**:

``` sudo apt install git-all ```

También para instalar en una **Mac** primeramente tenemos que tener instalado **Xcode Command Line Tools** y eso lo podemos lograr descargando **Xcode** desde la **AppStore**.

Luego de eso se puede instalar de dos maneras ya sea descargando el instalador: 

[Git para MAC](https://git-scm.com/download/mac)

O por medio de Homebrew que es el más utilizado, primero instalando homebrew ejecutando en la terminal el siguiente comando:

``` /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" ```

Luego de tener instalado Homebrew solo ejecutamos el siguiente comando:

``` brew install git ```

y listo ya tenemos **git** en nuestra **mac**

Y por último para usuarios de Windows solo descargan el instalador y ejecútenlo para tenerlo instalado.

[Descargar git para Windows](https://git-scm.com/download/win)

Cuando terminemos de instalar simplemente nos vamos a la consola y vamos a correr el siguiente comando:

``` git ```

Al hacer eso nos mostrará un listado de comandos que puedes usar con git como muestra la siguiente imagen:

![Lista de comandos en git][list]

[list]: http://i64.tinypic.com/b5oehd.png

Y el primer comando que vamos a ver es el siguiente a pesar que en esa lista no se muestra por default:

``` git config ```

Este parámetro nos permite establecer los datos de configuración que vamos a utilizar para nuestros proyectos. Y lo primero que tenemos q hacer es indicarle a git cual es nuestro nombre y nuestro correo electrónico, esto lo hacemos con el siguiente comando:

``` git config --global user.name "Edwin Ibañez" ```

En este caso estoy diciéndole a git que quiero hacer la configuración de manera global para no tener que indicar mi nombre cada vez que estoy trabajando en un proyecto. De la misma manera agregaré mi correo:

``` git config --global user.email "edwin.ibanez@tooducks.com ```

Ya que hayamos hecho esto vamos a comenzar a trabajar con **GIT**.
Para esto tenemos que crear un repositorio, un repositorio en términos muy simples es un lugar en el que se guardan ciertas cosas, en nuestro caso el **código**.
Para crear el repositorio debemos primero tener un directorio, así que vamos a crearlo:

``` mkdir MentorHer ```

Luego entramos a ese directorio:

``` cd MentorHer ```

 Y vamos a ejecutar:
 
``` git init ```

Esto nos va a crear un repositorio local en nuestra computadora y nos va a generar una carpeta oculta llamada **.git** que es donde se guardara toda la información referente a los cambios que estamos realizando a nuestro proyecto, ustedes nunca van a tener que entrar ahí pero es bueno que sepan donde se guarda.

Este directorio es donde se almacenará nuestro proyecto ahí estará almacenado todo nuestro código, vamos a hacer un ejemplo de la creación de un documento en nuestro directorio ejecutando el siguiente comando:

``` echo "Mentor Her" >> README.txt ```

Y luego vamos a ejecutar el siguiente comando para ver como se encuentra nuestro repositorio:

``` git status ```

Nos mostrará la siguiente imagen:

![Git Status][status]

[status]: http://i63.tinypic.com/2074w3m.jpg

Aqui podemos ver que detecto un archivo nuevo que no esta teniendo seguimiento, lo vamos a agregar al stage ejecutando el siguiente comando:

``` git add README.txt ```

Y si ejecutamos de nuevo:

``` git status ```

Nos mostrará la siguiente imagen:

![Status][again]

[again]: http://i66.tinypic.com/2dlp5sm.png

En este punto veremos que nuestro archivo cambio a verde, esto significa que ya estamos empezando a tener seguimiento de este archivo y por último hacemos un commit con el comando:

``` git commit -m "Crear archivo README.txt" ```

Lo que esta entre comillas es un comentario de porque estamos registrando este cambio.
Ejecutando ese comando nos mostrará la siguiente imagen:

![commit][commit]

[commit]: http://i67.tinypic.com/2wgrp1s.png

Si Ejecutamos de nuevo el siguiente comando: 

``` git status ```

Y nos mostrará la siguiente imagen:

![commit1][commit1]

[commit1]: http://i68.tinypic.com/kbovn4.png

En la imagen como vemos nos dice que estamos sobre el branch master, este es el branch por defecto donde trabajamos nuestro proyecto, se pueden crear más pero en este caso no será necesario y también podemos ver que no tenemos nada para hacer commit, sin embargo para seguir con la prueba ejecutamos el siguiente comando:

``` sudo nano README.txt ```

Se abrirá el editor de texto con nuestro archivo **README.txt** modificamos por ejemplo como esta en la siguiente imagen:

![editar][editar]

[editar]: http://i68.tinypic.com/hsq3wx.png

Guardamos este archivo que acabamos de editar. Y vamos a ejecutar el siguiente comando:

``` touch mentorher ```

Este comando lo que hace es crear un archivo llamado mentorher, ahora ejecutamos nuevamente:

``` git status ```

Nos mostrará la siguiente imagen:

![editar2][editar2]

[editar2]: http://i66.tinypic.com/sfxr9u.png

Como pueden ver en la imagen estan los últimos comandos utilizados y al ejecutar **git status** nos muestra que hemos modificado el archivo **README.txt** y que no estamos haciendo seguimiento al archivo mentorher que creamos con el comando **touch mentorher** ya que es nuevo.

Para añadirlos al stage podemos ejecutar:

``` git add README.txt mentorher ```

Así añadimos todos los archivos, pero tambien se puede ejecutar:

``` git add . ``` o ``` git add --all ```

Esto agregará todo al stage, luego ejecutamos: 

``` git commit -m "modificaciones" ```

Y ya tendriamos nuestros dos archivos en nuestro timeline como muestra la siguiente imagen:

![editar3][editar3]

[editar3]: http://i67.tinypic.com/2mfdo2f.png

En este momento tenemos 2 commits que hemos generado, pero ahora ¿cómo podemos ver esos commits? para esto vamos a hacer uso del comando: 

``` git log ```

Nos mostrará la siguiente imagen:

![editar4][editar4]

[editar4]: http://i64.tinypic.com/23shmbk.png

Ahí nos muestra cada uno de los **commits** que hayamos hecho, quién los hizo, cuando y de que consta el **commit**, si se trabajaría en proyectos de gran magnitud los comentarios son de gran ayuda, ya que nos diran de que consta el **commit** en ese punto. Así que traten de ser los más claros y descriptivos cuando hagan sus **commits**.

