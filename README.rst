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


Las cadenas también admiten operadores como +, que funciona reali-
zando una concatenación de las cadenas utilizadas como operandos y 
*, en la que se repite la cadena tantas veces como lo indique el número 
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
se de un signo *:

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


También se puede preceder el nombre del último parámetro con **, en 
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


