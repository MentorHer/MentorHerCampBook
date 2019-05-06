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

Como pueden ver en la imagen estan los últimos comandos utilizados y al ejecutar **git status** nos muestra que hemos modificado el archivo **README.txt** y que no estamos haciendo seguimiento al archivo **mentorher** que creamos con el comando **touch mentorher** ya que es nuevo.

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

Ahora quiero enseñarles como **corregir** o **modificar** un **commit**, pero antes de hacerlo quiero aclarar que esto solo es recomendable hacer si es que lo que queremos **corregir** o **modificar** esta justo en el **commit anterior** y no así si ya se hicieron varios **commits** y recien se dan cuenta de un **error** en un **commit** que hicieron por ejemplo hace unos tres **commits** atras, en ese caso es mejor corregirlo y hacer un **nuevo commit**.

Aclarado esto vamos empezar, como se muestra en esta última imagen vemos 2 commits, supongamos que queremos corregir algo de nuestro último commit que es el de **modificaciones**, lo que vamos a hacer es copiar todo el codigo que esta despues de la palabra **commit**, en este caso es **"c97fa.....e166"**

Y luego vamos a ir a la consola y ejecutar el siguiente comando, este comando es el **reset** pero tiene dos formas por asi decirlo de usar uno es el **soft** en este caso nos va a devolver al commit que estamos diciendo pero a la vez nos devolvera los cambios que realizamos y los dejara en el área de stage y el otro es el **hard** que te devuelve al commit que le estamos diciendo que nos lleve pero a la vez va a eliminar todos los cambios que se realizaron, es decir nos llevara al commit pero no tendra ningún cambio a partir de ahi. En este ejemplo vamos a utilizar el comando **soft** como esta a continuacion:

```git reset --soft c97fa12a066e91b60984e3c947b848a0fba3e166```

Ahora podremos modificar y realizar los cambios que necesitemos y cuando vayamos a hacer commit utilizaremos un nuevo comando para que el commit se haga al ultimo commit que hicimos y podemos usar el siguiente comando:

``` git commit --amend -m "Comentario"```

Con esto los cambios se guardaran en el último **commit** con el comentario que le demos. Y así podemos modificar o cambiar algun commit pero como dije solo si es el inmediato anterior.

Hasta aquí lo unico que hicimos es hacer repositorios de manera local, ahora les enseñare a hacer un repositorio remoto con la ayuda de **github**, lo primero que haremos es crearnos una cuenta en: [Github](https://github.com).

Siguen los pasos para crearse una cuenta en GitHub tienen que verificar el correo electrónico con el que crearon la cuenta y luego inician sesión, cuando inicien sesión les tendria que aparecer una ventana como la siguiente: 

![github][github]

[github]: http://i67.tinypic.com/xmk51z.png

Como pueden ver en la imagen en el lado izquierdo estan todos los proyectos que en este caso mi cuenta esta realizando el control de versiones.

Ahora para enlazar lo que anteriormente les enseñe que era git para ahora eso subirlo a github lo primero que tenemos que hacer es crear un nuevo repositorio es decir vamos a hacer click en el boton verde que dice **New** o si lo tienen en español dira **Nuevo** y les mostrará una imagen como la siguiente:

![mentor][mentor]

[mentor]: http://i67.tinypic.com/2rwxk6w.png

Como pueden ver en la imagen les pide un nombre para su repositorio en este ejemplo estoy colocando como nombre **MentorHer** y también se puede elegir entre un repositorio **público**, es decir que todos van a poder ver el repositorio y todos los commits del mismo o también elegir **privado** que solo el dueño del repositorio y los que él quiera podrán ver el repositorio, en este ejemplo dejaremos como **público** y damos click en **Crear repositorio** nos mostraría una imagen como la siguiente:

![mentor1][mentor1]

[mentor1]: http://i68.tinypic.com/2nvqt0x.png

Ahora ¿se acuerdan cuando hicimos **git init**? cuando hagamos eso en un directorio es decir en un proyecto  para estar usando **git** y ese mismo poder enlazar con **github** tenemos que usar los codigos que nos muestra en la anterior imagen que son: 

```git remote add origin https://github.com/elchapako/MentorHer.git```

```git push -u origin master ```

En este momento ya tendriamos configurado nuestro proyecto para hacer commits a **github**

¿Y como hacemos el commit a **github**?

Pues muy facil, se acuerdan que llegamos hasta hacer:

``` git commit -m "modificaciones" ```

Este es un ejemplo de hasta donde llegamos, es decir hacemos commit y ya habiamos creado un repositorio en **git** para ese mismo repositorio tenerlo en **github** solo se tiene que hacer el siguiente paso:

``` git push origin master ```

Y listo ya subieron ese repositorio a **github** al repositorio que hemos creado para este ejemplo es **MentorHer**.

Así con esto terminamos con lo básico que necesitan saber de **git** y **github**.


   

