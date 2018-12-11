# Formatos de datos
## Retroalimentacion:
Los  **datos**  son representaciones simbólicas (vale decir: numéricas, alfabéticas, algorítmicas, etc.) de un determinado atributo o variable cualitativa o cuantitativa, o sea: la descripción codificada de un hecho empírico, un suceso, una entidad.
Los  **datos** son, así, la información (valores o referentes) que recibe el computador a través de distintos medios, y que es manipulada mediante el procesamiento de los algoritmos de programación. Su contenido puede ser prácticamente cualquiera: estadísticas, números, descriptores, que por separado no tienen relevancia para los usuarios del sistema, pero que en conjunto pueden ser interpretados para obtener una información completa y específica.  

Algunos tipos de datos son:

-   **Caracteres**. Dígitos individuales que se pueden representar mediante datos numéricos (0-9), letras (a-z) u otros símbolos.
-   **Caracteres unicode**. Unicode es un estándar de codificación que permite representar más eficazmente los datos, permitiendo así hasta 65535 caracteres diferentes.
-   **Numéricos**. Pueden ser números reales o enteros, dependiendo de lo necesario.
-   **Booleanos**. Representan valores lógicos (verdadero o falso).

Fuente:  [https://concepto.de/dato-en-informatica/#ixzz5ZPESoV9T](https://concepto.de/dato-en-informatica/#ixzz5ZPESoV9T)
## 1. La importancia de los Formatos de Datos
Seamos honestos: tus datos no sirven de nada si no están disponibles en un formato en que los puedas usar. Hasta las visualizaciones, aplicaciones interactivas y análisis más sencillos requieren que los datos sean legibles en algún lenguaje de computadora. Para que los datos puedan ser usados, deben ser legibles en diferentes formatos.
Los datos deben ser abiertos y estar disponibles en un formato que sea legible para cualquier computadora; así se asegura que la información pueda ser procesada con la mínima intervención humana. Si tus datos cumplen con estas características, serán accesibles para cualquier persona y cualquiera los podrá procesar y usar.
## Datos legibles
El término se refiere a que la información esté en un formato o formatos que sean legibles y, por lo tanto, totalmente transparentes. Si los datos no son legibles, los usuarios tendrán que armar un documento desde cero para crear una estructura legible. ¡Esto no es recomendable!

Los datos que no están estructurados no necesariamente están mal. Si te decimos que la mayoría de los documentos se encuentran en formatos no legibles para la máquina, como PDF o Word e imágenes como GIF, JPEG, PNG, BMP, tal vez te parezca muy extraño que estos formatos no sean legibles en computadora. A lo que nos referimos es que estos formatos no son buenos vehículos para procesar datos. Están diseñados para que se vean estéticos o para imprimir, pero no para poder procesar la información.

Los datos que sí pueden ser leídos por las computadoras son simples y están codificados para que la computadora los pueda entender y procesar. Al contrario de los datos no estructurados (Pdf, Word), NO son sencillos de leer para nosotros, pero sí para las computadoras.

Los datos vienen en muchos formatos, siendo las tablas los formatos más comunes. Una tabla representa un set de datos en columnas y filas, y cada dato es único. Cada dato puede presentarse como una letra o como números. Los formatos CSV o TSV son necesarios para tabular datos y son legibles por tu computadora. Ambos formatos representan un solo set de datos en una fila, una coma para CSV y una tabla para TSV en columnas separadas. Todas las bases de datos son fáciles de trabajar en los dos formatos antes descritos.
# 2. Formato CSV
Los archivos **CSV** (del inglés comma-separated values) son un tipo de documento en formato abierto sencillo para representar datos en forma de tabla, en las que las columnas se separan por comas.
El formato **CSV** es muy sencillo y no indica un juego de caracteres concreto, ni cómo van situados los bytes, ni el formato para el salto de línea. Estos puntos deben indicarse muchas veces al abrir el archivo, por ejemplo, con una hoja de cálculo.
El formato CSV no está estandarizado. La idea básica de separar los campos con una coma es muy clara, pero se vuelve complicada cuando el valor del campo también contienen comillas dobles o saltos de línea. Las implementaciones de CSV pueden no manejar esos datos, o usar comillas de otra clase para envolver el campo. Pero esto no resuelve el problema: algunos campos también necesitan embeber estas comillas, así que las implementaciones de CSV pueden incluir caracteres o secuencias de escape.
Además, el término "CSV" también denota otros formatos de valores separados por delimitadores que usan delimitadores diferentes a la coma (como los valores separados por tabuladores). Un delimitador que no está presente en los valores de los campos (como un tabulador) mantiene el formato simple. Estos archivos separados por delimitadores alternativos reciben en algunas ocasiones la extensión aunque este uso sea incorrecto. Esto puede causar problemas en el intercambio de datos, por ello muchas aplicaciones que usan archivos CSV tienen opciones para cambiar el carácter delimitador.
Un archivo CSV (“valores separados por comas”) es un archivo de texto simple en el que los valores están separados por comas, de modo que los datos puedan guardarse en formato tabla. Puedes usar un CSV para cargar tus listas de suscriptores y sus propiedades (nombre, teléfono, dirección, etc.). Una forma sencilla de crear un archivo CSV es usar tu editor de texto preferido (Word, Notepad, etc.) o un programa de hojas de cálculo (Excel, Hojas de Cálculo de Google, etc.) y usar la opción “Guardar como” o “Exportar”

| Año | Marca | Modelo | Descripción | Precio |
| ---------- | ---------- | ---------- | ---------- | ---------- |
| 1997   | Ford |E350| ac, abs, moon | 3000.00|
| 1999   | Chevy |Venture| Extended Edition| 4900.00|
| 1999  | Chevy |Venture| Extended Edition, Very Large | 5000.00|
| 1996   | Jeep |Grand Cherokee| MUST SELL! air,moon,roof,loaded | 4799.00|

La tabla de arriba puede ser representado como sigue en CSV:

Año;Marca;Modelo;Descripción;Precio
1997;Ford;E350;ac, abs, moon;3000.00
1999;Chevy;Venture;Extended Edition;;4900.00
1999;Chevy;Venture;Extended Edition,Very Large;;5000.00
1996;Jeep;Grand Cherokee;"MUST SELL!
air;moon roof;loaded;4799.00
# 3. Formato TSV
Los ficheros TSV (del inglés tab separated values, valores separados por tabulaciones) son un tipo de documento sencillo para representar datos en forma de tabla, en las que las columnas se separan por tabulaciones y las filas por saltos de línea.
