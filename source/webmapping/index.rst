***********
Web Mapping
***********

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

Es una biblioteca basada en Javascript para el desarrollo de aplicaciones web interactivas integrando la tecnología de OpenLayers y ExtJS. Ofrece la interfaz de usuario propia de ExtJS, con todas las herramientas adaptadas al visor de mapas OpenLayers.

GeoMoose_:

GeoMOOSE es un framework de navegación de mapas para la visualización distribuida de datos cartográficos. Es particularmente útil para gestionar datos geoespaciales y no geoespaciales en oficinas regionales, urbanas y municipales (GeoMOOSE se originó en éstas últimas). Extiende la funcionalidad de MapServer y OpenLayers para proporcionar servicios de serie, como la identificación ‘drill-down’ para ver y organizar muchas capas, operaciones de selección y búsquedas en los juegos de datos.

GeoMOOSE es rápido, con buen rendimiento con cientos de capas y/o servicios al mismo tiempo. Los datos provenientes de diferentes orígenes se pueden mantener usando diferentes herramientas y con diferentes planificaciones ya que cada capa del mapa tiene su propio juego de ficheros de configuración para la publicación, simbología, plantillas así como datos de origen.

La interfaz de usuario es fácilmente configurable, y gracias a su arquitectura modular se pueden agregar servicios adicionales.

Leaflet_:

Leaflet está diseñado con la mente puesta en la simplicidad, el rendimiento y la facilidad de uso. Funciona de manera eficiente en las principales plataformas de escritorio y móviles, aprovechando las ventajas del HTML5 y CSS3 en los navegadores modernos, sin dejar de ser accesibles a los más antiguos. Se puede ampliar su funcionalidad con una gran cantidad de plugins, tiene una API bonita, fácil de usar y bien documentada, así como un código fuente simple y legible, que es una fácilidad para los desarrolladores que quieran contribuir.

Mapstore_:

MapStore ha sido desarrollado para crear, guardar, buscar y compartir de una manera sencilla e intuitiva mashups creados con contenido de fuentes del servidor como Google Maps, OpenStreetMap, MapQuest o servidores específicos proporcionados por la organización o cualquier otra persona. MapStore consta de dos componentes principales como MapManager y GeoStore, respectivamente front-end y back-end.

MapManager, utilizando una sola interfaz, permite al usuario crear, borrar y buscar mapas, generar un vínculo de inserción para poner un mapa en un sitio web, compartir tus propios mapas con otros usuarios. Además lleva a cabo la interacción con GeoStore. MapManager soporta la autenticación y la definición de políticas de acceso para proteger los mapas gestionados por GeoStore.

GeoStore es una aplicación JEE de código abierto cuyo objetivo es el almacenamiento, la búsqueda y la recuperación de datos sobre la marcha. GeoStore implementa una infraestructura flexible y modular desarrollado por encima de la tecnología de Java Enterprise con el fin de crear, gestionar, navegar y buscar las definiciones del mapa. GeoStore integra la autenticación y gestión de autorizaciones según el paradigma de Role Based Access Control (RBAC). Esto protege a los mapas de accesos no autorizados. El mecanismo de almacenamiento estándar de GeoStore consta de un DBMS: Oracle y PostgreSQL son compatibles.

Cartaro_:

Cartaro es la plataforma de cartografía web que proporciona los mejores componentes geoespaciales de código abierto en un sistema de gestión de contenidos. Con Cartaro usted es capaz de instalar y ejecutar su propio sitio web geográfico y compatible con los estándares de la OGC, con no más de unos pocos clics. Los componentes geoespaciales utilizados en Cartaro son PostGIS, GeoServer, GeoWebCache y OpenLayers. Todos los que se gestionan desde el potente CMS Drupal. 

Cartaro es para las organizaciones e individuos que necesitan ejecutar una infraestructura de datos espaciales ligera (SDI), sin necesidad de extensas configuraciones y mucha programación individual.

Cartaro sirve también para montar un sitio web con los beneficios de cualquier CMS pero con la ventaja de poder tratar la información espacial.

Puntos calientes
-------------------

Últimamente todo lo relacionado con Leaflet se convierte en tendencia, ya que están apareciendo distintas tecnologías que hacen uso de esta librería en sus desarrollos, como por ejemplo Mapbox_ o CartoDB_, cuyo aspecto visual tan aparente y resultón hacen que su uso prolifere.

Otro de los puntos en los que se está empleando mayor esfuerzo tecnológico es en los renderizadores 3D basados en WebGL tales como `WebGL Earth`_ o `F4 Map`_, que le dan otra dimensión a la forma de representar los datos espaciales en la web.

El futuro de los mapas podría pasar por mejorar las versiones móviles que hagan que su interacción con el entorno los enriquezca, de forma que pasen de ser consultores o indicadores de direcciones a compañeros imprescindibles en la vida cotidiana, ya que pueden convertirse en planificadores de jornadas, de escapadas de fin de semana e incluso de guías turísticos.


Curva de aprendizaje y conocimientos previos
-------------------------------------------------

Para poder trabajar con la mayoría de las librerías que aquí se presentan son imprescindibles conocimientos en Javascript, ya que la mayoría de éstas están desarrolladas bajo este lenguaje de programación. Aunque hay algunos como Cartaro que está basado en Drupal, para lo que hay que tener conocimientos básicos en PHP.

Es bueno tener conocimientos de servicios web, así como de XML, ya que muchas de las respuestas de los principales protocolos de transferencia de información geográfica usan éste lenguaje de respuesta. También hay que tener conocimientos de los estándares OGC que consumiran la parte cliente.

Hay librerías como OpenLayers o Leaflet donde esta curva de aprendizaje es muy poco pronunciada ya que su facilidad de comprensión y de uso, así como la documentación que poseen, hacen que la experiencia del desarrollador no sea determinante a la hora de elegirlas como posible base para el desarrollo de cliente web geográficos. De hecho otras librerías que aquí se mencionan usan OpenLayers como base cartográfica con la que interactuar y a la que integrarse.

Documentación
---------------

Toda la documentación necesaria para comenzar a usar cualquiera de las tecnologías que aquí se encuentran, la puedes encontrar en las guías de inicio rápido que se adjuntan:

Mapbender_: 

http://live.osgeo.org/es/quickstart/mapbender_quickstart.html

OpenLayers_: 

http://live.osgeo.org/es/quickstart/openlayers_quickstart.html

`GeoExt GXP`_: 

http://geoext.org/tutorials/quickstart.html

GeoMoose_: 

http://live.osgeo.org/es/quickstart/geomoose_quickstart.html

Leaflet_: 

http://leafletjs.com/examples/quick-start.html

Mapstore_: 

https://github.com/geosolutions-it/mapstore/wiki/Quick-Start-Guide

Cartaro_: 

http://live.osgeo.org/es/quickstart/cartaro_quickstart.html

Referencias
---------------

- Panorama SIG Libre, M. Montesinos y J. Sanz `Artículo v2`_, `Diapos v4`_, `Wiki Prodevelop`_

.. _Webmapping: http://wiki.osgeo.org/wiki/Panorama_SIG_Libre_2014/WebMapping
.. _Vladimir Agafonkin: http://agafonkin.com/en/
.. _Mapbox: https://www.mapbox.com
.. _CartoDB: http://cartodb.com/
.. _WebGL Earth: http://www.webglearth.com/
.. _F4 Map: http://demo.f4map.com/
.. _Artículo v2: http://dugi-doc.udg.edu/bitstream/handle/10256/1109/Montesinos_Art.pdf?sequence=18
.. _Diapos v4: http://www.slideshare.net/migmontesinos/panorama-del-ecosistema-de-software-libre-gis-2009
.. _Wiki Prodevelop: https://confluence.prodevelop.es/display/pan/Panorama+FOSS4G

.. Enlaces a webs de proyectos
.. _Mapbender: http://www.mapbender.org/Mapbender_Wiki
.. _OpenLayers: http://openlayers.org/
.. _GeoExt GXP: http://geoext.org/
.. _GeoMoose: http://www.geomoose.org/
.. _Leaflet: http://leafletjs.com/
.. _Mapstore: http://mapstore.geo-solutions.it/mapstore/
.. _Cartaro: http://cartaro.org/