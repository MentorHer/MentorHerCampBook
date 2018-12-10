# Primeros pasos con [Github](https://github.com)

En esta lección aprenderas como usar github pero primero te explicare que es git.

En el desarrollo web o cualquier tipo de desarrollo en general, uno de los probemas que tenemos en comun es el control del desarrollo que estamos realizando.
 
Muchos de nosotros seguramente tuvimos varios directorios que se llamaban por ejemplo: **Proyecto final**, **Proyecto final de verdad**, etc.

Esto con el fin de tener un **historial** de los cambios que hemos realizado a nuestro proyecto.

Incluso algunas veces seguro hemos querido llorar por un archivo que se nos **pierde** y era muy **importante** para el desarrollo.

Estos problemas se  resuelven al usar un **controlador de versiones** y es en eso que **GIT** nos ayuda a simpligicarnos la vida.

Lo primero que tenemos que hacer es instalar git en nuestro ordenador.

Iniciamos ejecutando el sigiente comando en consola para saber si ya tenemos instalado git:

``` git --version ```

Si lo tendrían instalado les saldría un mensaje como el siguiente:

![Git version][git]

[git]: http://i65.tinypic.com/34j2npc.png

Si es el caso que no tendrían instalado vamos a ir a la web de git para instalarlo según el **sistema operativo** de nuestro ordenador.

[Click aqui para ir a GIT](https://git-scm.com)

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

Como puedes ver en esta página nos explica como poder instalar git según el **Sistepa Operativo** que tengamos.

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

Y por último para usuarios de windows solo descargan el instalador y ejecutenlo para tenerlo instalado.

[Descargar git para windows](https://git-scm.com/download/win)

Cuando terminemos de instalar simplemente nos vamos a la consola y vamos a correr el siguiente comando:

``` git ```

Al hacer eso nos mostrará un listado de comandos que puedes usar con git como muestra la siguiente imagen:

![Lista de comandos en git][list]

[list]: http://i64.tinypic.com/b5oehd.png

Y el primer comando que vamos a ver es el siguiente a pesar que en esa lista no se muestra por default:

``` git config ```

Este parametro nos permite establecer los datos de configuracion que vamos a utilizar para nuestros proyectos. Y lo primero que tenemos q hacer es indicarle a git cual es nuestro nombre y nuestro correo electronico, esto lo hacemos con el siguiente comando:

``` git config --global user.name "Edwin Ibañez" ```

En este caso estoy diciendole a git que quiero hacer la configuración de manera global para no tener que indicar mi nombre cada vez que estoy trabajando en un proyecto. De la misma manera agregaré mi correo:

``` git config --global user.email "edwin.ibanez@tooducks.com ```

Ya que hayamos hecho esto vamos a comenzar a trabajar con **GIT**.
Para esto tenemos que crear un repositorio, un repositorio en terminos muy simples es un lugar en el que se guardan ciertas cosas, en nuestro caso el **codigo**.
Para crear el repositorio debemos primero tener un directorio, así que vamos a crearlo:

``` mkdir MentorHer ```

Luego entramos a ese directorio:

``` cd MentorHer ```

 Y vamos a ejecutar:
 
``` git init ```

Esto nos va a crear un repositorio local en nuestra computadora y nos va a generar una carpeta oculta llamada **.git** que es donde se guardara toda la información referente a los cambios que estamos realizando a nuestro proyecto, ustedes nunca van a tener que entrar ahí pero es bueno que sepan donde se guarda.