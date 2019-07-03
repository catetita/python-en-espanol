**Tutorial de python**
========

.. image:: https://github.com/catetita/pyton-en-espanol/blob/master/1_PXHkfdYyliqb1qCrznu5TQ.jpeg


**Introducción**
-------
**¿Qué es Python?**

Python es un lenguaje de programación creado por Guido van Rossum 
a principios de los años 90 cuyo nombre está inspirado en el grupo de 
cómicos ingleses “Monty Python”. Es un lenguaje similar a Perl, pero 
con una sintaxis muy limpia y que favorece un código legible.
Se trata de un lenguaje interpretado o de script, con tipado dinámico, 
fuertemente tipado, multiplataforma y orientado a objetos.

**Lenguaje interpretado o de script**

Un lenguaje interpretado o de script es aquel que se ejecuta utilizando 
un programa intermedio llamado intérprete, en lugar de compilar el 
código a lenguaje máquina que pueda comprender y ejecutar directa-
mente una computadora (lenguajes compilados).
La ventaja de los lenguajes compilados es que su ejecución es más 
rápida. Sin embargo los lenguajes interpretados son más flexibles y más 
portables.
Python tiene, no obstante, muchas de las características de los lengua-
jes compilados, por lo que se podría decir que es semi interpretado. En 
Python, como en Java y muchos otros lenguajes, el código fuente se 
traduce a un pseudo código máquina intermedio llamado bytecode la 
primera vez que se ejecuta, generando archivos .pyc o .pyo (bytecode 
optimizado), que son los que se ejecutarán en sucesivas ocasiones.

**Tipado dinámico**

La característica de tipado dinámico se refiere a que no es necesario 
declarar el tipo de dato que va a contener una determinada variable, 
sino que su tipo se determinará en tiempo de ejecución según el tipo 
del valor al que se asigne, y el tipo de esta variable puede cambiar si se 
le asigna un valor de otro tipo.

**Fuertemente tipado**

No se permite tratar a una variable como si fuera de un tipo distinto 
al que tiene, es necesario convertir de forma explícita dicha variable 
al nuevo tipo previamente. Por ejemplo, si tenemos una variable que 
contiene un texto (variable de tipo cadena o string) no podremos tra-
tarla como un número (sumar la cadena “9” y el número 8). En otros 
lenguajes el tipo de la variable cambiaría para adaptarse al comporta-
miento esperado, aunque esto es más propenso a errores.

**Multiplataforma**

El intérprete de Python está disponible en multitud de plataformas 
(UNIX, Solaris, Linux, DOS, Windows, OS/2, Mac OS, etc.) por lo 
que si no utilizamos librerías específicas de cada plataforma nuestro 
programa podrá correr en todos estos sistemas sin grandes cambios.

**Orientado a objetos**

La orientación a objetos es un paradigma de programación en el que 
los conceptos del mundo real relevantes para nuestro problema se tras-
ladan a clases y objetos en nuestro programa. La ejecución del progra-
ma consiste en una serie de interacciones entre los objetos.
Python también permite la programación imperativa, programación 
funcional y programación orientada a aspectos.

**¿Por qué Python?**

Python es un lenguaje que todo el mundo debería conocer. Su sintaxis 
simple, clara y sencilla; el tipado dinámico, el gestor de memoria, la 
gran cantidad de librerías disponibles y la potencia del lenguaje, entre 
otros, hacen que desarrollar una aplicación en Python sea sencillo, muy 
rápido y, lo que es más importante, divertido.
La sintaxis de Python es tan sencilla y cercana al lenguaje natural que 
los programas elaborados en Python parecen pseudocódigo. Por este 
motivo se trata además de uno de los mejores lenguajes para comenzar 
a programar.
Python no es adecuado sin embargo para la programación de bajo 
nivel o para aplicaciones en las que el rendimiento sea crítico.
Algunos casos de éxito en el uso de Python son Google, Yahoo, la 
NASA, Industrias Light & Magic, y todas las distribuciones Linux, en 
las que Python cada vez representa un tanto por ciento mayor de los 
programas disponibles.

**Instalación de Python**

Existen varias implementaciones distintas de Python: CPython, 
Jython, IronPython, PyPy, etc.
CPython es la más utilizada, la más rápida y la más madura. Cuando la 
gente habla de Python normalmente se refiere a esta implementación. 
En este caso tanto el intérprete como los módulos están escritos en C.
Jython es la implementación en Java de Python, mientras que 
IronPython es su contrapartida en C# (.NET). Su interés estriba en 
que utilizando estas implementaciones se pueden utilizar todas las 
librerías disponibles para los programadores de Java y .NET.
PyPy, por último, como habréis adivinado por el nombre, se trata de 
una implementación en Python de Python.
CPython está instalado por defecto en la mayor parte de las distribu-
ciones Linux y en las últimas versiones de Mac OS. Para comprobar si 
está instalado abre una terminal y escribe python. Si está instalado se 
iniciará la consola interactiva de Python y obtendremos parecido a lo 
siguiente:

.. code-block:: nim

 Python 2.5.1 (r251:54863, May 2 2007, 16:56:35)
 [GCC 4.1.2 (Ubuntu 4.1.2-0ubuntu4)] on linux2
 Type “help”, “copyright”, “credits” or “license” for more 
 information.
 >>> 


La primera línea nos indica la versión de Python que tenemos ins-
talada. Al final podemos ver el prompt (>>>) que nos indica que el 
intérprete está esperando código del usuario. Podemos salir escribiendo 
exit(), o pulsando Control + D.
Si no te muestra algo parecido no te preocupes, instalar Python es muy 
sencillo. Puedes descargar la versión correspondiente a tu sistema ope-
rativo desde la web de Python, en http://www.python.org/download/. 
Existen instaladores para Windows y Mac OS. Si utilizas Linux es 
muy probable que puedas instalarlo usando la herramienta de gestión 
de paquetes de tu distribución, aunque también podemos descargar la 
aplicación compilada desde la web de Python.

**Herramientas básicas**
-----

Existen dos formas de ejecutar código Python. Podemos escribir líneas 
de código en el intérprete y obtener una respuesta del intérprete para 
cada línea (sesión interactiva) o bien podemos escribir el código de un 
programa en un archivo de texto y ejecutarlo.
A la hora de realizar una sesión interactiva os aconsejo instalar y uti-
lizar iPython, en lugar de la consola interactiva de Python. Se puede 
encontrar en http://ipython.scipy.org/. iPython cuenta con características 
añadidas muy interesantes, como el autocompletado o el operador ?. 
(para activar la característica de autocompletado en Windows es nece-
sario instalar PyReadline, que puede descargarse desde http://ipython.
scipy.org/ moin/PyReadline/Intro)
La función de autocompletado se lanza pulsando el tabulador. Si 
escribimos fi y pulsamos Tab nos mostrará una lista de los objetos 
que comienzan con fi (file, filter y finally). Si escribimos file. y 
pulsamos Tab nos mostrará una lista de los métodos y propiedades del 
objeto file.
El operador ? nos muestra información sobre los objetos. Se utiliza 
añadiendo el símbolo de interrogación al final del nombre del objeto 
del cual queremos más información. Por ejemplo:

.. code-block:: nim

 In [3]: str?
 Type: type
 Base Class:
 String Form:
 Namespace: Python builtin
 Docstring:
 str(object) -> string

 Return a nice string representation of the object.
 If the argument is a string, the return value is the same 
 object. 

En el campo de IDEs y editores de código gratuitos PyDEV *(http://
pydev.sourceforge.net/)* se alza como cabeza de serie. PyDEV es un plu-
gin para Eclipse que permite utilizar este IDE multiplataforma para 
programar en Python. Cuenta con autocompletado de código (con 
información sobre cada elemento), resaltado de sintaxis, un depurador 
gráfico, resaltado de errores, explorador de clases, formateo del código, 
refactorización, etc. Sin duda es la opción más completa, sobre todo si 
instalamos las extensiones comerciales, aunque necesita de una canti-
dad importante de memoria y no es del todo estable.

Otras opciones gratuitas a considerar son SPE o Stani’s Python Editor 
*(http://sourceforge.net/projects/spe/)* ,  Eric *(http://die-offenbachs.de/eric/)* , 
BOA Constructor *(http://boa-constructor.sourceforge.net/)* o incluso 
emacs o vim.

Si no te importa desembolsar algo de dinero, Komodo *(http://www.
activestate.com/komodo_ide/)* y Wing IDE *(http://www.wingware.com/)* 
son también muy buenas opciones, con montones de características 
interesantes, como PyDEV, pero mucho más estables y robustos. Ade-
más, si desarrollas software libre no comercial puedes contactar con 
Wing Ware y obtener, con un poco de suerte, una licencia gratuita para 
Wing IDE Professional :)

**Mi primer programa en python**
=======

Como comentábamos en el capítulo anterior existen dos formas de 
ejecutar código Python, bien en una sesión interactiva (línea a línea) 
con el intérprete, o bien de la forma habitual, escribiendo el código en 
un archivo de código fuente y ejecutándolo.
El primer programa que vamos a escribir en Python es el clásico Hola 
Mundo, y en este lenguaje es tan simple como:

.. code-block:: nim

 print “Hola Mundo”

Vamos a probarlo primero en el intérprete. Ejecuta python o ipython 
según tus preferencias, escribe la línea anterior y pulsa Enter. El intér-
prete responderá mostrando en la consola el texto Hola Mundo.
Vamos ahora a crear un archivo de texto con el código anterior, de 
forma que pudiéramos distribuir nuestro pequeño gran programa entre 
nuestros amigos. Abre tu editor de texto preferido o bien el IDE que 
hayas elegido y copia la línea anterior. Guárdalo como hola.py, por 
ejemplo.
Ejecutar este programa es tan sencillo como indicarle el nombre del 
archivo a ejecutar al intérprete de Python

.. code-block:: nim

 python hola.py

pero vamos a ver cómo simplificarlo aún más.

Si utilizas Windows los archivos .py ya estarán asociados al intérprete 
de Python, por lo que basta hacer doble clic sobre el archivo para eje-
cutar el programa. Sin embargo como este programa no hace más que 
imprimir un texto en la consola, la ejecución es demasiado rápida para 
poder verlo si quiera. Para remediarlo, vamos a añadir una nueva línea 
que espere la entrada de datos por parte del usuario.

.. code-block:: nim

 print “Hola Mundo”
 raw_input()


De esta forma se mostrará una consola con el texto Hola Mundo hasta 
que pulsemos Enter.

Si utilizas Linux (u otro Unix) para conseguir este comportamiento, es 
decir, para que el sistema operativo abra el archivo .py con el intérprete 
adecuado, es necesario añadir una nueva línea al principio del archivo:

.. code-block:: nim

 #!/usr/bin/python
 print “Hola Mundo”
 raw_input()

A esta línea se le conoce en el mundo Unix como ``shebang`` , ``hashbang`` 
o ``sharpbang`` . El par de caracteres #! indica al sistema operativo que 
dicho script se debe ejecutar utilizando el intérprete especificado a 
continuación. De esto se desprende, evidentemente, que si esta no es la 
ruta en la que está instalado nuestro intérprete de Python, es necesario 
cambiarla.

Otra opción es utilizar el programa env (de environment, entorno) 
para preguntar al sistema por la ruta al intérprete de Python, de forma 
que nuestros usuarios no tengan ningún problema si se diera el caso de 
que el programa no estuviera instalado en dicha ruta:

.. code-block:: nim

 #!/usr/bin/env python
 print “Hola Mundo”
 raw_input()

Por supuesto además de añadir el shebang, tendremos que dar permi-
sos de ejecución al programa.

.. code-block:: nim

 chmod +x hola.py

Y listo, si hacemos doble clic el programa se ejecutará, mostrando una 
consola con el texto Hola Mundo, como en el caso de Windows.

También podríamos correr el programa desde la consola como si trata-
ra de un ejecutable cualquiera:

.. code-block:: nim

 ./hola.py


En Python los tipos básicos se dividen en:

* Números, como pueden ser 3 (entero), 15.57 (de coma flotante) o 
7 + 5j (complejos)

* Cadenas de texto, como “Hola Mundo”
  
* Valores booleanos: True (cierto) y False (falso).
  
Vamos a crear un par de variables a modo de ejemplo. Una de tipo 
cadena y una de tipo entero:

.. code-block:: nim

 # esto es una cadena
 c = “Hola Mundo”
 # y esto es un entero
 e = 23
 # podemos comprobarlo con la función type
 type(c)
 type(e)


Como veis en Python, a diferencia de muchos otros lenguajes, no se 
declara el tipo de la variable al crearla. En Java, por ejemplo, escribiría-
mos:

.. code-block:: nim

 String c = “Hola Mundo”;
 int e = 23;

Este pequeño ejemplo también nos ha servido para presentar los 
comentarios inline en Python: cadenas de texto que comienzan con el 
carácter # y que Python ignora totalmente. Hay más tipos de comenta-
rios, de los que hablaremos más adelante.


**Números**
-------

Como decíamos, en Python se pueden representar números enteros, 
reales y complejos.

**Enteros**

Los números enteros son aquellos números positivos o negativos que 
no tienen decimales (además del cero). En Python se pueden repre-
sentar mediante el tipo int (de integer, entero) o el tipo long (largo). 
La única diferencia es que el tipo long permite almacenar números 
más grandes. Es aconsejable no utilizar el tipo long a menos que sea 
necesario, para no malgastar memoria.

El tipo int de Python se implementa a bajo nivel mediante un tipo 
long de C. Y dado que Python utiliza C por debajo, como C, y a dife-
rencia de Java, el rango de los valores que puede representar depende 
de la plataforma.

En la mayor parte de las máquinas el long de C se almacena utilizando 
32 bits, es decir, mediante el uso de una variable de tipo int de Python 
podemos almacenar números de -231 a 231 - 1, o lo que es lo mismo, de 
-2.147.483.648 a 2.147.483.647. En plataformas de 64 bits, el rango es 
de -9.223.372.036.854.775.808 hasta 9.223.372.036.854.775.807.

El tipo long de Python permite almacenar números de cualquier preci-
sión, estando limitados solo por la memoria disponible en la máquina.

Al asignar un número a una variable esta pasará a tener tipo int, a 
menos que el número sea tan grande como para requerir el uso del tipo 
long.

.. code-block:: nim

 # type(entero) devolvería int
 entero = 23

También podemos indicar a Python que un número se almacene usan-
do long añadiendo una L al final:

.. code-block:: nim

 # type(entero) devolvería long
 entero = 23L


El literal que se asigna a la variable también se puede expresar como 
un octal, anteponiendo un cero:

.. code-block:: nim

 # 027 octal = 23 en base 10
 entero = 027

o bien en hexadecimal, anteponiendo un 0x:

.. code-block:: nim

 # 0×17 hexadecimal = 23 en base 10
 entero = 0×17

**Reales**

Los números reales son los que tienen decimales. En Python se expre-
san mediante el tipo float. En otros lenguajes de programación, como 
C, tenemos también el tipo double, similar a float pero de mayor 
precisión (double = doble precisión). Python, sin embargo, implementa 
su tipo float a bajo nivel mediante una variable de tipo double de C, 
es decir, utilizando 64 bits, luego en Python siempre se utiliza doble 
precisión, y en concreto se sigue el estándar IEEE 754: 1 bit para el 
signo, 11 para el exponente, y 52 para la mantisa. Esto significa que los 
valores que podemos representar van desde ±2,2250738585072020 x 
10-308 hasta ±1,7976931348623157×10308.

La mayor parte de los lenguajes de programación siguen el mismo 
esquema para la representación interna. Pero como muchos sabréis 
esta tiene sus limitaciones, impuestas por el hardware. Por eso desde 
Python 2.4 contamos también con un nuevo tipo Decimal, para el 
caso de que se necesite representar fracciones de forma más precisa. 
Sin embargo este tipo está fuera del alcance de este tutorial, y sólo es 
necesario para el ámbito de la programación científica y otros rela-
cionados. Para aplicaciones normales podeis utilizar el tipo float sin 
miedo, como ha venido haciéndose desde hace años, aunque teniendo 
en cuenta que los números en coma flotante no son precisos (ni en este 
ni en otros lenguajes de programación).

Para representar un número real en Python se escribe primero la parte 
entera, seguido de un punto y por último la parte decimal.

.. code-block:: nim

 real = 0.2703


También se puede utilizar notación científica, y añadir una e (de expo-
nente) para indicar un exponente en base 10. Por ejemplo:

.. code-block:: nim

 real = 0.1e-3
sería equivalente a 0.1 x 10-3 = 0.1 x 0.001 = 0.0001

**Complejos**

Los números complejos son aquellos que tienen parte imaginaria. Si 
no conocías de su existencia, es más que probable que nunca lo vayas a 
necesitar, por lo que puedes saltarte este apartado tranquilamente. De 
hecho la mayor parte de lenguajes de programación carecen de este 
tipo, aunque sea muy utilizado por ingenieros y científicos en general.

En el caso de que necesitéis utilizar números complejos, o simplemen-
te tengáis curiosidad, os diré que este tipo, llamado complex en Python, 
también se almacena usando coma flotante, debido a que estos núme-
ros son una extensión de los números reales. En concreto se almacena 
en una estructura de C, compuesta por dos variables de tipo double, 
sirviendo una de ellas para almacenar la parte real y la otra para la 
parte imaginaria.

Los números complejos en Python se representan de la siguiente 
forma:

.. code-block:: nim

 complejo = 2.1 + 7.8j

**Operadores**


Veamos ahora qué podemos hacer con nuestros números usando los 
operadores por defecto. Para operaciones más complejas podemos 
recurrir al módulo ``math`` .



**Operadores aritméticos**


================== =============== ================= 
Operador             Descripción          Ejemplo
================== =============== ================= 
     ``+``            SUMA         r = 3 + 2    # r es 5
     ``-``            RESTA        r = 4 - 7    # r es -3
================== =============== ================= 






================= ================= ============================
Operador            Descripción        Ejemplo
================= ================= ============================
     ``-``          Negación           r = -7       # r es -7
     ``*``          Multiplicación     r = 2 * 6    # r es 12
     ``**``         Exponente          r = 2 * * 6   # r es 64
     ``/``          División           r = 3.5 / 2  # r es 1.75
     ``//``         División entera    r = 3.5 // 2 # r es 1.0
     ``%``          Módulo             r = 7 % 2    # r es 1
================= ================= ============================ 


Puede que tengáis dudas sobre cómo funciona el operador de módulo, 
y cuál es la diferencia entre división y división entera.

El operador de módulo no hace otra cosa que devolvernos el resto de 
la división entre los dos operandos. En el ejemplo, 7/2 sería 3, con 1 de 
resto, luego el módulo es 1.

La diferencia entre división y división entera no es otra que la que 
indica su nombre. En la división el resultado que se devuelve es un 
número real, mientras que en la división entera el resultado que se 
devuelve es solo la parte entera.

No obstante hay que tener en cuenta que si utilizamos dos operandos 
enteros, Python determinará que queremos que la variable resultado 
también sea un entero, por lo que el resultado de, por ejemplo, 3 / 2 y 
3 // 2 sería el mismo: 1.

Si quisiéramos obtener los decimales necesitaríamos que al menos uno 
de los operandos fuera un número real, bien indicando los decimales

.. code-block:: nim

 r = 3.0 / 2


o bien utilizando la función float (no es necesario que sepais lo que 
significa el término función, ni que recordeis esta forma, lo veremos un 
poco más adelante):

.. code-block:: nim

 r = float(3) / 2


Esto es así porque cuando se mezclan tipos de números, Python con-
vierte todos los operandos al tipo más complejo de entre los tipos de 
los operandos.

**Operadores a nivel de bit**

Si no conocéis estos operadores es poco probable que vayáis a necesi-
tarlos, por lo que podéis obviar esta parte. Si aún así tenéis curiosidad 
os diré que estos son operadores que actúan sobre las representaciones 
en binario de los operandos.

Por ejemplo, si veis una operación como 3 & 2, lo que estais viendo es 
un and bit a bit entre los números binarios 11 y 10 (las representacio-
nes en binario de 3 y 2).

El operador ``and`` (&), del inglés “y”, devuelve 1 si el primer bit operando 
es 1 y el segundo bit operando es 1. Se devuelve 0 en caso contrario.

El resultado de aplicar and bit a bit a 11 y 10 sería entonces el número 
binario 10, o lo que es lo mismo, 2 en decimal (el primer dígito es 1 
para ambas cifras, mientras que el segundo es 1 sólo para una de ellas).

El operador ``or`` (|), del inglés “o”, devuelve 1 si el primer operando es 1 
o el segundo operando es 1. Para el resto de casos se devuelve 0.

El operador ``xor`` u or exclusivo (^) devuelve 1 si uno de los operandos 
es 1 y el otro no lo es.

El operador ``not`` (~), del inglés “no”, sirve para negar uno a uno cada 
bit; es decir, si el operando es 0, cambia a 1 y si es 1, cambia a 0.

Por último los operadores de desplazamiento (<< y >>) sirven para 
desplazar los bits n posiciones hacia la izquierda o la derecha.

========= =================== ======================
Operador   Descripción         Ejemplo
========= =================== ======================
&             and             r = 3 & 2  # r es 2
|             or              r = 3 | 2  # r es 3
^             xor             r = 3 ^ 2  # r es 1
~             not             r = ~3     # r es -4
<<        Desplazamiento izq. r = 3 << 1 # r es 6
>>        Desplazamiento der. r = 3 >> 1 # r es 1
========= =================== ======================


**Cadenas**

Las cadenas no son más que texto encerrado entre comillas simples 
(‘cadena’) o dobles (“cadena”). Dentro de las comillas se pueden 
añadir caracteres especiales escapándolos con \, como \n, el carácter de 
nueva línea, o \t, el de tabulación.

Una cadena puede estar precedida por el carácter u o el carácter r, los 
cuales indican, respectivamente, que se trata de una cadena que utiliza 
codificación Unicode y una cadena raw (del inglés, cruda). Las cade-
nas raw se distinguen de las normales en que los caracteres escapados 
mediante la barra invertida (\) no se sustituyen por sus contrapartidas. 
Esto es especialmente útil, por ejemplo, para las expresiones regulares, 
como veremos en el capítulo correspondiente.

.. code-block:: nim

 unicode = u”äóè”
 raw = r”\n”

También es posible encerrar una cadena entre triples comillas (simples 
o dobles). De esta forma podremos escribir el texto en varias líneas, y 
al imprimir la cadena, se respetarán los saltos de línea que introdujimos 
sin tener que recurrir al carácter \n, así como las comillas sin tener que 
escaparlas.

.. code-block:: nim

 triple = “““primera linea
      esto se vera en otra linea”””


Las cadenas también admiten operadores como +, que funciona realizando una concatenación de las cadenas utilizadas como operandos y ,
en la que se repite la cadena tantas veces como lo indique el número 
utilizado como segundo operando.

.. code-block:: nim

 a = “uno”
 b = “dos”

 c = a + b # c es “unodos”
 c = a * 3 # c es “unounouno”

**Booleanos**

Como decíamos al comienzo del capítulo una variable de tipo boolea-
no sólo puede tener dos valores: True (cierto) y False (falso). Estos 
valores son especialmente importantes para las expresiones condicio-
nales y los bucles, como veremos más adelante.

En realidad el tipo bool (el tipo de los booleanos) es una subclase del 
tipo int. Puede que esto no tenga mucho sentido para tí si no conoces 
los términos de la orientación a objetos, que veremos más adelante, 
aunque tampoco es nada importante.

Estos son los distintos tipos de operadores con los que podemos traba-
jar con valores booleanos, los llamados operadores lógicos o condicio-
nales:

========== ================== ===================================
Operador      Descripción        Ejemplo
========== ================== ===================================
and        ¿se cumple a y b?    r = True and False # r es False
or         ¿se cumple a o b?    r = True or False  # r es True
not        No a                 r = not True   # r es False
========== ================== ===================================

Los valores booleanos son además el resultado de expresiones que 
utilizan operadores relacionales (comparaciones entre valores):

========= ============================ ==========================
Operador    Descripción                  Ejemplo
========= ============================ ==========================
==          ¿son iguales a y b?          r = 5 == 3 # r es False
!=          ¿son distintos a y b?        r = 5 != 3 # r es True
<           ¿es a menor que b?           r = 5 < 3  # r es False
>           ¿es a mayor que b?           r = 5 > 3  # r es True
<=          ¿es a menor o igual que b?   r = 5 <= 5 # r es True
>=          ¿es a mayor o igual que b?   r = 5 >= 3 # r es True
========= ============================ ==========================

**Colecciones**
-------------

En el capítulo anterior vimos algunos tipos básicos, como los números, 
las cadenas de texto y los booleanos. En esta lección veremos algunos 
tipos de colecciones de datos: listas, tuplas y diccionarios.

**Lista**

La lista es un tipo de colección ordenada. Sería equivalente a lo que en 
otros lenguajes se conoce por arrays, o vectores.

Las listas pueden contener cualquier tipo de dato: números, cadenas, 
booleanos, … y también listas.

Crear una lista es tan sencillo como indicar entre corchetes, y separa-
dos por comas, los valores que queremos incluir en la lista:

.. code-block:: nim

 l = [22, True, “una lista”, [1, 2]]

Podemos acceder a cada uno de los elementos de la lista escribiendo el 
nombre de la lista e indicando el índice del elemento entre corchetes. 
Ten en cuenta sin embargo que el índice del primer elemento de la 
lista es 0, y no 1:

.. code-block:: nim

 l = [11, False]
 mi_var = l[0] # mi_var vale 11


Si queremos acceder a un elemento de una lista incluida dentro de otra 
lista tendremos que utilizar dos veces este operador, primero para in-
dicar a qué posición de la lista exterior queremos acceder, y el segundo 
para seleccionar el elemento de la lista interior:

.. code-block:: nim

 l = [“una lista”, [1, 2]] 
 mi_var = l[1][0] # mi_var vale 1

También podemos utilizar este operador para modificar un elemento 
de la lista si lo colocamos en la parte izquierda de una asignación:

.. code-block:: nim

 l = [22, True]
 l[0] = 99 # Con esto l valdrá [99, True]

El uso de los corchetes para acceder y modificar los elementos de una 
lista es común en muchos lenguajes, pero Python nos depara varias 
sorpresas muy agradables.

Una curiosidad sobre el operador [] de Python es que podemos utili-
zar también números negativos. Si se utiliza un número negativo como 
índice, esto se traduce en que el índice empieza a contar desde el final, 
hacia la izquierda; es decir, con [-1] accederíamos al último elemento 
de la lista, con [-2] al penúltimo, con [-3], al antepenúltimo, y así 
sucesivamente.

Otra cosa inusual es lo que en Python se conoce como slicing o parti-
cionado, y que consiste en ampliar este mecanismo para permitir selec-
cionar porciones de la lista. Si en lugar de un número escribimos dos 
números inicio y fin separados por dos puntos (inicio:fin) Python 
interpretará que queremos una lista que vaya desde la posición inicio 
a la posición fin, sin incluir este último. Si escribimos tres números 
(inicio:fin:salto) en lugar de dos, el tercero se utiliza para determi-
nar cada cuantas posiciones añadir un elemento a la lista.

.. code-block:: nim

 l = [99, True, “una lista”, [1, 2]] 
 mi_var = l[0:2]   # mi_var vale [99, True]
 mi_var = l[0:4:2] # mi_var vale [99, “una lista”]

Los números negativos también se pueden utilizar en un slicing, con el 
mismo comportamiento que se comentó anteriormente.

Hay que mencionar así mismo que no es necesario indicar el principio 
y el final del slicing, sino que, si estos se omiten, se usarán por defecto 
las posiciones de inicio y fin de la lista, respectivamente:

.. code-block:: nim

 l = [99, True, “una lista”]
 mi_var = l[1:]  # mi_var vale [True, “una lista”]
 mi_var = l[:2]  # mi_var vale [99, True]
 mi_var = l[:]   # mi_var vale [99, True, “una lista”]
 mi_var = l[::2] # mi_var vale [99, “una lista”]

También podemos utilizar este mecanismo para modificar la lista:

.. code-block:: nim

 l = [99, True, “una lista”, [1, 2]]
 l[0:2] = [0, 1] # l vale [0, 1, “una lista”, [1, 2]]

pudiendo incluso modificar el tamaño de la lista si la lista de la parte 
derecha de la asignación tiene un tamaño menor o mayor que el de la 
selección de la parte izquierda de la asignación:

.. code-block:: nim

 l[0:2] = [False] # l vale [False, “una lista”, [1, 2]]

En todo caso las listas ofrecen mecanismos más cómodos para ser mo-
dificadas a través de las funciones de la clase correspondiente, aunque 
no veremos estos mecanismos hasta más adelante, después de explicar 
lo que son las clases, los objetos y las funciones.

**Tuplas** 

Todo lo que hemos explicado sobre las listas se aplica también a las 
tuplas, a excepción de la forma de definirla, para lo que se utilizan 
paréntesis en lugar de corchetes.

.. code-block:: nim

 t = (1, 2, True, “python”)

En realidad el constructor de la tupla es la coma, no el paréntesis, pero 
el intérprete muestra los paréntesis, y nosotros deberíamos utilizarlos, 
por claridad.

.. code-block:: nim

 >>> t = 1, 2, 3
 >>> type(t)
 type “tuple”

Además hay que tener en cuenta que es necesario añadir una coma 
para tuplas de un solo elemento, para diferenciarlo de un elemento 
entre paréntesis.

.. code-block:: nim

 >>> t = (1)
 >>> type(t)
 type “int”
 >>> t = (1,)
 >>> type(t)
 type “tuple”

Para referirnos a elementos de una tupla, como en una lista, se usa el 
operador []:

.. code-block:: nim

 mi_var = t[0] # mi_var es 1
 mi_var = t[0:2] # mi_var es (1, 2)

Podemos utilizar el operador [] debido a que las tuplas, al igual que 
las listas, forman parte de un tipo de objetos llamados secuencias. 
Permitirme un pequeño inciso para indicaros que las cadenas de texto 
también son secuencias, por lo que no os extrañará que podamos hacer 
cosas como estas:

.. code-block:: nim

 c = “hola mundo”
 c[0]   # h
 c[5:]  # mundo
 c[::3] # hauo

Volviendo al tema de las tuplas, su diferencia con las listas estriba en 
que las tuplas no poseen estos mecanismos de modificación a través 
de funciones tan útiles de los que hablábamos al final de la anterior 
sección.

Además son inmutables, es decir, sus valores no se pueden modificar 
una vez creada; y tienen un tamaño fijo.

A cambio de estas limitaciones las tuplas son más “ligeras” que las 
listas, por lo que si el uso que le vamos a dar a una colección es muy 
básico, puedes utilizar tuplas en lugar de listas y ahorrar memoria.

**Diccionarios**

Los diccionarios, también llamados matrices asociativas, deben su 
nombre a que son colecciones que relacionan una clave y un valor. Por 
ejemplo, veamos un diccionario de películas y directores:

.. code-block:: nim

 d = {“Love Actually “: “Richard Curtis”,
     “Kill Bill”: “Tarantino”,
 “Amélie”: “Jean-Pierre Jeunet”}

El primer valor se trata de la clave y el segundo del valor asociado 
a la clave. Como clave podemos utilizar cualquier valor inmutable: 
podríamos usar números, cadenas, booleanos, tuplas, … pero no listas 
o diccionarios, dado que son mutables. Esto es así porque los diccio-
narios se implementan como tablas hash, y a la hora de introducir un 
nuevo par clave-valor en el diccionario se calcula el hash de la clave 
para después poder encontrar la entrada correspondiente rápidamente. 
Si se modificara el objeto clave después de haber sido introducido en el 
diccionario, evidentemente, su hash también cambiaría y no podría ser 
encontrado.

La diferencia principal entre los diccionarios y las listas o las tuplas es 
que a los valores almacenados en un diccionario se les accede no por su 
índice, porque de hecho no tienen orden, sino por su clave, utilizando 
de nuevo el operador [].

.. code-block:: nim

 d[“Love Actually “] # devuelve “Richard Curtis”

Al igual que en listas y tuplas también se puede utilizar este operador 
para reasignar valores.

.. code-block:: nim

 d[“Kill Bill”] = “Quentin Tarantino”

Sin embargo en este caso no se puede utilizar slicing, entre otras cosas 
porque los diccionarios no son secuencias, si no mappings (mapeados, 
asociaciones).


**Control de flujo**
------------------

En esta lección vamos a ver los condicionales y los bucles.

**Sentencias condicionales**

Si un programa no fuera más que una lista de órdenes a ejecutar de 
forma secuencial, una por una, no tendría mucha utilidad. Los con-
dicionales nos permiten comprobar condiciones y hacer que nuestro 
programa se comporte de una forma u otra, que ejecute un fragmento 
de código u otro, dependiendo de esta condición.

Aquí es donde cobran su importancia el tipo booleano y los operadores 
lógicos y relacionales que aprendimos en el capítulo sobre los tipos 
básicos de Python.

**if**

La forma más simple de un estamento condicional es un if (del inglés 
si) seguido de la condición a evaluar, dos puntos (:) y en la siguiente 
línea e indentado, el código a ejecutar en caso de que se cumpla dicha 
condición.

.. code-block:: nim

 fav = “mundogeek.net”
 # si (if) fav es igual a “mundogeek.net”
 if fav == “mundogeek.net”:
    print “Tienes buen gusto!”
    print “Gracias”

Como veis es bastante sencillo.

Eso si, aseguraros de que indentáis el código tal cual se ha hecho en el 
ejemplo, es decir, aseguraros de pulsar Tabulación antes de las dos ór-
denes print, dado que esta es la forma de Python de saber que vuestra 
intención es la de que los dos print se ejecuten sólo en el caso de que 
se cumpla la condición, y no la de que se imprima la primera cadena si 
se cumple la condición y la otra siempre, cosa que se expresaría así:

.. code-block:: nim

 if fav == “mundogeek.net”:
    print “Tienes buen gusto!”
 print “Gracias”


En otros lenguajes de programación los bloques de código se determi-
nan encerrándolos entre llaves, y el indentarlos no se trata más que de 
una buena práctica para que sea más sencillo seguir el flujo del progra-
ma con un solo golpe de vista. Por ejemplo, el código anterior expresa-
do en Java sería algo así:

.. code-block:: nim

 String fav = “mundogeek.net”;
 if (fav.equals(“mundogeek.net”)){
    System.out.println(“Tienes buen gusto!”);
    System.out.println(“Gracias”);
 }

Sin embargo, como ya hemos comentado, en Python se trata de una 
obligación, y no de una elección. De esta forma se obliga a los progra-
madores a indentar su código para que sea más sencillo de leer :)

**if … else**

Vamos a ver ahora un condicional algo más complicado. ¿Qué haría-
mos si quisiéramos que se ejecutaran unas ciertas órdenes en el caso de 
que la condición no se cumpliera? Sin duda podríamos añadir otro if 
que tuviera como condición la negación del primero:

.. code-block:: nim

 if fav == “mundogeek.net”:
    print “Tienes buen gusto!”
    print “Gracias”
 if fav != “mundogeek.net”:
    print “Vaya, que lástima”
 
pero el condicional tiene una segunda construcción mucho más útil:

.. code-block:: nim
 if fav == “mundogeek.net”:
    print “Tienes buen gusto!”
    print “Gracias”
 else:
    print “Vaya, que lástima”

Vemos que la segunda condición se puede sustituir con un else (del 
inglés: si no, en caso contrario). Si leemos el código vemos que tiene 
bastante sentido: “si fav es igual a mundogeek.net, imprime esto y esto, 
si no, imprime esto otro”.

**if … elif … elif … else**

Todavía queda una construcción más que ver, que es la que hace uso 
del elif.

.. code-block:: nim

 if numero < 0:
    print “Negativo”
 elif numero > 0:
    print “Positivo”
 else:
    print “Cero”

elif es una contracción de else if, por lo tanto elif numero > 0 puede 
leerse como “si no, si numero es mayor que 0”. Es decir, primero se 
evalúa la condición del if. Si es cierta, se ejecuta su código y se con-
tinúa ejecutando el código posterior al condicional; si no se cumple, 
se evalúa la condición del elif. Si se cumple la condición del elif 
se ejecuta su código y se continua ejecutando el código posterior al 
condicional; si no se cumple y hay más de un elif se continúa con el 
siguiente en orden de aparición. Si no se cumple la condición del if ni 
de ninguno de los elif, se ejecuta el código del else.

**A if C else B**

También existe una construcción similar al operador ? de otros lengua-
jes, que no es más que una forma compacta de expresar un if else. En 
esta construcción se evalúa el predicado C y se devuelve A si se cumple 
o B si no se cumple: A if C else B. Veamos un ejemplo:

.. code-block:: nim

 var = “par” if (num % 2 == 0) else “impar”

Y eso es todo. Si conocéis otros lenguajes de programación puede que 
esperarais que os hablara ahora del switch, pero en Python no existe 
esta construcción, que podría emularse con un simple diccionario, así 
que pasemos directamente a los bucles.

**Bucles**
---------
___________

Mientras que los condicionales nos permiten ejecutar distintos frag-
mentos de código dependiendo de ciertas condiciones, los bucles nos 
permiten ejecutar un mismo fragmento de código un cierto número de 
veces, mientras se cumpla una determinada condición.

**while**

El bucle while (mientras) ejecuta un fragmento de código mientras se 
cumpla una condición.

.. code-block:: nim

 edad = 0
 while edad < 18:
    edad = edad + 1
    print “Felicidades, tienes “ + str(edad)

La variable edad comienza valiendo 0. Como la condición de que edad 
es menor que 18 es cierta (0 es menor que 18), se entra en el bucle. 
Se aumenta edad en 1 y se imprime el mensaje informando de que 
el usuario ha cumplido un año. Recordad que el operador + para las 
cadenas funciona concatenando ambas cadenas. Es necesario utilizar 
la función str (de ``string``, cadena) para crear una cadena a partir del 
número, dado que no podemos concatenar números y cadenas, pero ya 
comentaremos esto y mucho más en próximos capítulos.

Ahora se vuelve a evaluar la condición, y 1 sigue siendo menor que 18, 
por lo que se vuelve a ejecutar el código que aumenta la edad en un 
año e imprime la edad en la pantalla. El bucle continuará ejecutándose 
hasta que edad sea igual a 18, momento en el cual la condición dejará 
de cumplirse y el programa continuaría ejecutando las instrucciones 
siguientes al bucle.

Ahora imaginemos que se nos olvidara escribir la instrucción que 
aumenta la edad. En ese caso nunca se llegaría a la condición de que 
edad fuese igual o mayor que 18, siempre sería 0, y el bucle continuaría 
indefinidamente escribiendo en pantalla Has cumplido 0.

Esto es lo que se conoce como un bucle infinito.

Sin embargo hay situaciones en las que un bucle infinito es útil. Por 
ejemplo, veamos un pequeño programa que repite todo lo que el usua-
rio diga hasta que escriba adios.

.. code-block:: nim

 while True:
    entrada = raw_input(“> “)
    if entrada == “adios”:
        break
    else:
        print entrada

Para obtener lo que el usuario escriba en pantalla utilizamos la función 
raw_input. No es necesario que sepais qué es una función ni cómo 
funciona exactamente, simplemente aceptad por ahora que en cada 
iteración del bucle la variable entrada contendrá lo que el usuario 
escribió hasta pulsar Enter.

Comprobamos entonces si lo que escribió el usuario fue adios, en cuyo 
caso se ejecuta la orden break o si era cualquier otra cosa, en cuyo caso 
se imprime en pantalla lo que el usuario escribió.

La palabra clave break (romper) sale del bucle en el que estamos.

Este bucle se podría haber escrito también, no obstante, de la siguiente 
forma:

.. code-block:: nim

 salir = False
 while not salir:
    entrada = raw_input()
    if entrada == “adios”:
        salir = True
    else:
        print entrada

pero nos ha servido para ver cómo funciona break.
Otra palabra clave que nos podemos encontrar dentro de los bucles es 
continue (continuar). Como habréis adivinado no hace otra cosa que 
pasar directamente a la siguiente iteración del bucle.

.. code-block:: nim

 edad = 0
 while edad < 18:
    edad = edad + 1
    if edad % 2 == 0:
        continue
    print “Felicidades, tienes “ + str(edad)

Como veis esta es una pequeña modificación de nuestro programa de 
felicitaciones. En esta ocasión hemos añadido un if que comprueba si 
la edad es par, en cuyo caso saltamos a la próxima iteración en lugar de 
imprimir el mensaje. Es decir, con esta modificación el programa sólo 
imprimiría felicitaciones cuando la edad fuera impar.

**for … in**

A los que hayáis tenido experiencia previa con según que lenguajes este 
bucle os va a sorprender gratamente. En Python for se utiliza como 
una forma genérica de iterar sobre una secuencia. Y como tal intenta 
facilitar su uso para este fin.

Este es el aspecto de un bucle for en Python:

.. code-block:: nim

 secuencia = [“uno”, “dos”, “tres”]
 for elemento in secuencia:
    print elemento

Como hemos dicho los for se utilizan en Python para recorrer secuen-
cias, por lo que vamos a utilizar un tipo secuencia, como es la lista, para 
nuestro ejemplo.

Leamos la cabecera del bucle como si de lenguaje natural se tratara: 
“para cada elemento en secuencia”. Y esto es exactamente lo que hace 
el bucle: para cada elemento que tengamos en la secuencia, ejecuta 
estas líneas de código.

Lo que hace la cabecera del bucle es obtener el siguiente elemento de 
la secuencia secuencia y almacenarlo en una variable de nombre ele-
mento. Por esta razón en la primera iteración del bucle elemento valdrá 
“uno”, en la segunda “dos”, y en la tercera “tres”.

Fácil y sencillo.

En C o C++, por ejemplo, lo que habríamos hecho sería iterar sobre las 
posiciones, y no sobre los elementos:

.. code-block:: nim

 int mi_array[] = {1, 2, 3, 4, 5};
 int i;
 for(i = 0; i < 5; i++) {
    printf(“%d\n”, mi_array[i]);
 }

Es decir, tendríamos un bucle for que fuera aumentando una variable 
i en cada iteración, desde 0 al tamaño de la secuencia, y utilizaríamos 
esta variable a modo de índice para obtener cada elemento e imprimir-
lo.

Como veis el enfoque de Python es más natural e intuitivo.

Pero, ¿qué ocurre si quisiéramos utilizar el for como si estuviéramos en 
C o en Java, por ejemplo, para imprimir los números de 30 a 50? No os 
preocupéis, porque no necesitaríais crear una lista y añadir uno a uno 
los números del 30 al 50. Python proporciona una función llamada 
range (rango) que permite generar una lista que vaya desde el primer 
número que le indiquemos al segundo. Lo veremos después de ver al 
fin a qué se refiere ese término tan recurrente: las funciones.

**funCiones**
------------

Una función es un fragmento de código con un nombre asociado que 
realiza una serie de tareas y devuelve un valor. A los fragmentos de 
código que tienen un nombre asociado y no devuelven valores se les 
suele llamar procedimientos. En Python no existen los procedimien-
tos, ya que cuando el programador no especifica un valor de retorno la 
función devuelve el valor None (nada), equivalente al null de Java.

Además de ayudarnos a programar y depurar dividiendo el programa 
en partes las funciones también permiten reutilizar código.

En Python las funciones se declaran de la siguiente forma:

.. code-block:: nim

 def mi_funcion(param1, param2):
    print param1
    print param2

Es decir, la palabra clave def seguida del nombre de la función y entre 
paréntesis los argumentos separados por comas. A continuación, en 
otra línea, indentado y después de los dos puntos tendríamos las líneas 
de código que conforman el código a ejecutar por la función.

También podemos encontrarnos con una cadena de texto como 
primera línea del cuerpo de la función. Estas cadenas se conocen con 
el nombre de docstring (cadena de documentación) y sirven, como su 
nombre indica, a modo de documentación de la función.

.. code-block:: nim

 def mi_funcion(param1, param2):
    “““Esta funcion imprime los dos valores pasados
    como parametros”””
    print param1
    print param2

Esto es lo que imprime el opeardor ? de iPython o la función help 
del lenguaje para proporcionar una ayuda sobre el uso y utilidad de 
las funciones. Todos los objetos pueden tener docstrings, no solo las 
funciones, como veremos más adelante.

Volviendo a la declaración de funciones, es importante aclarar que 
al declarar la función lo único que hacemos es asociar un nombre al 
fragmento de código que conforma la función, de forma que podamos 
ejecutar dicho código más tarde referenciándolo por su nombre. Es 
decir, a la hora de escribir estas líneas no se ejecuta la función. Para 
llamar a la función (ejecutar su código) se escribiría:

.. code-block:: nim

 mi_funcion(“hola”, 2)

Es decir, el nombre de la función a la que queremos llamar seguido de 
los valores que queramos pasar como parámetros entre paréntesis. La 
asociación de los parámetros y los valores pasados a la función se hace 
normalmente de izquierda a derecha: como a param1 le hemos dado un 
valor “hola” y param2 vale 2, mi_funcion imprimiría hola en una línea, 
y a continuación 2.

Sin embargo también es posible modificar el orden de los parámetros 
si indicamos el nombre del parámetro al que asociar el valor a la hora 
de llamar a la función:

.. code-block:: nim

 mi_funcion(param2 = 2, param1 = “hola”)

El número de valores que se pasan como parámetro al llamar a la fun-
ción tiene que coincidir con el número de parámetros que la función 
acepta según la declaración de la función. En caso contrario Python se 
quejará:

.. code-block:: nim

 >>> mi_funcion(“hola”)
 Traceback (most recent call last):
 File “<stdin>”, line 1, in <module>
 TypeError: mi_funcion() takes exactly 2 arguments (1 given)

También es posible, no obstante, definir funciones con un número va-
riable de argumentos, o bien asignar valores por defecto a los paráme-
tros para el caso de que no se indique ningún valor para ese parámetro 
al llamar a la función.

Los valores por defecto para los parámetros se definen situando un 
signo igual después del nombre del parámetro y a continuación el valor 
por defecto:

.. code-block:: nim

 def imprimir(texto, veces = 1):
    print veces * texto

En el ejemplo anterior si no indicamos un valor para el segundo 
parámetro se imprimirá una sola vez la cadena que le pasamos como 
primer parámetro:

.. code-block:: nim

 >>> imprimir(“hola”)
 hola

si se le indica otro valor, será este el que se utilice:

.. code-block:: nim
 >>> imprimir(“hola”, 2)
 holahola

Para definir funciones con un número variable de argumentos coloca-
mos un último parámetro para la función cuyo nombre debe preceder-
se de un signo :

.. code-block:: nim

 def varios(param1, param2, *otros):
    for val in otros:
        print val

.. code-block:: nim

 varios(1, 2)
 varios(1, 2, 3)
 varios(1, 2, 3, 4)

Esta sintaxis funciona creando una tupla (de nombre otros en el 
ejemplo) en la que se almacenan los valores de todos los parámetros 
extra pasados como argumento. Para la primera llamada, varios(1, 2), 
la tupla otros estaría vacía dado que no se han pasado más parámetros 
que los dos definidos por defecto, por lo tanto no se imprimiría nada. 
En la segunda llamada otros valdría (3, ), y en la tercera (3, 4).


También se puede preceder el nombre del último parámetro con * * , en 
cuyo caso en lugar de una tupla se utilizaría un diccionario. Las claves 
de este diccionario serían los nombres de los parámetros indicados al 
llamar a la función y los valores del diccionario, los valores asociados a 
estos parámetros.

En el siguiente ejemplo se utiliza la función items de los diccionarios, 
que devuelve una lista con sus elementos, para imprimir los parámetros 
que contiene el diccionario.

.. code-block:: nim

 def varios(param1, param2, **otros):
    for i in otros.items():
        print i
 varios(1, 2, tercero = 3)

Los que conozcáis algún otro lenguaje de programación os estaréis 
preguntando si en Python al pasar una variable como argumento de 
una función estas se pasan por referencia o por valor. En el paso por 
referencia lo que se pasa como argumento es una referencia o puntero 
a la variable, es decir, la dirección de memoria en la que se encuentra el 
contenido de la variable, y no el contenido en si. En el paso por valor, 
por el contrario, lo que se pasa como argumento es el valor que conte-
nía la variable.

La diferencia entre ambos estriba en que en el paso por valor los 
cambios que se hagan sobre el parámetro no se ven fuera de la fun-
ción, dado que los argumentos de la función son variables locales a la 
función que contienen los valores indicados por las variables que se 
pasaron como argumento. Es decir, en realidad lo que se le pasa a la 
función son copias de los valores y no las variables en si.
Si quisiéramos modificar el valor de uno de los argumentos y que estos 
cambios se reflejaran fuera de la función tendríamos que pasar el pará-
metro por referencia.

En C los argumentos de las funciones se pasan por valor, aunque se 
puede simular el paso por referencia usando punteros. En Java también 
se usa paso por valor, aunque para las variables que son objetos lo que 
se hace es pasar por valor la referencia al objeto, por lo que en realidad 
parece paso por referencia.

En Python también se utiliza el paso por valor de referencias a objetos,
como en Java, aunque en el caso de Python, a diferencia de Java, todo 
es un objeto (para ser exactos lo que ocurre en realidad es que al objeto 
se le asigna otra etiqueta o nombre en el espacio de nombres local de la 
función).

Sin embargo no todos los cambios que hagamos a los parámetros 
dentro de una función Python se reflejarán fuera de esta, ya que hay 
que tener en cuenta que en Python existen objetos inmutables, como 
las tuplas, por lo que si intentáramos modificar una tupla pasada como 
parámetro lo que ocurriría en realidad es que se crearía una nueva ins-
tancia, por lo que los cambios no se verían fuera de la función.

Veamos un pequeño programa para demostrarlo. En este ejemplo 
se hace uso del método append de las listas. Un método no es más 
que una función que pertenece a un objeto, en este caso a una lista; y 
append, en concreto, sirve para añadir un elemento a una lista.

.. code-block:: nim

 def f(x, y):
    x = x + 3
    y.append(23)
    print x, y

.. code-block:: nim

 x = 22
 y = [22]
 f(x, y)
 print x, y

El resultado de la ejecución de este programa sería

.. code-block:: nim

 25 [22, 23]
 22 [22, 23]

Como vemos la variable x no conserva los cambios una vez salimos de 
la función porque los enteros son inmutables en Python. Sin embargo 
la variable y si los conserva, porque las listas son mutables.

En resumen: los valores mutables se comportan como paso por refe-
rencia, y los inmutables como paso por valor.

Con esto terminamos todo lo relacionado con los parámetros de las 
funciones. Veamos por último cómo devolver valores, para lo que se 
utiliza la palabra clave return:

.. code-block:: nim

 def sumar(x, y):
    return x + y

.. code-block:: nim   

 print sumar(3, 2)

Como vemos esta función tan sencilla no hace otra cosa que sumar los 
valores pasados como parámetro y devolver el resultado como valor de 
retorno.

También podríamos pasar varios valores que retornar a return.

.. code-block:: nim

 def f(x, y):
    return x * 2, y * 2

.. code-block:: nim

 a, b = f(1, 2)

Sin embargo esto no quiere decir que las funciones Python puedan de-
volver varios valores, lo que ocurre en realidad es que Python crea una 
tupla al vuelo cuyos elementos son los valores a retornar, y esta única 
variable es la que se devuelve.

**orientaCión a objetos**
-------------------------

En el capítulo de introducción ya comentábamos que Python es un 
lenguaje multiparadigma en el se podía trabajar con programación es-
tructurada, como veníamos haciendo hasta ahora, o con programación 
orientada a objetos o programación funcional.

La Programación Orientada a Objetos (POO u OOP según sus siglas 
en inglés) es un paradigma de programación en el que los conceptos 
del mundo real relevantes para nuestro problema se modelan a través 
de clases y objetos, y en el que nuestro programa consiste en una serie 
de interacciones entre estos objetos.

**Clases y objetos**

Para entender este paradigma primero tenemos que comprender qué es 
una clase y qué es un objeto. Un objeto es una entidad que agrupa un 
estado y una funcionalidad relacionadas. El estado del objeto se define 
a través de variables llamadas atributos, mientras que la funcionalidad 
se modela a través de funciones a las que se les conoce con el nombre 
de métodos del objeto.

Un ejemplo de objeto podría ser un coche, en el que tendríamos atri-
butos como la marca, el número de puertas o el tipo de carburante y 
métodos como arrancar y parar. O bien cualquier otra combinación de 
atributos y métodos según lo que fuera relevante para nuestro progra-
ma.

Una clase, por otro lado, no es más que una plantilla genérica a partir 
de la cuál instanciar los objetos; plantilla que es la que define qué atri-
butos y métodos tendrán los objetos de esa clase.

Volviendo a nuestro ejemplo: en el mundo real existe un conjunto de 
objetos a los que llamamos coches y que tienen un conjunto de atribu-
tos comunes y un comportamiento común, esto es a lo que llamamos 
clase. Sin embargo, mi coche no es igual que el coche de mi vecino, y 
aunque pertenecen a la misma clase de objetos, son objetos distintos.

En Python las clases se definen mediante la palabra clave class segui-
da del nombre de la clase, dos puntos (:) y a continuación, indentado, 
el cuerpo de la clase. Como en el caso de las funciones, si la primera 
línea del cuerpo se trata de una cadena de texto, esta será la cadena de 
documentación de la clase o docstring.

.. code-block:: nim

 class Coche:
    “””Abstraccion de los objetos coche.”””
    def __init__(self, gasolina):
        self.gasolina = gasolina
        print “Tenemos”, gasolina, “litros”
    def arrancar(self):
        if self.gasolina > 0:
            print “Arranca”
        else:
            print “No arranca”
    def conducir(self):
        if self.gasolina > 0:
            self.gasolina -= 1
            print “Quedan”, self.gasolina, “litros”
        else:
            print “No se mueve”


Lo primero que llama la atención en el ejemplo anterior es el nombre 
tan curioso que tiene el método _ _ init _ _. Este nombre es una conven-
ción y no un capricho. El método _ _ init _ _, con una doble barra baja al 
principio y final del nombre, se ejecuta justo después de crear un nuevo 
objeto a partir de la clase, proceso que se conoce con el nombre de 
instanciación. El método _ _ init _ _ sirve, como sugiere su nombre, para 
realizar cualquier proceso de inicialización que sea necesario.

Como vemos el primer parámetro de _ _ init _ _ y del resto de métodos 
de la clase es siempre self. Esta es una idea inspirada en Modula-3 y 
sirve para referirse al objeto actual. Este mecanismo es necesario para 
poder acceder a los atributos y métodos del objeto diferenciando, por 
ejemplo, una variable local mi_var de un atributo del objeto self.
mi_var.

Si volvemos al método __init__ de nuestra clase Coche veremos cómo 
se utiliza self para asignar al atributo gasolina del objeto (self.gaso-
lina) el valor que el programador especificó para el parámetro gasoli-
na. El parámetro gasolina se destruye al final de la función, mientras 
que el atributo gasolina se conserva (y puede ser accedido) mientras el 
objeto viva.

Para crear un objeto se escribiría el nombre de la clase seguido de cual-
quier parámetro que sea necesario entre paréntesis. Estos parámetros 
son los que se pasarán al método __init__, que como decíamos es el 
método que se llama al instanciar la clase.

.. code-block:: nim

 mi_coche = Coche(3)

Os preguntareis entonces cómo es posible que a la hora de crear nues-
tro primer objeto pasemos un solo parámetro a __init__, el número 
3, cuando la definición de la función indica claramente que precisa de 
dos parámetros (self y gasolina). Esto es así porque Python pasa el 
primer argumento (la referencia al objeto que se crea) automágicamen-
te.

Ahora que ya hemos creado nuestro objeto, podemos acceder a sus 
atributos y métodos mediante la sintaxis objeto.atributo y objeto.
metodo():

.. code-block:: nim

 >>> print mi_coche.gasolina
 3
 >>> mi_coche.arrancar()
 Arranca
 >>> mi_coche.conducir()
 Quedan 2 litros
 >>> mi_coche.conducir()
 Quedan 1 litros
 >>> mi_coche.conducir()
 Quedan 0 litros
 >>> mi_coche.conducir()
 No se mueve
 >>> mi_coche.arrancar()
 No arranca
 >>> print mi_coche.gasolina
 0

Como último apunte recordar que en Python, como ya se comentó 
en repetidas ocasiones anteriormente, todo son objetos. Las cadenas, 
por ejemplo, tienen métodos como upper(), que devuelve el texto en 
mayúsculas o count(sub), que devuelve el número de veces que se 
encontró la cadena sub en el texto.

**Herencia**

Hay tres conceptos que son básicos para cualquier lenguaje de pro-
gramación orientado a objetos: el encapsulamiento, la herencia y el 
polimorfismo.

En un lenguaje orientado a objetos cuando hacemos que una clase 
(subclase) herede de otra clase (superclase) estamos haciendo que la 
subclase contenga todos los atributos y métodos que tenía la supercla-
se. No obstante al acto de heredar de una clase también se le llama a 
menudo “extender una clase”.

Supongamos que queremos modelar los instrumentos musicales de 
una banda, tendremos entonces una clase Guitarra, una clase Batería, 
una clase Bajo, etc. Cada una de estas clases tendrá una serie de atribu-
tos y métodos, pero ocurre que, por el mero hecho de ser instrumentos 
musicales, estas clases compartirán muchos de sus atributos y métodos; 
un ejemplo sería el método tocar().

Es más sencillo crear un tipo de objeto Instrumento con las atributos y 
métodos comunes e indicar al programa que Guitarra, Batería y Bajo 
son tipos de instrumentos, haciendo que hereden de Instrumento.

Para indicar que una clase hereda de otra se coloca el nombre de la cla-
se de la que se hereda entre paréntesis después del nombre de la clase:

.. code-block:: nim

 class Instrumento:
    def __init__(self, precio):
 self.precio = precio
    def tocar(self):
        print “Estamos tocando musica”
    def romper(self):
        print “Eso lo pagas tu”
        print “Son”, self.precio, “$$$”
 class Bateria(Instrumento):
    pass
 class Guitarra(Instrumento):
    pass

Como Bateria y Guitarra heredan de Instrumento, ambos tienen un 
método tocar() y un método romper(), y se inicializan pasando un 
parámetro precio. Pero, ¿qué ocurriría si quisiéramos especificar un 
nuevo parámetro tipo_cuerda a la hora de crear un objeto Guitarra? 
Bastaría con escribir un nuevo método __init__ para la clase Guitarra 
que se ejecutaría en lugar del __init__ de Instrumento. Esto es lo que 
se conoce como sobreescribir métodos.

Ahora bien, puede ocurrir en algunos casos que necesitemos sobrees-
cribir un método de la clase padre, pero que en ese método queramos 
ejecutar el método de la clase padre porque nuestro nuevo método no 
necesite más que ejecutar un par de nuevas instrucciones extra. En ese 
caso usaríamos la sintaxis SuperClase.metodo(self, args) para llamar 
al método de igual nombre de la clase padre. Por ejemplo, para llamar 
al método __init__ de Instrumento desde Guitarra usaríamos Instru-
mento.__init__(self, precio)

Observad que en este caso si es necesario especificar el parámetro self.

**Herencia múltiple**

En Python, a diferencia de otros lenguajes como Java o C#, se permite 
la herencia múltiple, es decir, una clase puede heredar de varias clases a 
la vez. Por ejemplo, podríamos tener una clase Cocodrilo que heredara 
de la clase Terrestre, con métodos como caminar() y atributos como 
velocidad_caminar y de la clase Acuatico, con métodos como nadar() 
y atributos como velocidad_nadar. Basta con enumerar las clases de 

las que se hereda separándolas por comas:

.. code-block:: nim

 class Cocodrilo(Terrestre, Acuatico):
    pass

En el caso de que alguna de las clases padre tuvieran métodos con el 
mismo nombre y número de parámetros las clases sobreescribirían la 
implementación de los métodos de las clases más a su derecha en la 
definición.

En el siguiente ejemplo, como Terrestre se encuentra más a la iz-
quierda, sería la definición de desplazar de esta clase la que prevale-
cería, y por lo tanto si llamamos al método desplazar de un objeto de 
tipo Cocodrilo lo que se imprimiría sería “El animal anda”.

.. code-block:: nim

 class Terrestre:
    def desplazar(self):
        print “El animal anda”
 class Acuatico:
    def desplazar(self):
        print “El animal nada”
 class Cocodrilo(Terrestre, Acuatico):
    pass
 c = Cocodrilo()
 c.desplazar()

**Polimorfismo**

La palabra polimorfismo, del griego poly morphos (varias formas), se re-
fiere a la habilidad de objetos de distintas clases de responder al mismo 
mensaje. Esto se puede conseguir a través de la herencia: un objeto de 
una clase derivada es al mismo tiempo un objeto de la clase padre, de 
forma que allí donde se requiere un objeto de la clase padre también se 
puede utilizar uno de la clase hija.

Python, al ser de tipado dinámico, no impone restricciones a los tipos 
que se le pueden pasar a una función, por ejemplo, más allá de que el 
objeto se comporte como se espera: si se va a llamar a un método f() 
del objeto pasado como parámetro, por ejemplo, evidentemente el 
objeto tendrá que contar con ese método. Por ese motivo, a diferencia 
de lenguajes de tipado estático como Java o C++, el polimorfismo en 
Python no es de gran importancia.

En ocasiones también se utiliza el término polimorfismo para referirse 
a la sobrecarga de métodos, término que se define como la capacidad 
del lenguaje de determinar qué método ejecutar de entre varios méto-
dos con igual nombre según el tipo o número de los parámetros que se 
le pasa. En Python no existe sobrecarga de métodos (el último método 
sobreescribiría la implementación de los anteriores), aunque se puede 
conseguir un comportamiento similar recurriendo a funciones con va-
lores por defecto para los parámetros o a la sintaxis * params o * * params 
explicada en el capítulo sobre las funciones en Python, o bien usando 
decoradores (mecanismo que veremos más adelante).

**Encapsulación**

La encapsulación se refiere a impedir el acceso a determinados mé-
todos y atributos de los objetos estableciendo así qué puede utilizarse 
desde fuera de la clase.

Esto se consigue en otros lenguajes de programación como Java utili-
zando modificadores de acceso que definen si cualquiera puede acceder 
a esa función o variable (public) o si está restringido el acceso a la 
propia clase (private).

En Python no existen los modificadores de acceso, y lo que se suele 
hacer es que el acceso a una variable o función viene determinado por 
su nombre: si el nombre comienza con dos guiones bajos (y no termina 
también con dos guiones bajos) se trata de una variable o función pri-
vada, en caso contrario es pública. Los métodos cuyo nombre comien-
za y termina con dos guiones bajos son métodos especiales que Python 
llama automáticamente bajo ciertas circunstancias, como veremos al 
final del capítulo.

En el siguiente ejemplo sólo se imprimirá la cadena correspondiente al 
método publico(), mientras que al intentar llamar al método __pri-
vado() Python lanzará una excepción quejándose de que no existe 
(evidentemente existe, pero no lo podemos ver porque es privado).

.. code-block:: nim

 class Ejemplo:
    def publico(self):
        print “Publico”
    def __privado(self):
        print “Privado”
 ej = Ejemplo()
 ej.publico()
 ej.__privado()

Este mecanismo se basa en que los nombres que comienzan con un 
doble guión bajo se renombran para incluir el nombre de la clase 
(característica que se conoce con el nombre de name mangling). Esto 
implica que el método o atributo no es realmente privado, y podemos 
acceder a él mediante una pequeña trampa:

.. code-block:: nim

 ej._Ejemplo__privado()

En ocasiones también puede suceder que queramos permitir el acceso 
a algún atributo de nuestro objeto, pero que este se produzca de forma 
controlada. Para esto podemos escribir métodos cuyo único cometido 
sea este, métodos que normalmente, por convención, tienen nombres 
como getVariable y setVariable; de ahí que se conozcan también con 
el nombre de getters y setters.

.. code-block:: nim

 class Fecha():
    def __init__(self):
        self.__dia = 1
    def getDia(self):
        return self.__dia
    def setDia(self, dia):
        if dia > 0 and dia < 31:
            self.__dia = dia
        else:
            print “Error”
 mi_fecha = Fecha()
 mi_fecha.setDia(33)

Esto se podría simplificar mediante propiedades, que abstraen al usua-
rio del hecho de que se está utilizando métodos entre bambalinas para 
obtener y modificar los valores del atributo:

.. code-block:: nim

 class Fecha(object):
    def __init__(self):
        self.__dia = 1
    def getDia(self):
        return self.__dia
    def setDia(self, dia):
        if dia > 0 and dia < 31:
            self.__dia = dia
        else:
            print “Error”
    dia = property(getDia, setDia)
 mi_fecha = Fecha()
 mi_fecha.dia = 33

**Clases de “nuevo-estilo”**

En el ejemplo anterior os habrá llamado la atención el hecho de que la 
clase Fecha derive de object. La razón de esto es que para poder usar 
propiedades la clase tiene que ser de “nuevo-estilo”, clases enriquecidas 
introducidas en Python 2.2 que serán el estándar en Python 3.0 pero 
que aún conviven con las clases “clásicas” por razones de retrocompa-
tibilidad. Además de las propiedades las clases de nuevo estilo añaden 
otras funcionalidades como descriptores o métodos estáticos.

Para que una clase sea de nuevo estilo es necesario, por ahora, que 
extienda una clase de nuevo-estilo. En el caso de que no sea necesa-
rio heredar el comportamiento o el estado de ninguna clase, como en 
nuestro ejemplo anterior, se puede heredar de object, que es un objeto 
vacio que sirve como base para todas las clases de nuevo estilo.

La diferencia principal entre las clases antiguas y las de nuevo estilo 
consiste en que a la hora de crear una nueva clase anteriormente no se 
definía realmente un nuevo tipo, sino que todos los objetos creados a 
partir de clases, fueran estas las clases que fueran, eran de tipo instan-
ce.

**Métodos especiales**

Ya vimos al principio del artículo el uso del método __init__. Exis-
ten otros métodos con significados especiales, cuyos nombres siempre 
comienzan y terminan con dos guiones bajos. A continuación se listan 
algunos especialmente útiles.

__init__(self, args)
Método llamado después de crear el objeto para realizar tareas de 
inicialización.

__new__(cls, args)
Método exclusivo de las clases de nuevo estilo que se ejecuta antes que 
__init__ y que se encarga de construir y devolver el objeto en sí. Es 
equivalente a los constructores de C++ o Java. Se trata de un método 
estático, es decir, que existe con independencia de las instancias de 
la clase: es un método de clase, no de objeto, y por lo tanto el primer 
parámetro no es self, sino la propia clase: cls.

__del__(self)
Método llamado cuando el objeto va a ser borrado. También llamado 
destructor, se utiliza para realizar tareas de limpieza.

__str__(self)
Método llamado para crear una cadena de texto que represente a nues-
tro objeto. Se utiliza cuando usamos print para mostrar nuestro objeto 
o cuando usamos la función str(obj) para crear una cadena a partir de 
nuestro objeto.

__cmp__(self, otro)
Método llamado cuando se utilizan los operadores de comparación 
para comprobar si nuestro objeto es menor, mayor o igual al objeto 
pasado como parámetro. Debe devolver un número negativo si nuestro 
objeto es menor, cero si son iguales, y un número positivo si nuestro 
objeto es mayor. Si este método no está definido y se intenta com-
parar el objeto mediante los operadores <, <=, > o >= se lanzará una 
excepción. Si se utilizan los operadores == o != para comprobar si dos 
objetos son iguales, se comprueba si son el mismo objeto (si tienen el 
mismo id).

__len__(self)
Método llamado para comprobar la longitud del objeto. Se utiliza, por 
ejemplo, cuando se llama a la función len(obj) sobre nuestro objeto. 
Como es de suponer, el método debe devolver la longitud del objeto.

Existen bastantes más métodos especiales, que permite entre otras 
cosas utilizar el mecanismo de slicing sobre nuestro objeto, utilizar 
los operadores aritméticos o usar la sintaxis de diccionarios, pero un 
estudio exhaustivo de todos los métodos queda fuera del propósito del 
capítulo.

**evisitando objetos**
-----------------

En los capítulos dedicados a los tipos simples y las colecciones veíamos 
por primera vez algunos de los objetos del lenguaje Python: números, 
booleanos, cadenas de texto, diccionarios, listas y tuplas.

Ahora que sabemos qué son las clases, los objetos, las funciones, y los 
métodos es el momento de revisitar estos objetos para descubrir su 
verdadero potencial.

Veremos a continuación algunos métodos útiles de estos objetos. Evi-
dentemente, no es necesario memorizarlos, pero si, al menos, recordar 
que existen para cuando sean necesarios.

**Diccionarios**

D.get(k[, d])
Busca el valor de la clave k en el diccionario. Es equivalente a utilizar 
D[k] pero al utilizar este método podemos indicar un valor a devolver 
por defecto si no se encuentra la clave, mientras que con la sintaxis 
D[k], de no existir la clave se lanzaría una excepción.

D.has_key(k)
Comprueba si el diccionario tiene la clave k. Es equivalente a la sin-
taxis k in D.

D.items()
Devuelve una lista de tuplas con pares clave-valor.

D.keys()
Devuelve una lista de las claves del diccionario.

D.pop(k[, d])
Borra la clave k del diccionario y devuelve su valor. Si no se encuentra 
dicha clave se devuelve d si se especificó el parámetro o bien se lanza 
una excepción.

D.values()
Devuelve una lista de los valores del diccionario.

**Cadenas**

S.count(sub[, start[, end]])
Devuelve el número de veces que se encuentra sub en la cadena. Los 
parámetros opcionales start y end definen una subcadena en la que 
buscar.

S.find(sub[, start[, end]])
Devuelve la posición en la que se encontró por primera vez sub en la 
cadena o -1 si no se encontró.

S.join(sequence)
Devuelve una cadena resultante de concatenar las cadenas de la se-
cuencia seq separadas por la cadena sobre la que se llama el método.

S.partition(sep)
Busca el separador sep en la cadena y devuelve una tupla con la sub-
cadena hasta dicho separador, el separador en si, y la subcadena del 
separador hasta el final de la cadena. Si no se encuentra el separador, la 
tupla contendrá la cadena en si y dos cadenas vacías.

S.replace(old, new[, count])
Devuelve una cadena en la que se han reemplazado todas las ocurren-
cias de la cadena old por la cadena new. Si se especifica el parámetro 
count, este indica el número máximo de ocurrencias a reemplazar.

S.split([sep [,maxsplit]])
Devuelve una lista conteniendo las subcadenas en las que se divide 
nuestra cadena al dividirlas por el delimitador sep. En el caso de que 
no se especifique sep, se usan espacios. Si se especifica maxsplit, este 
indica el número máximo de particiones a realizar.

**Listas**

L.append(object)
Añade un objeto al final de la lista.

L.count(value)
Devuelve el número de veces que se encontró value en la lista.

L.extend(iterable)
Añade los elementos del iterable a la lista.

L.index(value[, start[, stop]])
Devuelve la posición en la que se encontró la primera ocurrencia de 
value. Si se especifican, start y stop definen las posiciones de inicio y 
fin de una sublista en la que buscar.

L.insert(index, object)
Inserta el objeto object en la posición index.

L.pop([index])
Devuelve el valor en la posición index y lo elimina de la lista. Si no se 
especifica la posición, se utiliza el último elemento de la lista.

L.remove(value)
Eliminar la primera ocurrencia de value en la lista.

L.reverse()
Invierte la lista. Esta función trabaja sobre la propia lista desde la que 
se invoca el método, no sobre una copia.

L.sort(cmp=None, key=None, reverse=False)
Ordena la lista. Si se especifica cmp, este debe ser una función que tome 
como parámetro dos valores x e y de la lista y devuelva -1 si x es menor 
que y, 0 si son iguales y 1 si x es mayor que y.

El parámetro reverse es un booleano que indica si se debe ordenar 
la lista de forma inversa, lo que sería equivalente a llamar primero a 
L.sort() y después a L.reverse().

Por último, si se especifica, el parámetro key debe ser una función que 
tome un elemento de la lista y devuelva una clave a utilizar a la hora de 
comparar, en lugar del elemento en si.

**prograMaCión funCional**
-------------------------

La programación funcional es un paradigma en el que la programa-
ción se basa casi en su totalidad en funciones, entendiendo el concepto 
de función según su definición matemática, y no como los simples 
subprogramas de los lenguajes imperativos que hemos visto hasta 
ahora.

En los lenguajes funcionales puros un programa consiste exclusiva-
mente en la aplicación de distintas funciones a un valor de entrada 
para obtener un valor de salida.

Python, sin ser un lenguaje puramente funcional incluye varias caracte-
rísticas tomadas de los lenguajes funcionales como son las funciones de 
orden superior o las funciones lambda (funciones anónimas).

**Funciones de orden superior**

El concepto de funciones de orden superior se refiere al uso de fun-
ciones como si de un valor cualquiera se tratara, posibilitando el pasar 
funciones como parámetros de otras funciones o devolver funciones 
como valor de retorno.

Esto es posible porque, como hemos insistido ya en varias ocasiones, 
en Python todo son objetos. Y las funciones no son una excepción.
Veamos un pequeño ejemplo

.. code-block:: nim

 def saludar(lang):
    def saludar_es():
  print “Hola”
    def saludar_en():
        print “Hi”
    def saludar_fr():
        print “Salut”
    lang_func = {“es”: saludar_es,
                 “en”: saludar_en,
                 “fr”: saludar_fr}
    return lang_func[lang]
 f = saludar(“es”)
 f()

Como podemos observar lo primero que hacemos en nuestro pequeño 
programa es llamar a la función saludar con un parámetro “es”. En la 
función saludar se definen varias funciones: saludar_es, saludar_en y 
saludar_fr y a continuación se crea un diccionario que tiene como cla-
ves cadenas de texto que identifican a cada lenguaje, y como valores las 
funciones. El valor de retorno de la función es una de estas funciones. 
La función a devolver viene determinada por el valor del parámetro 
lang que se pasó como argumento de saludar.

Como el valor de retorno de saludar es una función, como hemos 
visto, esto quiere decir que f es una variable que contiene una función. 
Podemos entonces llamar a la función a la que se refiere f de la forma 
en que llamaríamos a cualquier otra función, añadiendo unos parénte-
sis y, de forma opcional, una serie de parámetros entre los paréntesis.

Esto se podría acortar, ya que no es necesario almacenar la función que 
nos pasan como valor de retorno en una variable para poder llamarla:

.. code-block:: nim

 >>> saludar(“en”)()
 Hi
 >>> saludar(“fr”)()
 Salut

En este caso el primer par de paréntesis indica los parámetros de la 
función saludar, y el segundo par, los de la función devuelta por salu-
dar.

**Iteraciones de orden superior sobre listas**
-----------------------

Una de las cosas más interesantes que podemos hacer con nuestras 
funciones de orden superior es pasarlas como argumentos de las fun-
ciones map, filter y reduce. Estas funciones nos permiten sustituir los 
bucles típicos de los lenguajes imperativos mediante construcciones 
equivalentes.

**map(function, sequence[, sequence, ...])**

La función map aplica una función a cada elemento de una secuencia y 
devuelve una lista con el resultado de aplicar la función a cada elemen-
to. Si se pasan como parámetros n secuencias, la función tendrá que 
aceptar n argumentos. Si alguna de las secuencias es más pequeña que 
las demás, el valor que le llega a la función function para posiciones 
mayores que el tamaño de dicha secuencia será None.

A continuación podemos ver un ejemplo en el que se utiliza map para 
elevar al cuadrado todos los elementos de una lista:

.. code-block:: nim

 def cuadrado(n):
    return n ** 2
 l = [1, 2, 3]
 l2 = map(cuadrado, l)

**filter(function, sequence)**

La funcion filter verifica que los elementos de una secuencia cum-
plan una determinada condición, devolviendo una secuencia con los 
elementos que cumplen esa condición. Es decir, para cada elemento de 
sequence se aplica la función function; si el resultado es True se añade 
a la lista y en caso contrario se descarta.

A continuación podemos ver un ejemplo en el que se utiliza filter 
para conservar solo los números que son pares.

.. code-block:: nim

 def es_par(n):
    return (n % 2.0 == 0)
 l = [1, 2, 3]
l2 = filter(es_par, l)

**reduce(function, sequence[, initial])**

La función reduce aplica una función a pares de elementos de una 
secuencia hasta dejarla en un solo valor.
A continuación podemos ver un ejemplo en el que se utiliza reduce 
para sumar todos los elementos de una lista.

.. code-block:: nim

 def sumar(x, y):
    return x + y
 l = [1, 2, 3]
 l2 = reduce(sumar, l)

**Funciones lambda**
-------------------

El operador lambda sirve para crear funciones anónimas en línea. Al ser 
funciones anónimas, es decir, sin nombre, estas no podrán ser referen-
ciadas más tarde.

Las funciones lambda se construyen mediante el operador lambda, los 
parámetros de la función separados por comas (atención, SIN parénte-
sis), dos puntos (:) y el código de la función.

Esta construcción podrían haber sido de utilidad en los ejemplos an-
teriores para reducir código. El programa que utilizamos para explicar 
filter, por ejemplo, podría expresarse así:

.. code-block:: nim

 l = [1, 2, 3]
 l2 = filter(lambda n: n % 2.0 == 0, l)

Comparemoslo con la versión anterior:

.. code-block:: nim

 def es_par(n):
    return (n % 2.0 == 0)
 l = [1, 2, 3]
 l2 = filter(es_par, l)

Las funciones lambda están restringidas por la sintaxis a una sola 
expresión.

**Comprensión de listas**
----------------

En Python 3000 map, filter y reduce perderán importancia. Y aun-
que estas funciones se mantendrán, reduce pasará a formar parte del 
módulo functools, con lo que quedará fuera de las funciones dispo-
nibles por defecto, y map y filter se desaconsejarán en favor de las list 
comprehensions o comprensión de listas.

La comprensión de listas es una característica tomada del lenguaje de 
programación funcional Haskell que está presente en Python desde la 
versión 2.0 y consiste en una construcción que permite crear listas a 
partir de otras listas.

Cada una de estas construcciones consta de una expresión que deter-
mina cómo modificar el elemento de la lista original, seguida de una o 
varias clausulas for y opcionalmente una o varias clausulas if.
Veamos un ejemplo de cómo se podría utilizar la comprensión de listas 
para elevar al cuadrado todos los elementos de una lista, como hicimos 
en nuestro ejemplo de map.

.. code-block:: nim

 l2 = [n ** 2 for n in l]

Esta expresión se leería como “para cada n en l haz n ** 2”. Como 
vemos tenemos primero la expresión que modifica los valores de la lista 
original (n ** 2), después el for, el nombre que vamos a utilizar para 
referirnos al elemento actual de la lista original, el in, y la lista sobre la 
que se itera.

El ejemplo que utilizamos para la función filter (conservar solo los 
números que son pares) se podría expresar con comprensión de listas 
así:
.. code-block:: nim

 l2 = [n for n in l if n % 2.0 == 0]

Veamos por último un ejemplo de compresión de listas con varias 
clausulas for:

.. code-block:: nim

 l = [0, 1, 2, 3]
 m = [“a”, “b”]
 n = [s * v for s in m
           for v in l
           if v > 0]

Esta construcción sería equivalente a una serie de for-in anidados:

.. code-block:: nim

 l = [0, 1, 2, 3]
 m = [“a”, “b”]
 n = []
 for s in m:
    for v in l:
        if v > 0:
            n.append(s* v)

**Generadores**

Las expresiones generadoras funcionan de forma muy similar a la 
comprensión de listas. De hecho su sintaxis es exactamente igual, a 
excepción de que se utilizan paréntesis en lugar de corchetes:

.. code-block:: nim

 l2 = (n ** 2 for n in l)
 
Sin embargo las expresiones generadoras se diferencian de la compren-
sión de listas en que no se devuelve una lista, sino un generador.

.. code-block:: nim

 >>> l2 = [n ** 2 for n in l]
 >>> l2
 [0, 1, 4, 9]
 >>> l2 = (n ** 2 for n in l)
 >>> l2
 <generator object at 0×00E33210>

Un generador es una clase especial de función que genera valores sobre 
los que iterar. Para devolver el siguiente valor sobre el que iterar se 
utiliza la palabra clave yield en lugar de return. Veamos por ejemplo 
un generador que devuelva números de n a m con un salto s.

.. code-block:: nim

 def mi_generador(n, m, s):
    while(n <= m):
        yield n
        n += s
 >>> x = mi_generador(0, 5, 1)
 >>> x
 <generator object at 0×00E25710>

El generador se puede utilizar en cualquier lugar donde se necesite un 
objeto iterable. Por ejemplo en un for-in:

.. code-block:: nim

 for n in mi_generador(0, 5, 1):
    print n

Como no estamos creando una lista completa en memoria, sino gene-
rando un solo valor cada vez que se necesita, en situaciones en las que 
no sea necesario tener la lista completa el uso de generadores puede 
suponer una gran diferencia de memoria. En todo caso siempre es po-
sible crear una lista a partir de un generador mediante la función list:

.. code-block:: nim

 lista = list(mi_generador)

**Decoradores**

Un decorador no es es mas que una función que recibe una función 
como parámetro y devuelve otra función como resultado. Por ejem-
plo podríamos querer añadir la funcionalidad de que se imprimiera el 
nombre de la función llamada por motivos de depuración:

.. code-block:: nim

 def mi_decorador(funcion):
    def nueva(*args):
        print “Llamada a la funcion”, funcion.__name__
        retorno = funcion(*args)
        return retorno
    return nueva

Como vemos el código de la función mi_decorador no hace más que 
crear una nueva función y devolverla. Esta nueva función imprime el 
nombre de la función a la que “decoramos”, ejecuta el código de dicha 
función, y devuelve su valor de retorno. Es decir, que si llamáramos 
a la nueva función que nos devuelve mi_decorador, el resultado sería 
el mismo que el de llamar directamente a la función que le pasamos 
como parámetro, exceptuando el que se imprimiría además el nombre 
de la función.

Supongamos como ejemplo una función imp que no hace otra cosa que 
mostrar en pantalla la cadena pasada como parámetro.

.. code-block:: nim

 >>> imp(“hola”)
 hola
 >>> mi_decorador(imp)(“hola”)
 Llamada a la función imp
 hola

La sintaxis para llamar a la función que nos devuelve mi_decorador no 
es muy clara, aunque si lo estudiamos detenidamente veremos que no 
tiene mayor complicación. Primero se llama a la función que decora 
con la función a decorar: mi_decorador(imp); y una vez obtenida la 
función ya decorada se la puede llamar pasando el mismo parámetro 
que se pasó anteriormente: mi_decorador(imp)(“hola”)

Esto se podría expresar más claramente precediendo la definición de la 
función que queremos decorar con el signo @ seguido del nombre de la 
función decoradora:

.. code-block:: nim

 @mi_decorador
 def imp(s):
    print s

De esta forma cada vez que se llame a imp se estará llamando realmen-
te a la versión decorada. Python incorpora esta sintaxis desde la versión 
2.4 en adelante.

Si quisiéramos aplicar más de un decorador bastaría añadir una nueva 
línea con el nuevo decorador.

.. code-block:: nim

 @otro_decorador
 @mi_decorador
 def imp(s):
    print s

Es importante advertir que los decoradores se ejecutarán de abajo a 
arriba. Es decir, en este ejemplo primero se ejecutaría mi_decorador y 
después otro_decorador.

**Excepciones**
-------------

Las excepciones son errores detectados por Python durante la eje-
cución del programa. Cuando el intérprete se encuentra con una 
situación excepcional, como el intentar dividir un número entre 0 o 
el intentar acceder a un archivo que no existe, este genera o lanza una 
excepción, informando al usuario de que existe algún problema.

Si la excepción no se captura el flujo de ejecución se interrumpe y se 
muestra la información asociada a la excepción en la consola de forma 
que el programador pueda solucionar el problema.

Veamos un pequeño programa que lanzaría una excepción al intentar 
dividir 1 entre 0.

.. code-block:: nim

 def division(a, b):
    return a / b
 def calcular():
    division(1, 0)
 calcular()

Si lo ejecutamos obtendremos el siguiente mensaje de error:

.. code-block:: nim

 $ python ejemplo.py
 Traceback (most recent call last):
 File “ejemplo.py”, line 7, in
 calcular()
 File “ejemplo.py”, line 5, in calcular
 division(1, 0)
 File “ejemplo.py”, line 2, in division
 a / b
 ZeroDivisionError: integer division or modulo by zero

Lo primero que se muestra es el trazado de pila o traceback, que con-
siste en una lista con las llamadas que provocaron la excepción. Como 
vemos en el trazado de pila, el error estuvo causado por la llamada a 
calcular() de la línea 7, que a su vez llama a division(1, 0) en la 
línea 5 y en última instancia por la ejecución de la sentencia a / b de 
la línea 2 de division.

A continuación vemos el tipo de la excepción, ZeroDivisionError, 
junto a una descripción del error: “integer division or modulo by zero” 
(módulo o división entera entre cero).
En Python se utiliza una construcción try-except para capturar y 
tratar las excepciones. El bloque try (intentar) define el fragmento de 
código en el que creemos que podría producirse una excepción. El blo-
que except (excepción) permite indicar el tratamiento que se llevará a 
cabo de producirse dicha excepción. Muchas veces nuestro tratamiento 
de la excepción consistirá simplemente en imprimir un mensaje más 
amigable para el usuario, otras veces nos interesará registrar los errores 
y de vez en cuando podremos establecer una estrategia de resolución 
del problema.

En el siguiente ejemplo intentamos crear un objeto f de tipo fichero. 
De no existir el archivo pasado como parámetro, se lanza una excep-
ción de tipo IOError, que capturamos gracias a nuestro try-except.

.. code-block:: nim

 try:
    f = file(“archivo.txt”)
 except:
    print “El archivo no existe”

Python permite utilizar varios except para un solo bloque try, de 
forma que podamos dar un tratamiento distinto a la excepción de-
pendiendo del tipo de excepción de la que se trate. Esto es una buena 
práctica, y es tan sencillo como indicar el nombre del tipo a continua-
ción del except.

.. code-block:: nim

 try:
    num = int(“3a”)
    print no_existe
 except NameError:
    print “La variable no existe”
 except ValueError:
    print “El valor no es un numero”

Cuando se lanza una excepción en el bloque try, se busca en cada una 
de las clausulas except un manejador adecuado para el tipo de error 
que se produjo. En caso de que no se encuentre, se propaga la excep-
ción.

Además podemos hacer que un mismo except sirva para tratar más 
de una excepción usando una tupla para listar los tipos de error que 
queremos que trate el bloque:

.. code-block:: nim

 try:
    num = int(“3a”)
    print no_existe
 except (NameError, ValueError):
    print “Ocurrio un error”

La construcción try-except puede contar además con una clausula 
else, que define un fragmento de código a ejecutar sólo si no se ha 
producido ninguna excepción en el try.

.. code-block:: nim

 try:
    num = 33
 except:
    print “Hubo un error!”
 else:
    print “Todo esta bien”

También existe una clausula finally que se ejecuta siempre, se pro-
duzca o no una excepción. Esta clausula se suele utilizar, entre otras 
cosas, para tareas de limpieza.

.. code-block:: nim

 try:
    z = x / y
 except ZeroDivisionError:
    print “Division por cero”
 finally:
    print “Limpiando”

También es interesante comentar que como programadores podemos 
crear y lanzar nuestras propias excepciones. Basta crear una clase que 
herede de Exception o cualquiera de sus hijas y lanzarla con raise.
class MiError(Exception):

.. code-block:: nim

    def __init__(self, valor):
        self.valor = valor

    def __str__(self):
        return “Error “ + str(self.valor)
 try:
    if resultado > 20:
        raise MiError(33)
 except MiError, e:
    print e

Por último, a continuación se listan a modo de referencia las excepcio-
nes disponibles por defecto, así como la clase de la que deriva cada una 
de ellas entre paréntesis.

BaseException: Clase de la que heredan todas las excepciones.
Exception(BaseException): Super clase de todas las excepciones que 
no sean de salida.

GeneratorExit(Exception): Se pide que se salga de un generador.

StandardError(Exception): Clase base para todas las excepciones que 
no tengan que ver con salir del intérprete.

ArithmeticError(StandardError): Clase base para los errores aritmé-
ticos.

FloatingPointError(ArithmeticError): Error en una operación de 
coma flotante.

OverflowError(ArithmeticError): Resultado demasiado grande para 
poder representarse.

ZeroDivisionError(ArithmeticError): Lanzada cuando el segundo 
argumento de una operación de división o módulo era 0.

AssertionError(StandardError): Falló la condición de un estamento 
assert.

AttributeError(StandardError): No se encontró el atributo.

EOFError(StandardError): Se intentó leer más allá del final de fichero.

EnvironmentError(StandardError): Clase padre de los errores relacio-
nados con la entrada/salida.

IOError(EnvironmentError): Error en una operación de entrada/salida.

OSError(EnvironmentError): Error en una llamada a sistema.

WindowsError(OSError): Error en una llamada a sistema en Windows.

ImportError(StandardError): No se encuentra el módulo o el elemen-
to del módulo que se quería importar.

LookupError(StandardError): Clase padre de los errores de acceso.

IndexError(LookupError): El índice de la secuencia está fuera del 
rango posible.

KeyError(LookupError): La clave no existe.

MemoryError(StandardError): No queda memoria suficiente.

NameError(StandardError): No se encontró ningún elemento con ese 
nombre.

UnboundLocalError(NameError): El nombre no está asociado a ninguna 
variable.

ReferenceError(StandardError): El objeto no tiene ninguna referen-
cia fuerte apuntando hacia él.

RuntimeError(StandardError): Error en tiempo de ejecución no espe-
cificado.

NotImplementedError(RuntimeError): Ese método o función no está 
implementado.

SyntaxError(StandardError): Clase padre para los errores sintácticos.

IndentationError(SyntaxError): Error en la indentación del archivo.

TabError(IndentationError): Error debido a la mezcla de espacios y 
tabuladores.

SystemError(StandardError): Error interno del intérprete.

TypeError(StandardError): Tipo de argumento no apropiado.

ValueError(StandardError): Valor del argumento no apropiado.

UnicodeError(ValueError): Clase padre para los errores relacionados 
con unicode.

UnicodeDecodeError(UnicodeError): Error de decodificación unicode.

UnicodeEncodeError(UnicodeError): Error de codificación unicode.

UnicodeTranslateError(UnicodeError): Error de traducción unicode.

StopIteration(Exception): Se utiliza para indicar el final del iterador.

Warning(Exception): Clase padre para los avisos.

DeprecationWarning(Warning): Clase padre para avisos sobre caracte-
rísticas obsoletas.

FutureWarning(Warning): Aviso. La semántica de la construcción cam-
biará en un futuro.

ImportWarning(Warning): Aviso sobre posibles errores a la hora de 
importar.

PendingDeprecationWarning(Warning): Aviso sobre características que 
se marcarán como obsoletas en un futuro próximo.

RuntimeWarning(Warning): Aviso sobre comportmaientos dudosos en 
tiempo de ejecución.

SyntaxWarning(Warning): Aviso sobre sintaxis dudosa.

UnicodeWarning(Warning): Aviso sobre problemas relacionados con 
Unicode, sobre todo con problemas de conversión.

UserWarning(Warning): Clase padre para avisos creados por el progra-
mador.

KeyboardInterrupt(BaseException): El programa fué interrumpido 
por el usuario.

SystemExit(BaseException): Petición del intérprete para terminar la 
ejecución.

**Módulos y paquetes**
--------

**modulos**

Para facilitar el mantenimiento y la lectura los programas demasiado 
largos pueden dividirse en módulos, agrupando elementos relaciona-
dos. Los módulos son entidades que permiten una organización y divi-
sión lógica de nuestro código. Los ficheros son su contrapartida física: 
cada archivo Python almacenado en disco equivale a un módulo.

Vamos a crear nuestro primer módulo entonces creando un pequeño 
archivo modulo.py con el siguiente contenido:

.. code-block:: nim

 def mi_funcion():
    print “una funcion”
 class MiClase:
    def __init__(self):
        print “una clase”
 print “un modulo”

Si quisiéramos utilizar la funcionalidad definida en este módulo en 
nuestro programa tendríamos que importarlo. Para importar un mó-
dulo se utiliza la palabra clave import seguida del nombre del módulo, 
que consiste en el nombre del archivo menos la extensión. Como ejem-
plo, creemos un archivo programa.py en el mismo directorio en el que 
guardamos el archivo del módulo (esto es importante, porque si no se 
encuentra en el mismo directorio Python no podrá encontrarlo), con el 
siguiente contenido:

.. code-block:: nim

 import modul
 modulo.mi_funcion()

El import no solo hace que tengamos disponible todo lo definido 
dentro del módulo, sino que también ejecuta el código del módulo. Por 
esta razón nuestro programa, además de imprimir el texto “una fun-
cion” al llamar a mi_funcion, también imprimiría el texto “un modulo”, 
debido al print del módulo importado. No se imprimiría, no obstante, 
el texto “una clase”, ya que lo que se hizo en el módulo fue tan solo 
definir de la clase, no instanciarla.

La clausula import también permite importar varios módulos en la 
misma línea. En el siguiente ejemplo podemos ver cómo se importa 
con una sola clausula import los módulos de la distribución por defecto 
de Python os, que engloba funcionalidad relativa al sistema operativo; 
sys, con funcionalidad relacionada con el propio intérprete de Python 
y time, en el que se almacenan funciones para manipular fechas y 
horas.

.. code-block:: nim

 import os, sys, time
 print time.asctime()

Sin duda os habréis fijado en este y el anterior ejemplo en un detalle 
importante, y es que, como vemos, es necesario preceder el nombre de 
los objetos que importamos de un módulo con el nombre del módulo 
al que pertenecen, o lo que es lo mismo, el espacio de nombres en el 
que se encuentran. Esto permite que no sobreescribamos accidental-
mente algún otro objeto que tuviera el mismo nombre al importar otro 
módulo.

Sin embargo es posible utilizar la construcción from-import para 
ahorrarnos el tener que indicar el nombre del módulo antes del objeto 
que nos interesa. De esta forma se importa el objeto o los objetos que 
indiquemos al espacio de nombres actual.

.. code-block:: nim

 from time import asctime
 print asctime()

Aunque se considera una mala práctica, también es posible importar 
todos los nombres del módulo al espacio de nombres actual usando el 
caracter *:

.. code-block:: nim

 from time import *

Ahora bien, recordareis que a la hora de crear nuestro primer módulo 
insistí en que lo guardarais en el mismo directorio en el que se en-
contraba el programa que lo importaba. Entonces, ¿cómo podemos 
importar los módulos os, sys o time si no se encuentran los archivos 
os.py, sys.py y time.py en el mismo directorio?

A la hora de importar un módulo Python recorre todos los directorios 
indicados en la variable de entorno PYTHONPATH en busca de un archivo 
con el nombre adecuado. El valor de la variable PYTHONPATH se puede 
consultar desde Python mediante sys.path

.. code-block:: nim

 >>> import sys
 >>> sys.path

De esta forma para que nuestro módulo estuviera disponible para 
todos los programas del sistema bastaría con que lo copiáramos a uno 
de los directorios indicados en PYTHONPATH.

En el caso de que Python no encontrara ningún módulo con el nom-
bre especificado, se lanzaría una excepción de tipo ImportError.

Por último es interesante comentar que en Python los módulos 
también son objetos; de tipo module en concreto. Por supuesto esto 
significa que pueden tener atributos y métodos. Uno de sus atributos, 
__name__, se utiliza a menudo para incluir código ejecutable en un 
módulo pero que este sólo se ejecute si se llama al módulo como pro-
grama, y no al importarlo. Para lograr esto basta saber que cuando se 
ejecuta el módulo directamente __name__ tiene como valor “__main__”, 
mientras que cuando se importa, el valor de __name__ es el nombre del 
módulo:

.. code-block:: nim

 print “Se muestra siempre”
 if __name__ == “__main__”:
    print “Se muestra si no es importacion”

Otro atributo interesante es __doc__, que, como en el caso de fun-
ciones y clases, sirve a modo de documentación del objeto (docstring 
o cadena de documentación). Su valor es el de la primera línea del 
cuerpo del módulo, en el caso de que esta sea una cadena de texto; en 
caso contrario valdrá None.

**Paquetes**

Si los módulos sirven para organizar el código, los paquetes sirven para 
organizar los módulos. Los paquetes son tipos especiales de módulos 
(ambos son de tipo module) que permiten agrupar módulos relacio-
nados. Mientras los módulos se corresponden a nivel físico con los 
archivos, los paquetes se representan mediante directorios.
En una aplicación cualquiera podríamos tener, por ejemplo, un paque-
te iu para la interfaz o un paquete bbdd para la persistencia a base de 
datos.

Para hacer que Python trate a un directorio como un paquete es nece-
sario crear un archivo __init__.py en dicha carpeta. En este archivo se 
pueden definir elementos que pertenezcan a dicho paquete, como una 
constante DRIVER para el paquete bbdd, aunque habitualmente se trata-
rá de un archivo vacío. Para hacer que un cierto módulo se encuentre 
dentro de un paquete, basta con copiar el archivo que define el módulo 
al directorio del paquete.

Como los modulos, para importar paquetes también se utiliza import 
y from-import y el caracter . para separar paquetes, subpaquetes y 
módulos.

.. code-block:: nim

 import paq.subpaq.modulo
 paq.subpaq.modulo.func()

A lo largo de los próximos capítulos veremos algunos módulos y pa-
quetes de utilidad. Para encontrar algún módulo o paquete que cubra 
una cierta necesidad, puedes consultar la lista de PyPI (Python Pac-
kage Index) en http://pypi.python.org/, que cuenta a la hora de escribir 
estas líneas, con más de 4000 paquetes distintos.

**entrada/salida y fiCheros**
---------

Nuestros programas serían de muy poca utilidad si no fueran capaces 
de interaccionar con el usuario. En capítulos anteriores vimos, de pasa-
da, el uso de la palabra clave print para mostrar mensajes en pantalla.
En esta lección, además de describir más detalladamente del uso de 
print para mostrar mensajes al usuario, aprenderemos a utilizar las 
funciones input y raw_input para pedir información, así como los 
argumentos de línea de comandos y, por último, la entrada/salida de 
ficheros.

**Entrada estándar**

La forma más sencilla de obtener información por parte del usuario 
es mediante la función raw_input. Esta función toma como paráme-
tro una cadena a usar como prompt (es decir, como texto a mostrar al 
usuario pidiendo la entrada) y devuelve una cadena con los caracteres 
introducidos por el usuario hasta que pulsó la tecla Enter. Veamos un 
pequeño ejemplo:

.. code-block:: nim

 nombre = raw_input(“Como te llamas? “)
 print “Encantado, “ + nombre

Si necesitáramos un entero como entrada en lugar de una cadena, por 
ejemplo, podríamos utilizar la función int para convertir la cadena a 
entero, aunque sería conveniente tener en cuenta que puede lanzarse 
una excepción si lo que introduce el usuario no es un número.

.. code-block:: nim

 try:
    edad = raw_input(“Cuantos anyos tienes? “)
    dias = int(edad) * 365
    print “Has vivido “ + str(dias) + “ dias”
 except ValueError:
    print “Eso no es un numero”

La función input es un poco más complicada. Lo que hace esta fun-
ción es utilizar raw_input para leer una cadena de la entrada estándar, 
y después pasa a evaluarla como si de código Python se tratara; por lo 
tanto input debería tratarse con sumo cuidado.

**Parámetros de línea de comando**

Además del uso de input y raw_input el programador Python cuen-
ta con otros métodos para obtener datos del usuario. Uno de ellos es 
el uso de parámetros a la hora de llamar al programa en la línea de 
comandos. Por ejemplo:

.. code-block:: nim

 python editor.py hola.txt

En este caso hola.txt sería el parámetro, al que se puede acceder a 
través de la lista sys.argv, aunque, como es de suponer, antes de poder 
utilizar dicha variable debemos importar el módulo sys. sys.argv[0] 
contiene siempre el nombre del programa tal como lo ha ejecutado el 
usuario, sys.argv[1], si existe, sería el primer parámetro; sys.argv[2] 
el segundo, y así sucesivamente.

.. code-block:: nim

 import sys
 if(len(sys.argv) > 1):
    print “Abriendo “ + sys.argv[1]
 else:
    print “Debes indicar el nombre del archivo”

Existen módulos, como optparse, que facilitan el trabajo con los argu-
mentos de la línea de comandos, pero explicar su uso queda fuera del 
objetivo de este capítulo.

**Salida estándar**

La forma más sencilla de mostrar algo en la salida estándar es median-
te el uso de la sentencia print, como hemos visto multitud de veces en 
ejemplos anteriores. En su forma más básica a la palabra clave print le 
sigue una cadena, que se mostrará en la salida estándar al ejecutarse el 
estamento.

.. code-block:: nim

 >>> print “Hola mundo”
 Hola mundo

Después de imprimir la cadena pasada como parámetro el puntero se 
sitúa en la siguiente línea de la pantalla, por lo que el print de Python 
funciona igual que el println de Java.

En algunas funciones equivalentes de otros lenguajes de programación 
es necesario añadir un carácter de nueva línea para indicar explícita-
mente que queremos pasar a la siguiente línea. Este es el caso de la 
función printf de C o la propia función print de Java.

Ya explicamos el uso de estos caracteres especiales durante la explica-
ción del tipo cadena en el capítulo sobre los tipos básicos de Python. 
La siguiente sentencia, por ejemplo, imprimiría la palabra “Hola”, 
seguida de un renglón vacío (dos caracteres de nueva línea, ‘\n’), y 
a continuación la palabra “mundo” indentada (un carácter tabulador, 
‘\t’).

.. code-block:: nim

 print “Hola\n\n\tmundo”

Para que la siguiente impresión se realizara en la misma línea tendría-
mos que colocar una coma al final de la sentencia. Comparemos el 
resultado de este código:

.. code-block:: nim

 >>> for i in range(3):
 >>> ...print i,
 0 1 2

Con el de este otro, en el que no utiliza una coma al final de la senten-
cia:

.. code-block:: nim

 >>> for i in range(3):
 >>> ...print i
 0
 1
 2

Este mecanismo de colocar una coma al final de la sentencia funcio-
na debido a que es el símbolo que se utiliza para separar cadenas que 
queramos imprimir en la misma línea.

.. code-block:: nim

 >>> print “Hola”, “mundo”
 Hola mundo

Esto se diferencia del uso del operador + para concatenar las cadenas 
en que al utilizar las comas print introduce automáticamente un espa-
cio para separar cada una de las cadenas. Este no es el caso al utilizar 
el operador +, ya que lo que le llega a print es un solo argumento: una 
cadena ya concatenada.

.. code-block:: nim
 >>> print “Hola” + “mundo”
 Holamundo

Además, al utilizar el operador + tendríamos que convertir antes cada 
argumento en una cadena de no serlo ya, ya que no es posible concate-
nar cadenas y otros tipos, mientras que al usar el primer método no es 
necesaria la conversión.

.. code-block:: nim

 >>> print “Cuesta”, 3, “euros”
 Cuesta 3 euros
 >>> print “Cuesta” + 3 + “euros”
 <type ‘exceptions.TypeError’>: cannot concatenate ‘str’ and 
 ‘int’ objects

La sentencia print, o más bien las cadenas que imprime, permiten 
también utilizar técnicas avanzadas de formateo, de forma similar al 
sprintf de C. Veamos un ejemplo bastante simple:

.. code-block:: nim

 print “Hola %s” % “mundo”
 print “%s %s” % (“Hola”, “mundo”)

Lo que hace la primera línea es introducir los valores a la derecha del 
símbolo % (la cadena “mundo”) en las posiciones indicadas por los espe-
cificadores de conversión de la cadena a la izquierda del símbolo %, tras 
convertirlos al tipo adecuado.

En la segunda línea, vemos cómo se puede pasar más de un valor a 
sustituir, por medio de una tupla.

En este ejemplo sólo tenemos un especificador de conversión: %s.
Los especificadores más sencillos están formados por el símbolo % 
seguido de una letra que indica el tipo con el que formatear el valor 
Por ejemplo:

============= ==============
Especificador  Formato
============= ==============
%s             Cadena
%d             Entero
%o             Octal
%x             Hexadecimal
%f             Real
============= ==============

Se puede introducir un número entre el % y el carácter que indica el 
tipo al que formatear, indicando el número mínimo de caracteres que 
queremos que ocupe la cadena. Si el tamaño de la cadena resultante 
es menor que este número, se añadirán espacios a la izquierda de la 
cadena. En el caso de que el número sea negativo, ocurrirá exactamente 
lo mismo, sólo que los espacios se añadirán a la derecha de la cadena.

.. code-block:: nim

 >>> print “%10s mundo” % “Hola”
 ______Hola mundo
 >>> print “%-10s mundo” % “Hola”
 Hola_______mundo

En el caso de los reales es posible indicar la precisión a utilizar prece-
diendo la f de un punto seguido del número de decimales que quere-
mos mostrar:

.. code-block:: nim

 >>> from math import pi
 >>> print “%.4f” % pi
 3.1416

La misma sintaxis se puede utilizar para indicar el número de caracte-
res de la cadena que queremos mostrar

.. code-block:: nim

 >>> print “%.4s” % “hola mundo”
 hola

**Archivos**

Los ficheros en Python son objetos de tipo file creados mediante la 
función open (abrir). Esta función toma como parámetros una cadena 
con la ruta al fichero a abrir, que puede ser relativa o absoluta; una 
cadena opcional indicando el modo de acceso (si no se especifica se 
accede en modo lectura) y, por último, un entero opcional para especi-
ficar un tamaño de buffer distinto del utilizado por defecto.
El modo de acceso puede ser cualquier combinación lógica de los 
siguientes modos:

* ‘r’: read, lectura. Abre el archivo en modo lectura. El archivo tiene 
que existir previamente, en caso contrario se lanzará una excepción 
de tipo IOError.

* ‘w’: write, escritura. Abre el archivo en modo escritura. Si el archi-
vo no existe se crea. Si existe, sobreescribe el contenido.

* ‘a’: append, añadir. Abre el archivo en modo escritura. Se diferen-
cia del modo ‘w’ en que en este caso no se sobreescribe el conteni-
do del archivo, sino que se comienza a escribir al final del archivo.

* ‘b’: binary, binario.

* ‘+’: permite lectura y escritura simultáneas.

* ‘U’: universal newline, saltos de línea universales. Permite trabajar 
con archivos que tengan un formato para los saltos de línea que no 
coincide con el de la plataforma actual (en Windows se utiliza el 
caracter CR LF, en Unix LF y en Mac OS CR).

.. code-block:: nim

 f = open(“archivo.txt”, “w”)

Tras crear el objeto que representa nuestro archivo mediante la función 
open podremos realizar las operaciones de lectura/escritura pertinen-
tes utilizando los métodos del objeto que veremos en las siguientes 
secciones.

Una vez terminemos de trabajar con el archivo debemos cerrarlo utili-
zando el método close.

**Lectura de archivos**

Para la lectura de archivos se utilizan los métodos read, readline y 
realines.

El método read devuelve una cadena con el contenido del archivo o 
bien el contenido de los primeros n bytes, si se especifica el tamaño 
máximo a leer.

.. code-block:: nim

 completo = f.read()
 parte = f2.read(512)

El método readline sirve para leer las líneas del fichero una por una. 
Es decir, cada vez que se llama a este método, se devuelve el conteni-
do del archivo desde el puntero hasta que se encuentra un carácter de 
nueva línea, incluyendo este carácter.

.. code-block:: nim

 while True:
      linea = f.readline()
      if not linea: break
      print linea


Por último, readlines, funciona leyendo todas las líneas del archivo y 
devolviendo una lista con las líneas leídas.

**Escritura de archivos**

Para la escritura de archivos se utilizan los método write y writelines. 
Mientras el primero funciona escribiendo en el archivo una cadena de 
texto que toma como parámetro, el segundo toma como parámetro una 
lista de cadenas de texto indicando las líneas que queremos escribir en 
el fichero.

**Mover el puntero de lectura/escritura**

Hay situaciones en las que nos puede interesar mover el puntero de 
lectura/escritura a una posición determinada del archivo. Por ejemplo 
si queremos empezar a escribir en una posición determinada y no al 
final o al principio del archivo.

Para esto se utiliza el método seek que toma como parámetro un nú-
mero positivo o negativo a utilizar como desplazamiento. También es 
posible utilizar un segundo parámetro para indicar desde dónde quere-
mos que se haga el desplazamiento: 0 indicará que el desplazamiento 
se refiere al principio del fichero (comportamiento por defecto), 1 se 
refiere a la posición actual, y 2, al final del fichero.

Para determinar la posición en la que se encuentra actualmente el 
puntero se utiliza el método tell(), que devuelve un entero indicando 
la distancia en bytes desde el principio del fichero.

**expresiones regulares**
-----------

Las expresiones regulares, también llamadas regex o regexp, consisten 
en patrones que describen conjuntos de cadenas de caracteres.

Algo parecido sería escribir en la línea de comandos de Windows

.. code-block:: nim

 dir *.exe

‘*.exe’ sería una “expresión regular” que describiría todas las cadenas 
de caracteres que empiezan con cualquier cosa seguida de ‘.exe’, es 
decir, todos los archivos exe.

El trabajo con expresiones regulares en Python se realiza mediante el 
módulo re, que data de Python 1.5 y que proporciona una sintaxis para 
la creación de patrones similar a la de Perl. En Python 1.6 el módulo 
se reescribió para dotarlo de soporte de cadenas unicode y mejorar su 
rendimiento.

El módulo re contiene funciones para buscar patrones dentro de una 
cadena (search), comprobar si una cadena se ajusta a un determinado 
criterio descrito mediante un patrón (match), dividir la cadena usando 
las ocurrencias del patrón como puntos de ruptura (split) o para sus-
tituir todas las ocurrencias del patrón por otra cadena (sub). Veremos 
estas funciones y alguna más en la próxima sección, pero por ahora, 
aprendamos algo más sobre la sintaxis de las expresiones regulares.

**patrones**

La expresión regular más sencilla consiste en una cadena simple, que
describe un conjunto compuesto tan solo por esa misma cadena. Por 
ejemplo, veamos cómo la cadena “python” coincide con la expresión 
regular “python” usando la función match:

.. code-block:: nim

 import re
 if re.match(“python”, “python”):
   print “cierto”

Si quisiéramos comprobar si la cadena es “python”,  “jython”, 
“cython” o cualquier otra cosa que termine en “ython”, podríamos 
utilizar el carácter comodín, el punto ‘.’:

.. code-block:: nim

 re.match(“.ython”, “python”)
 re.match(“.ython”, “jython”)

La expresión regular “.ython” describiría a todas las cadenas que con-
sistan en un carácter cualquiera, menos el de nueva línea, seguido de 
“ython”. Un carácter cualquiera y solo uno. No cero, ni dos, ni tres.
En el caso de que necesitáramos el carácter ‘.’ en la expresión regular, 
o cualquier otro de los caracteres especiales que veremos a continua-
ción, tendríamos que escaparlo utilizando la barra invertida.

Para comprobar si la cadena consiste en 3 caracteres seguidos de un 
punto, por ejemplo, podríamos utilizar lo siguiente:

.. code-block:: nim

 re.match(“...\.”, “abc.”)

Si necesitáramos una expresión que sólo resultara cierta para las cade-
nas “python”, “jython” y “cython” y ninguna otra, podríamos utilizar 
el carácter ‘|’ para expresar alternativa escribiendo los tres subpatro-
nes completos:

.. code-block:: nim

 re.match(“python|jython|cython”, “python”)

o bien tan solo la parte que pueda cambiar, encerrada entre paréntesis, 
formando lo que se conoce como un grupo. Los grupos tienen una 
gran importancia a la hora de trabajar con expresiones regulares y este 
no es su único uso, como veremos en la siguiente sección.

.. code-block:: nim

 re.match(“(p|j|c)ython”, “python”)

Otra opción consistiría en encerrar los caracteres ‘p’, ‘j’ y ‘c’ entre 
corchetes para formar una clase de caracteres, indicando que en esa po-
sición puede colocarse cualquiera de los caracteres de la clase.

.. code-block:: nim

 re.match(“[pjc]ython”, “python”)

¿Y si quisiéramos comprobar si la cadena es “python0”, “python1”, 
“python2”, ... , “python9”? En lugar de tener que encerrar los 10 dígitos 
dentro de los corchetes podemos utilizar el guión, que sirve para indi-
car rangos. Por ejemplo a-d indicaría todas las letras minúsculas de la 
‘a’ a la ‘d’; 0-9 serían todos los números de 0 a 9 inclusive.

.. code-block:: nim

 re.match(“python[0-9]”, “python0”)

Si quisiéramos, por ejemplo, que el último carácter fuera o un dígito o 
una letra simplemente se escribirían dentro de los corchetes todos los 
criterios, uno detras de otro.

.. code-block:: nim

 re.match(“python[0-9a-zA-Z]”, “pythonp”)

Es necesario advertir que dentro de las clases de caracteres los caracte-
res especiales no necesitan ser escapados. Para comprobar si la cadena 
es “python.” o “python,”, entonces, escribiríamos:

.. code-block:: nim

 re.match(“python[.,]”, “python.”)

y no

.. code-block:: nim

 re.match(“python[\.,]”, “python.”)

ya que en este último caso estaríamos comprobando si la cadena es 
“python.”, “python,” o “python\”.

Los conjuntos de caracteres también se pueden negar utilizando el 
símbolo ‘^’. La expresión “python[^0-9a-z]”, por ejemplo, indicaría 
que nos interesan las cadenas que comiencen por “python” y tengan 
como último carácter algo que no sea ni una letra minúscula ni un 
número.

.. code-block:: nim

 re.match(“python[^0-9a-z]”, “python+”)

El uso de [0-9] para referirse a un dígito no es muy común, ya que, al 
ser la comprobación de que un carácter es un dígito algo muy utilizado, 
existe una secuencia especial equivalente: ‘\d’. Existen otras secuen-
cias disponibles que listamos a continuación:

.. code-block:: nim

 “\d”: un dígito. Equivale a [0-9]
 “\D”: cualquier carácter que no sea un dígito. Equivale a [^0-9]
 “\w”: cualquier caracter alfanumérico. Equivale a [a-zA-Z0-9_]
 “\W”: cualquier carácter no alfanumérico. Equivale a [^a-zA-
 Z0-9_]
 “\s”: cualquier carácter en blanco. Equivale a [ \t\n\r\f\v]
 “\S”: cualquier carácter que no sea un espacio en blanco. Equivale 
 a [^ \t\n\r\f\v]

Veamos ahora cómo representar repeticiones de caracteres, dado que 
no sería de mucha utilidad tener que, por ejemplo, escribir una expre-
sión regular con 30 caracteres ‘\d’ para buscar números de 30 dígitos. 
Para este menester tenemos los caracteres especiales +, * y ?, además de 
las llaves {}.

El carácter + indica que lo que tenemos a la izquierda, sea un carác-
ter como ‘a’, una clase como ‘[abc]’ o un subpatrón como (abc), 
puede encontrarse una o mas veces. Por ejemplo la expresión regular 
“python+” describiría las cadenas “python”, “pythonn” y “pythonnn”, 
pero no “pytho”, ya que debe haber al menos una n.

El carácter * es similar a +, pero en este caso lo que se sitúa a su iz-
quierda puede encontrarse cero o mas veces.

El carácter ? indica opcionalidad, es decir, lo que tenemos a la izquier-
da puede o no aparecer (puede aparecer 0 o 1 veces).

Finalmente las llaves sirven para indicar el número de veces exacto que 
puede aparecer el carácter de la izquierda, o bien un rango de veces que 
puede aparecer. Por ejemplo {3} indicaría que tiene que aparecer exac-
tamente 3 veces, {3,8} indicaría que tiene que aparecer de 3 a 8 veces, 
