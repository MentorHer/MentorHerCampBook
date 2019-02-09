# Librerías

Ya sabes como funciona Python, cuáles son algunos de sus usos, cómo escribir un programa básico y como ejecutarlo!

Ahora vamos a aprender un poco más sobre las diferentes herramientas y contigo que Python utiliza, estas son las librerías, que en realidad son un código escrito en Python que puede ser reutilizado por otro programador.

Por ejemplo:

### NumPy

Permite hacer computación científica con Python, por ejemplo:

* funciones de álgebra lineal
* funcionalidades de trabajo con números aleatorios
* trabajos con grupos (arreglos) "array de objetos"

Referencia: http://www.numpy.org

Es necesario instalarlo, de la siguiente manera desde la línea de comando:
>> $ pip install numpy

Para incluirlo en tu código con Python y poder trabajar con sus funcionalidades, escribe en tu archivo:
```python
import numpy as np
```

Ejemplo de uso (matrices):
>>> a = np.arange(15).reshape(3, 5)
>>> a
array([[ 0,  1,  2,  3,  4],
       [ 5,  6,  7,  8,  9],
       [10, 11, 12, 13, 14]])


### SciPy

Es la herramienta de Python, de software libre para matemáticas, ciencia e ingeniería.

Referencia: https://www.scipy.org


### Matplotlib

Permite generar gráficos en 2D de los datos de nuestro código Python.

Referencia: https://matplotlib.org

Para incluirlo en tu código con Python y poder trabajar con sus funcionalidades, escribe en tu archivo:
```python
import matplotlib.pyplot as plt
```

Ejemplo:

```python
import numpy as np
import matplotlib.pyplot as plt

# valores de 'x' y 'y' para generar una curva de la función seno
x = np.arange(0, 3 * np.pi, 0.1)
y = np.sin(x)

#  graficar los puntos con la matplotlib
plt.plot(x, y)
plt.show()  # así mostramos la gráfica generada
```

![Gráfica generada con Matplotlib](sine.png)




Otras librerías que nos servirán para que puedas trabajar con datos son:

### Pandas

Pandas es una librería de Python destinada al análisis de datos, que proporciona unas estructuras de datos flexibles y que permiten trabajar con ellos de forma muy eficiente.

Es necesario instalarlo, de la siguiente manera desde la línea de comando:
>> $ pip install pandas

Para incluirlo en tu código, debes importarlo a tu archivo, así:

```python
import pandas as pd
```

Más detalles del uso de estas librerías, más adelante.
