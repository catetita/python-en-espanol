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
