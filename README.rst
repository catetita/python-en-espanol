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



