********************
Dispositivos móviles
********************

Incluiremos en la categoría de dispositivos móviles los paquetes de software que se pueden utilizar desde *smartphones* y tabletas.  

Autores
------------

- |shiguera|

Puntos calientes
----------------
Actualmente hay dos sistemas operativos para móviles que acaparan la mayoría de los dispositivos utilizados. Se trata del sistema iOS de Apple y el sistema Android de Google. El más '*abierto*' es el sistema operativo Android, si bien ninguno de los dos es realmente abierto.

Es importante destacar que, cuando el dispositivo móvil utiliza un navegador web para visualizar información en la red, la distinción entre dispositivos móviles y ordenadores de escritorio se hace más difusa, pues las mismas herramientas y librerías nos sirven para visualizar información en un dispositivo móvil u otro tipo de elemento de computación. Es el caso de las librerías OpenLayers o LeafLet, que nos permiten, con pequeñas diferencias, acceder a la visualización de información cartográfica desde cualquier navegador, sea este basado en móviles o en ordenadores de escritorio.

Otro frente actual es el de los sistemas operativos que tratan de ser funcionales tanto en dispositivos móviles como en ordenadores de escritorio. En esta categoría se incuyen el sistema operativo Ubuntu móvil o el Windows 8 que permiten ser ejecutados en todo tipo de ordenadores. Es previsible que el aumento de potencia de los dispositivos móviles unido a la conveniencia de compatibilidad entre dispositivos, permita en un futuro cercano que la distinción entre sistemas operativos para dispositivos móviles y para ordenadores de escritorio se haga cada vez más difusa.

Software
--------
El sistema operativo Android permite utilizar una variante del lenguaje Java para programar los dispositivos móviles. En este sentido, muchas de las librerías Java disponibles para ordenadores de escritorio se pueden utilizar bajo condiciones de operación Android. Sería el caso, por ejemplo, de la librería *Java Topology Suite (JTS)*, que ha sido tratada en la sección correspondiente a librerías.

Existen por otra parte librerías específicas desarrolladas para Android, como es el caso de *Mapsforge*, pensada para visualizar información cartográfica en dispositivos Android. 

La utilización de Java permite también que librerías inicialmente pensadas para ser utilizadas en dispositivos móviles puedan ser reutilizadas en ordenadores de escritorio bajo entorno Java. En general la diferencia está en la parte gráfica de Java: En el caso de ordenadores de escritorio es usual utilizar el entorno Swing que no es compatible con Android. 

.. figure:: img/movilidad.png
   :align: center
   :alt: Información general sobre las tecnologías

   Información general sobre tecnologías

OpenLayers_ y LeafLet_: Han sido tratados en la sección de WebMapping 

OSMDroid_: El objetivo de OSMDroid es proporcionar una librería Java-Android para visualizar mapas en dispositivos Android. Ofrece una clase MapView para sustituir a la que viene de serie en Android que permite la visualización de tiles de OpenStreetMap. Se pueden visualizar tiles en modo on-line y en modo off-line. También proporciona clases para visualizar e interactuar con overlays, marcadores y otros.

MapsForge_: Se trata de una librería que permite visualizar mapas de OpenStreetMap en dispositivos Android. La visualización se realiza en modo off-line y con mapas en formato vectorial. Es necesario disponer de los mapas en un formato propio de MapsForge. Dichos mapas se pueden crear a partir de los ficheros *osm* de OpenStreetMap mediante la herramienta Osmosis_.

OsmAnd_: Es una herramienta de navegación y routing para trabajar desde dispositivos Android con cartografía procedente de OpenStreetMap.

GeoPaparazzi_: Permite tomar fotografías y notas georeferenciadas desde dispositivos Android, para poder ser visualizadas posteriormente con otras herramientas GIS. También proporciona una herramienta de tracking durante los recorridos.

gvSIGMini_: Es un cliente visualizador de cartografía para Android. Proporciona clientes WMS y WMS-C. Permite la búsqueda de direcciones y el cálculo de rutas. Trabaja en modo on-line y off-line. Se pueden superponer varias capas. Proporciona funciones de navegación GPS y posicionamiento por GPS o por red telefónica. Se puede compartir la posición a través de las redes sociales (Twitter, Facebook)  o por SMS y eMail. Permite la integración de *Street View*.

Graphhopper_: Es una herramienta de routing que trabaja con datos de OpenStreetMap. Se puede utilizar desde dispositivos Android, a través de su integración con MapsForge. También es posible utilizarlo desde páginas web como un servicio mediante llamadas HTTP desde Java o Javascript. Desde aplicaciones Java de escritorio es posible trabajar con Graphhopper en modo off-line. Se pueden calcular rutas para automóviles, bicicletas o paseos andando. También se pueden crear vehículos personalizados.

OsmSharp_: Es una herramienta para trabajar con cartografía de OpenStreetMap. Permite la visualización de información vectorial y el cálculo de rutas. Se puede utilizar en Android, iOS y WindowsPhone.


Curva de aprendizaje y conocimientos previos
--------------------------------------------
La programación de los dispositivos Android se realiza a través de un lenguaje Java propio de Android. Muchas de las librerías disponibles para Java funcionan también en dispositivos Android. Es necesario conocer los fundamentos básicos de la programación Java y, además, conocer la forma de utilizar Java en Android. No es un lenguaje sencillo y además la variedad de dispositivos y de tamaños de pantallas hace un poco más complicada la programación.

Conocidos los fundamentos de la programación en Android, es posible utilizar las herramientas descritas anteriormente con un pequeño esfuerzo adicional. 


Documentación
-------------

OpenLayers_:

.. _OpenLayers: http://docs.openlayers.org/

LeafLet_:

.. _LeafLet: http://leafletjs.com/index.html

OSMDroid_:

.. _OSMDroid: https://code.google.com/p/osmdroid/

MapsForge_:

.. _MapsForge: https://code.google.com/p/mapsforge/

.. _Osmosis: http://wiki.openstreetmap.org/wiki/Osmosis

OsmAnd_:

.. _OsmAnd: http://osmand.net/

GeoPaparazzi_:

.. _GeoPaparazzi: http://geopaparazzi.github.io/geopaparazzi/

gvSIGMini_:

.. _gvSIGMini: https://confluence.prodevelop.es/display/GVMN/Documentation

Graphhopper_:

.. _Graphhopper: http://graphhopper.com/#overview

OsmSharp_:

.. _OsmSharp: https://github.com/xivk/OsmSharp
