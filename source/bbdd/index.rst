**************
Bases de datos
**************

Introducción
---------------

Una base de datos espacial es una base de datos que se ha optimizado para almacenar y consultar datos que representa los objetos definidos en un espacio geométrico. La mayoría de las bases de datos espaciales permiten representar objetos geométricos simples, tales como puntos, líneas y polígonos. Algunas bases de datos espaciales manejan estructuras más complejas, tales como objetos en tres dimensiones, coberturas topológicas, redes lineales, y TIN. 

Aunque a día de hoy existen bases de datos NoSQL que también empiezan a soportar funcionalidades geométricas, en este artículo vamos a centrarnos únicamente en las bases de datos clásicas, dado que son las que tienen, con mucha diferencia, la implementación más madura.

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

Software
----------

//TODo esto viene copiado directamente del wiki, darle formato y traducir.

This database extensions are usually based on a basic geometric data type you can operate with. The only background you really need to use this geometric database extensions is the same as working with any database.

{| class="wikitable sortable"  style="text-align: center;"
! Name
! Year
! OSGeo
! Live
! License
! Ohloh
! Tech
|-
| [http://postgis.net/ PostGIS]
| 2005
| {{yes|G}}
| {{yes|✓}}
| [http://opensource.org/licenses/gpl-2.0.php GPL v2]
| [http://www.ohloh.net/p/postgis ohloh]
| C/C++
|-
| [https://dev.mysql.com/doc/refman/5.0/es/spatial-extensions.html MySQL Spatial]
| ???
| {{no|☹}}
| {{no|☹}}
| [http://www.mysql.com/about/legal/licensing/oem/ Oracle]
| [http://www.ohloh.net/p/mysql ohloh]
| C/C++
|-
| [http://www.gaia-gis.it/gaia-sins/ Spatialite]
| 2008
| {{no|☹}}
| {{no|☹}}
| [https://www.gaia-gis.it/fossil/libspatialite/index  MPL tri-license]
| [http://www.ohloh.net/p/spatialite ohloh]
| C/C++
|-
| [http://www.h2gis.org/ H2GIS]
| 2008
| {{no|☹}}
| {{no|☹}}
| [https://github.com/irstv/H2GIS GPL3]
| {{no|☹}}
| Java
|-
|}

=== Compliance with [http://www.opengeospatial.org/standards/sfs Simple Feature Access OGC Standard] ===


{| class="wikitable sortable"  style="text-align: center;"
! Name
! Binary Geometry
! Normalized Geometry
! Types and Functions
|-
| [http://postgis.net/ PostGIS]
| {{yes|✓}}
| {{yes|✓}}
| {{yes|✓}}
|-
| [https://dev.mysql.com/doc/refman/5.0/es/spatial-extensions.html MySQL Spatial]
| {{no|☹}}
| {{no|☹}}
| {{yes|☹}}<ref name="partially">Partially supported</ref>
|-
| [http://www.gaia-gis.it/gaia-sins/ Spatialite]
| {{yes|✓}}
| {{yes|✓}}
| {{yes|✓}}
|-
| [http://www.h2gis.org/ H2GIS]
| {{yes|✓}}
| {{yes|✓}}
| {{yes|✓}}
|-
|}
<references/>


Curva de aprendizaje y conocimientos previos
------------------------------------------------

Dado que la mayoría de las bases de datos con extensiones espaciales siguen un mismo estándar, la programación y uso de dichas extensiones es muy similar de una plataforma a otra. 

//TODO poner algo más

Documentación
----------------

Enlace al wiki y quizás alguna sugerencia particular en alguna sección.

//TODO poner bonito

http://en.wikipedia.org/wiki/Spatial_database

Autores
----------

- |delawen|
