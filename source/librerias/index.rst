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

Software
--------

.. note:: Aquí explicaría en qué campos se suele mover cada elemento sofware. Por ejemplo, Geoserver permite CSW, pero generalmente su uso es más WMS/WFS...
.. todo:: Queda hablar routing

Cualquier librería LiDAR presentada en este documento se puede utilizar para la transformación de formatos láser, pero quizás la más adecuada para ello es PDAL, ya que está pensada especialmente para ello. Es más, PDAL trata de mejorar la librería libLAS cuyo desarrollo lleva parado algún tiempo. A su vez, libLAS se generó a partir de una versión anterior de LASlib, aunque estas últimas han seguido evolucionando hacia una potente herramienta de procesado. Cabe notar, para evitar equívocos, que la librería LASlib es completamente libre, mientras que las herramientas (LASTools) tienen el código cerrado pero su utilización está autorizada para usos no comerciales. Además de lectura y escritura de datos y la transformación entre formatos, SPDlib incorpora herramientas para procesar y analizar datos y para generar modelos digitales de elevación. Por último, LASzip es la única librería capaz de leer y escribir datos LiDAR en formato LAZ. Éste es un tipo de formato comprimido pero con las mismas especificaciones que el formato LAS.

El procesamiento de datos es, en general, *la recogida y manipulación de elementos de datos para producir información significativa*. Así pues, a través del **geoprocesamiento**, se manipulan los datos espaciales con el objetivo de presentarlos en un contexto específico. En cuanto al procesamiento de datos vectoriales aparecen dos tendencias claras: una serie de librerías orientadas a la generación de scriptlets de forma intuitiva y sencilla (GeoScript/Shapely); y librerías clásicas de geoprocesamiento a nivel servidor (GEOS/JTS/GeoTools). Además, GDAL se suele utilizar para la preparación de imágenes ráster de forma que mejoren el rendimiento al ser servidas.

**GeoBatch** da un paso más allá en el geoprocesamiento, permitiendo la definición de ciertos flujos de procesamiento y permitiendo la ejecución de los mismos en background a través de distintos roles y usuarios (así como la ejecución programada de los mismos).

**Mapnik** es una herramienta para el renderizado de mapas atractivos, con bordes de geometrías limpios y suaves, provisto de un sistema gráfico con anti-aliasing de calidad, posicionamiento inteligente de etiquetas, y simbolización SVG escalable. La mayor fama de mapnik viene por ser utilizado como render de la capa principal de Open Street Map.

Puntos calientes
----------------

.. note:: Dentro de la sección, hacia donde se está moviendo la comunidad.
.. todo:: Queda hablar de routing

Últimamente, la tecnología LiDAR está en auje y cada vez aparecen más librerías que ofrecen la posibilidad de trabajar con datos LiDAR en el formato LAS. Algunas también incorporan conjuntos herramientas para el procesado y análisis de datos. Estas herramientas suelen aparecer como comandos de consola para favorecer el desarrollos de *scripts*. Con el objetivo de favorecer la programación de sencillos programas, todas incorporan *bindings* en python. Para permitir un uso más sencillo y cómodo la comunidad está haciendo esfuerzos en la creación interfaces gráficas y en la incorporación de forma nativa de lectura y escritura de datos láser en clientes de escritorio como QGIS o GRASS. 

Respecto al **geoprocesamiento**, probablemente, los avances más significativos se están realizando en la abstración de las librerías clásicas con el objetivo de facilitar su uso de cara a los desarrolladores. Dentro de este grupo se enmcuentran GeoScript, Shapely o  GeoBatch. 

Mapnik se suele embeber típicamente en aplicaciones python que publican mapas en Internet, aunque las últimas mejoras incorporadas han permitido que Mapnik también se utilice para crear mapas de alta resolución en papel.

Curva de aprendizaje y conocimientos previos
--------------------------------------------

.. note:: Metería otra tabla con los conocimientos previos necesarios para trabajar con y en cada software.
.. todo:: Queda hablar del los otros grupos de librerías

Para trabajar con las librerías LiDAR es conveniente tener conocimientos de C++, ya que es el lenguaje común a todas ellas. Aunque existen ya interfaces gráficas para trabajar con estas herramientas, el módo más rápido y versátil es la línea de comando y la utilización de *scripts* o incluso la programación en Python. Por tanto, tener experiencia en estos campos facilitaría su utilización. Escribir en la consola nunca es agradable para cualquier persona que empieza, pero la mayor ventajan que presentan es que todas las herramientas tienen las mismas funcionalidades y es muy intuitivo aprender el lenguaje utilizado en cualquiera de ellas si se adquieren conocmientos previos en alguna otra librería. 

En cuanto al **geoprocesamiento**, los conocimientos necesarios son distintos según la(s) librería(s) que quieras usar. Para todas necesitarás conocimentos acerca del modelo `SFA`_. A no ser que necesites una funcionalidad específica de una de las librerías, podrás elegir aquella que se adecúe más a tus conocimientos.

.. _SFA: http://www.opengeospatial.org/standards/sfa

Documentación
-------------

.. note:: Enlace al wiki y quizás alguna sugerencia particular en alguna sección.



