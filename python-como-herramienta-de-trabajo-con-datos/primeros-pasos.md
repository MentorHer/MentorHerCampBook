# Primeros pasos en Python

A continuacion te presentamos Python como lenguaje de programacion. En este apartado aprenderas:
- Que es python
- Como se instala
- Caracteristicas 
- Diferencias en relacion a otros lenguajes
- Entender y ejecutar código

## 1. Que es python

Python es un lenguaje de programación interpretado cuya filosofía prioriza la escritura de código legible.
La principal diferencia entre un lenguaje compilado y uno interpretado es que el lenguaje compilado requiere un paso adicional antes de ser ejecutado, la compilación, que convierte el código que escribes a lenguaje de máquina. Un lenguaje interpretado, por otro lado, es convertido a lenguaje de máquina a medida que es ejecutado.
Ejemplos de lenguajes compilados incluyen C, C++, Java, Go y Rust, entre muchos otros. Ejemplos de lenguajes interpretados incluyen Ruby, Python y JavaScript, entre muchos otros. A todos estos lenguajes se les conoce como lenguajes de alto nivel.
El nombre del lenguaje proviene de la afición de su creador original, Guido van Rossum, por los humoristas británicos Monty Python. El principal objetivo que persigue este lenguaje es la facilidad, tanto de lectura, como de diseño.

## 2. Instalación
## 3. Características 
Python es un lenguaje de programación multiparadigma. Esto significa que más que forzar a los programadores a adoptar un estilo particular de programación, permite varios estilos: programación orientada a objetos, programación imperativa y programación funcional.
Alguna de las más destacadas es el empleo del indentado (tabulaciones) para definir bloques de código en condicionales y bucles, y el uso avanzado que hace de vectores, listas, y textos.

## 4. Usos 
## 5. Diferencias en relacion a otros lenguajes
A diferencia de los programadores de C, C# o incluso de PHP, aquella gente que ha estado llegando a Python, --como la mayoría que llega a Perl y a Ruby-- lo ha hecho porque disfrutan de programar y buscan un lenguaje que les facilite hacer mejor algo que les gusta. Este lenguaje recoge lo mejor de otros y es reconocido porque es muy limpio y legible, lo que facilita mucho la tarea de los programadores.

## 6. Diferencias entre python 2 y 3
## 7. Ejemplos de codigo y su interpretación
A continuación se veran algunos ejemplos de código sencillos para ir interiorizandonos con python.
Se veran tópicos mas detallados en los siguientes capitulos pero a continuación se detallan algunos ejemplos básicos.
Cabe recalcar que el resto de los ejemplos se trabajaran con la version 3 de python.

Para imprimir un número o texto en pantalla, usamos la función Print
```python
print('Hola mundo')
```
Para recibir un texto por el usuario, empleamos la función Input
```python
nombre=input('Introduce tu nombre: ')
```
Si queremos recibir un número, tenemos que convertirlo con la función Int
```python
edad = int(input('Introduce tu edad: '))
```
Las estructuras condicionales se realizan de forma similar a casi todos los lenguajes de programación. Por ejemplo, el siguiente código recibe un número, y dice si es par o impar.
```python
### Introducir un numero por teclado y decir si es par o impar
num = int(input('Introduzca un numero: '))
if num % 2 == 0:
    print('Par')
else:
    print('Impar')
```
El bucle de tipo for si tiene ciertas particularidades. El siguiente ejemplo, muestra como imprimir en pantalla los 10 primeros números
```python
### Ejemplo for, imprime los 10 primeros numeros en una linea
for i in range(10):
    print(i, end=" ") #imprimir numero, sin salto linea
    print() #lineavacia
```
Por su parte, un “equivalente” a un bucle de tipo foreach tendría la siguiente forma.
```python
###Ejemplo foreach, imprime los numeros de la lista del 1 al 4
for i in [1, 2, 3, 4]:
    print(i, end=" ") #imprimir numero, sin salto linea
    print() #lineavacia
```
Si ejecutamos el código en una cadena, se ejecuta la acción para cada letra
```python
### Ejemplo foreach, imprime las letras MENTORHER
for i in "MENTORHER":
    print(i)
```
El bucle while se ejecutaría de la siguiente forma
```python
### Ejemplo while, imprime los primeros 10 numeros
i = 1
while i <= 10:
    print(i)
    i += 1
```
Por último para definir una función usamos la palabra reservada Def. El siguiente ejemplo define una función que calcula el máximo de dos números, y cómo usarla para calcular el máximo entre 20 y 30.
```python
### Ejemplo de función
def max (a, b):
    if a < b:
        return b
    elif b < a:
        return a
    else:
        return a
```
Y para llamar a la función creada ejecutamos:
```python
print(max(20, 30))
```
## 8. Ejecución de código
## 9. Entornos de trabajo (IDE)
Existen varios IDEs para programar con python, entre los cuales los mas relevantes son:
* PyCharm https://www.jetbrains.com/pycharm
* Eclipse + PyDev http://www.pydev.org
* Sublime Text https://www.sublimetext.com
* Atom https://atom.io/
* Visual Studio Code https://code.visualstudio.com/

## 10. Referencias - Documentación importante
