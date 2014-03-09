*********
Librerías
*********

.. todo:: Sección por completar. Discusión del contenido en la :issue:`9`

Autores
-------

- |alediator|
- |rantolin|
- |shiguera|

Introducción
------------

En esta sección se va a cubrir todo el conjunto de paquetes que ofrecen funcionalidades avanzadas para cualquier sistema de información en la forma de librerías. Como se verá, algunos de estos proyectos han cogido protagonismo a lo largo del tiempo ofreciendo no sólo una interfaz de programación (o API en inglés), si no también un conjunto de herramientas propias. Dado el gran abanico que representan, se dividirá esta sección en otras cuatro secciones en las que se agrupan librerías con características y funcionalidades similares. Así, tendremos la siguiente división:

- **Geoprocesamiento**: Aquí se incluyen todas las herramientas y librerías que proporcionan métodos para la manipulación de información geoespacial como  GDAL/OGR, GEOS, JTS/GeoTools, Geoscript o Shapely.
- **Routing**: Estas librerías ofrecen enrutamiento geoespacial y funcionalidad de análisis de redes. Comprendemos aquí las librerías OSRM, pgRouting y OpenTripPlanner 
- **LiDAR**: Aquí se hablará sobre aquellas librerías y conjunto de herramientas capaces de trabajar con datos LiDAR_. Destacan en esta categoría las librerías libLAS, LASlib/LASzip, SPDlib, PDAL y LASpy.
- **Varios**: Por último, consideramos dos librerías aisladas, una para el renderizado como Mapnik y otra para la automatización procesos para la publicación de información como GeoBatch.

.. _LiDAR: http://es.wikipedia.org/wiki/LIDAR

La siguiente tabla muestra las principales características las librerías tratadas en este artículo. Información detallada sobre la estructura de la tabla se encuentra en la :ref:`introducción <info-tabla>`.

.. figure:: imgs/tabla-principal.png
   :align: center
   :alt: Información general sobre librerías

.. important:: Se puede consultar la versión más reciente, así como los enlaces asociados y anotaciones en la sección de `Librerías`_ del wiki de OSGeo.

.. _Librerías: http://wiki.osgeo.org/wiki/Panorama_SIG_Libre_2014/Librer%C3%ADas#Main_information

Puntos calientes
----------------

.. note:: Dentro de la sección, hacia donde se está moviendo la comunidad.
.. todo:: Queda hablar del los otros tres grupos de librerías

Últimamente, la tecnología LiDAR está en auje y cada vez aparecen más librerías que ofrecen la posibilidad de trabajar con datos LiDAR en el formato LAS_. Algunas también incorporan conjuntos herramientas para el procesado y análisis de datos. Estas herramientas suelen aparecer como comandos de consola para favorecer el desarrollos de *scripts*. Con el objetivo de favorecer la programación de sencillos programas, todas incorporan *bindings* en python. Para permitir un uso más sencillo y cómodo la comunidad está haciendo esfuerzos en la creación interfaces gráficas y en la incorporación de forma nativa de lectura y escritura de datos láser en clientes de escritorio como QGIS o GRASS. 

Software
--------

.. note:: Aquí explicaría en qué campos se suele mover cada elemento sofware. Por ejemplo, Geoserver permite CSW, pero generalmente su uso es más WMS/WFS...
.. todo:: Queda hablar del los otros tres grupos de librerías

Cualquier librería LiDAR presentada en este documento se puede utilizar para la transformación de formatos láser, pero quizás la más adecuada para ello es PDAL, ya que está pensada especialmente para ello. Es más, PDAL trata de mejorar la librería libLAS cuyo desarrollo lleva parado algún tiempo. A su vez, libLAS se generó a partir de una versión anterior de LASlib, aunque estas últimas han seguido evolucionando hacia una potente herramienta de procesado. Cabe notar, para evitar equívocos, que la librería LASlib es completamente libre, mientras que las herramientas (LASTools) tienen el código cerrado pero su utilización está autorizada para usos no comerciales. Además de lectura y escritura de datos y la transformación entre formatos, SPDlib incorpora herramientas para procesar y analizar datos y para generar modelos digitales de elevación. Por último, LASzip es la única librería capaz de leer y escribir datos LiDAR en formato LAZ. Éste es un tipo de formato comprimido pero con las mismas especificaciones que el formato LAS.

Curva de aprendizaje y conocimientos previos
--------------------------------------------

.. note:: Metería otra tabla con los conocimientos previos necesarios para trabajar con y en cada software.
.. todo:: Queda hablar del los otros tres grupos de librerías

Para trabajar con las librerías LiDAR es conveniente tener conocimientos de C++, ya que es el lenguaje común a todas ellas. Aunque existen ya interfaces gráficas para trabajar con estas herramientas, el módo más rápido y versátil es la línea de comando y la utilización de *scripts* o incluso la programación en Python. Por tanto, tener experiencia en estos campos facilitaría su utilización. Escribir en la consola nunca es agradable para cualquier persona que empieza, pero la mayor ventajan que presentan es que todas las herramientas tienen las mismas funcionalidades y es muy intuitivo aprender el lenguaje utilizado en cualquiera de ellas si se adquieren conocmientos previos en alguna otra librería. 

Documentación
-------------

.. note:: Enlace al wiki y quizás alguna sugerencia particular en alguna sección.



