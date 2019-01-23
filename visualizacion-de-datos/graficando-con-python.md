# Graficando con Python
Entre las librerias mas populares de Python tenemos a:

###Matplotlib###
Nos permite graficar desde histogramas hasta graficas lineales y mapas de calor. Tiene un soporte completo a graficas 2D y un soporte limitado a graficas 3D. 

###Seaborn###
Esta libreria nos permite crear graficas estadisticas atractivas e informativas.  Esta basado en matplotlib. Su objetivo es hacer de las visualizaciones un parte central de la exploracion de datos y nos permite crear visualizaciones mas complejas.

Lo primero que tenemos que hacer es importar alguna de las librerias:

<img src="https://farm5.staticflickr.com/4867/31878128527_0250445bbc_b.jpg" style="width: 85%; height: 85%">

El primer tipo de grafica que veremos sera:

###Graficas Lineales###

Generalmente se usa para presentar observaciones recolectadas en intervalos regulares. En el eje x se representa el intervalo regular, como el tiempo. En el eje y mostramos las observaciones, ordenadas por el eje x y conectadas por una linea.

<img src="https://farm8.staticflickr.com/7810/31878167537_3d3f52c009_b.jpg" style="width: 80%; height: 80%">

Esta linea se crea llamando a la funcion ```plot()``` que recibe dos parametros: Los datos para el eje x que contiene los intervalos regulares y las observaciones para el eje y. 
Este tipo de graficos son bastante utiles para presentar series de tiempo y secuencias de datos donde hay una orden entre las observaciones. 

Al ejecutar el ejemplo se crea un diagrama de líneas que muestra el patrón de onda sinusoidal en el eje y a lo largo del eje x con un intervalo constante entre las observaciones.

###Bar Chart###

Este grafico generalmente se usa para presentar cantidades relativas para categorias multiples.

El eje x representa las categorías y están espaciadas uniformemente. El eje y representa la cantidad para cada categoría y se dibuja como una barra desde la línea de base hasta el nivel apropiado en el eje y.

Se puede crear un gráfico de barras llamando a la función ```bar()``` y pasando los nombres de las categorías para el eje x y las cantidades para el eje y.

<img src="https://farm8.staticflickr.com/7853/46844934851_bc61e9b1c8_b.jpg" style="width: 80%; height: 80%">

Un grafico de barras puede ser util para comparar multiples cantidades de puntos o estimaciones.

En el ejemplo anterior se crea un set de datos con tres categorias, cada una definida con una etiqueta. Se dibuja un único valor entero aleatorio para la cantidad en cada categoría.
