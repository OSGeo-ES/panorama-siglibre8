*************
*Web Mapping*
*************

.. todo:: Sección por completar. Discusión del contenido en la :issue:`3`

Autores
----------

- |alediator|
- |delawen|
- |moiarcsan|

Introducción
--------------

Resulta evidente la importancia del FOSS en el ámbito de la geomática. No hay más que ver la cantidad de proyectos, comunidades, blogs, congresos y demás eventos (como el que ocupa este artículo) que se organizan con cada vez mayor éxito. Esto puede provocar al recién llegado cierta confusión ya que el inherente carácter modular del software libre hace que muchos proyectos dependan de otros y por tanto las interconexiones son múltiples y a todos los niveles.

Con la proliferación de Internet, la aparición de los servidores de mapas se produjo de forma conjunta a la de aplicaciones web que exponían los contenidos servidos por estos productos. Al principio la mayor parte de ellas se materializaban como desarrollos ex profeso y por tanto se resolvían los mismos problemas una y otra vez.
Esta situación derivó como es natural hacia proyectos que intentan proporcionar un conjunto de componentes comunes en general en forma de documentos HTML y aplicaciones escritas en JavaScript que proporcionan al desarrollador una base sobre la que realizar su aplicación específica. También han ido apareciendo proyectos que se basan en mayor o menor medida en código de servidor, básicamente PHP o Java.

La motivación de este texto por tanto es la presentación ante los lectores, desde un punto de vista lo más generalista posible, del estado del arte en este ámbito de la ciencia para dar al lector pistas que le acerquen a aquellos proyectos/productos que le puedan ser de interés para realizar cualquier tipo de proyecto.

En esta sección se tratarán los diferentes proyectos relacionados con la representación de la información geográfica en un cliente web y que tiene como objetivo la visualización y manipulación de la misma.

En la siguiente tabla se presentan las características principales de los productos revisados en el contexto de este trabajo. Se puede consultar más información sobre la estructura de la tabla en la  :ref:`introducción <info-tabla>`.

.. figure:: imgs/tabla-principal.png
   :align: center
   :alt: Información general sobre las tecnologías

   Información general sobre tecnologías

.. figure:: imgs/estandares.png
   :align: center
   :alt: Implementación de estándares OGC

   Implementación de estándares OGC

.. important:: Se puede consultar la versión más reciente, así como los enlaces asociados y anotaciones en la sección de `Webmapping`_ del wiki de OSGeo.

Software
----------

En esta sección se describirá brevemente cada uno de los productos evaluados en esta comparativa. El orden de aparición es cronológico, empezando por los proyectos más veteranos.

Mapbender_:

Cliente Web-GIS construido con Javascript, que ofrece un interfaz de usuario configurable no dependiente de ningún servidor de mapas concreto. Su orientación es la de un geoportal cliente de servicios OGC. Incluye un soporte bastante completo de usuarios, grupos y servicios OGC (OWS). Una característica diferenciadora de Mapbender es la capacidad de edición en cliente sobre navegador, utilizando WFS-T.
MapBender es un proyecto graduado de OSGeo.

OpenLayers_:

OpenLayers es un cliente Web-GIS ligero construido con clases Javascript, sin dependencia de servidores de mapas concretos. Ofrece una interfaz de usuario simplificada que ataca a servicios WMS y WFS de forma transparente para el usuario y desarrollador. Las características a destacar de este producto es la cantidad de herramientas ya implementadas, que hacen que el desarrollar con esta librearía sea mucho más fácil para funcionalidades más complejas.
Actualmente es uno de los proyectos de SIG libre cuya comunidad es de las más activas que existen, a pesar de contar con un grupo de desarrolladores no muy numeroso.
OpenLayers es un proyecto graduado de OSGeo.
Destaca la integración de OpenLayers con otros proyectos como GeoExt o Mapstore.

`GeoExt GXP`_:

bla

GeoMoose_:

bla

Leaflet_:

bla

Mapstore_:

bla

Cartaro_:

bla

Puntos calientes
-------------------

.. note:: Dentro de la sección, hacia donde se está moviendo la comunidad.


Curva de aprendizaje y conocimientos previos
-------------------------------------------------

.. note:: Metería otra tabla con los conocimientos previos necesarios para trabajar con y en cada software.

Documentación
---------------

.. note:: Enlace al wiki y quizás alguna sugerencia particular en alguna sección.

Referencias
---------------

.. Enlaces a webs de  proyectos

.. _Webmapping: http://wiki.osgeo.org/wiki/Panorama_SIG_Libre_2014/WebMapping
.. _Mapbender: http://www.mapbender.org/Mapbender_Wiki
.. _OpenLayers: http://openlayers.org/
.. _GeoExt GXP: http://geoext.org/
.. _GeoMoose: http://www.geomoose.org/
.. _Leaflet: http://leafletjs.com/
.. _Mapstore: http://mapstore.geo-solutions.it/mapstore/
.. _Cartaro: http://cartaro.org/