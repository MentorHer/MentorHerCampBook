# Graficando con Python
Entre las librerias mas populares de Python tenemos a:

###Matplotlib###
Nos permite graficar desde histogramas hasta graficas lineales y mapas de calor. Tiene un soporte completo a graficas 2D y un soporte limitado a graficas 3D. 

###Seaborn###
Esta libreria nos permite crear graficas estadisticas atractivas e informativas.  Esta basado en matplotlib. Su objetivo es hacer de las visualizaciones un parte central de la exploracion de datos y nos permite crear visualizaciones mas complejas.

Lo primero que tenemos que hacer es importar alguna de las librarias:
![Importando Matplotlib][matplotlib]{: width=150 height=100 style="float:right; padding:16px"}
[matplotlib]: https://farm5.staticflickr.com/4867/31878128527_0250445bbc_b.jpg 


El primer tipo de grafica que veremos sera:

###Graficas Lineales###

Generalmente se usa para presentar observaciones recolectadas en intervalos regulares. En el eje x se representa el intervalo regular, como el tiempo. En el eje y mostramos las observaciones, ordenadas por el eje x y conectadas por una linea.

![Linear Plot] (https://farm8.staticflickr.com/7810/31878167537_3d3f52c009_b.jpg) 

Esta linea se crea llamando a la funcion ```plot()``` que recibe dos parametros: Los datos para el eje x que contiene los intervalos regulares y las observaciones para el eje y. 
Este tipo de graficos son bastante utiles para presentar series de tiempo y secuencias de datos donde hay una orden entre las observaciones. 

Al ejecutar el ejemplo se crea un diagrama de líneas que muestra el patrón de onda sinusoidal en el eje y a lo largo del eje x con un intervalo constante entre las observaciones.
