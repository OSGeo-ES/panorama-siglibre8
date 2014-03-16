**************
Bases de datos
**************

Autores
----------

- |delawen|

Introducción
---------------

Una base de datos espacial es una base de datos que se ha optimizado para almacenar y consultar datos que representa los objetos definidos en un espacio geométrico. La mayoría de las bases de datos espaciales permiten representar objetos geométricos simples, tales como puntos, líneas y polígonos. Algunas bases de datos espaciales manejan estructuras más complejas, tales como objetos en tres dimensiones, coberturas topológicas, redes lineales, y TIN.

Aunque a día de hoy existen bases de datos NoSQL que también empiezan a soportar funcionalidades geométricas, en este artículo vamos a centrarnos únicamente en las bases de datos clásicas, dado que son las que tienen, con mucha diferencia, la implementación más madura.

Software
----------

//TODo esto viene copiado directamente del wiki, darle formato y traducir.

This database extensions are usually based on a basic geometric data type you can operate with. The only background you really need to use this geometric database extensions is the same as working with any database.

.. note:: borrada tabla del wiki

=== Compliance with [http://www.opengeospatial.org/standards/sfs Simple Feature Access OGC Standard] ===

.. note:: borrada tabla del wiki


Puntos calientes
------------------

El Open Geospatial Consortium (OGC) ha desarrollado el estándar Simple Feature y establece normas para las funcionalidades espaciales de los sistemas de bases de datos. También llamada norma ISO 19125, se presenta en dos partes:

La primera parte, la norma ISO 19125-1 (SFA-CA para la "arquitectura común"), define un modelo de características simples de dos dimensiones, con interpolación lineal entre vértices. El modelo de datos definido en SFA-CA es una jerarquía de clases. Esta parte también define la representación utilizando WKT (well known text) y WKB (well known binary). Este tipo de datos contiene no sólo las coordenadas del objeto a representar, sino que también contiene referencias a la proyección utilizada y otras características que pudieran resultar de interés a la hora de operar con dichas geometrías.

La segunda parte de la norma ISO 19125-2 (SFA-SQL), define una serie de funcionalidades utilizando SQL. Estas funcionalidades abarcan la mayoría de las operaciones típicas que pueden llevarse a cabo con datos geográficos:

* Mediciones Espaciales: Para calcular la longitud de una línea, el área de un polígono, la distancia entre geometrías,...
* Funciones Espaciales: Modificar geometrías existentes para crear nuevas, es decir, operar con geometrías para obtener nuevas geometrías (intersección, buffering,...)
* Predicados Espaciales: Devuelven un booleano (verdadero/falso) acerca de la condición de una o más geometrías espaciales. Por ejemplo, si dos geometrías interseccionan o si están dentro de un buffer.
* Creación de Geometrías: Normalmente en base a una lista de coordenadas, se genera una nueva geometrías.
* Descripción de Geometrías: Devuelven información específica acerca de una geometría, por ejemplo qué punto es el centro de un círculo.



Curva de aprendizaje y conocimientos previos
------------------------------------------------

Dado que la mayoría de las bases de datos con extensiones espaciales siguen un mismo estándar, la programación y uso de dichas extensiones es muy similar de una plataforma a otra.

.. todo:: poner algo más

Documentación
----------------

Enlace al wiki y quizás alguna sugerencia particular en alguna sección.

.. todo:: poner bonito

http://en.wikipedia.org/wiki/Spatial_database


