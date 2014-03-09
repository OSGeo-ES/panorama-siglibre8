**********
Servidores
**********

.. todo:: Sección por completar. Discusión del contenido en la :issue:`2`


Autores
---------------

- |alediator|
- |delawen|
- |jsanz|


Introducción
---------------

En esta sección se va a abordar el amplio conjunto de proyectos correspondientes a la capa intermedia de cualquier sistema de información, también conocida como *middleware*. En esta sección se cubre por tanto cualquier aplicación que se ejecuta en un servidor y que tiene como objetivo proporcionar uno o más servicios que serán consumidos por clientes, independientemente de si estos son otras aplicaciones de servidor, clientes *web*, clientes de escritorio o dispositivos móviles.

¿Qué tipos de servicios actualmente se ofrecen relacionados con la |IG|? Una agrupación funcional podría agruparlos en las siguientes categorías:

- **Servidores de mapas**: Encargados de renderizar datos tanto vectoriales como *raster* en diferentes estilos y proyecciones cartográficas, en general cmupliondo el estándar `WMS de OGC`_
- **Servidores de teselas**: Una variante del anterior es aquellos servidores que ofrecen la cartografía renderizada únicamente en juegos de teselas con un número limitado de resoluciones, casi siempre además empleando sistemas de almacenamiento intermedio (*caches*). En este caso hay dos estándares en el sector, el estándar `TMS`_ y el `WMTS de OGC`_
- **Servidores de datos brutos**: Al contrario que las categorías anteriores, estos servidores ofrecen la cartografía vectorial o *raster* en formatos que deben luego ser procesados por los clientes para la tarea para la que estén desarrollados, tanto si es para su análisis como su visualización. Los estándares de comunicación son `WFS`_ y `WCS`_ respectivamente para datos vectoriales y *raster*. En esta categoría se podrían incluir  también a los servidores relacionados con la publicación de datos de sensores, en todo el abanico de estándares OGC englobados en lo que se conoce como `Sensor Web Enablement`_
- **Servidores de metadatos**: Estos servidores implementan estándares de descubrimiento de datos como `CSW`_. Mediante estos servidores usuarios y otros componentes pueden encontrar juegosde datos y otros servicios mediante protocolos estandarizados. Estos servidores son el corazón de las Infraestructuras de Datos Espaciales.
- **Servidores de geoprocesos**: Estos servidores exponen operaciones de análisis, que pueden partir de datos directamente disponibles en el servidor o bien acceder a otros servidores de datos brutos para encadenar servicios que realicen flujos de geoprocesamiento de todo tipo. El estándar de OGC para geoprocesamiento es el `WPS`_.

.. _WMS de OGC: http://www.opengeospatial.org/standards/wms
.. _TMS: https://en.wikipedia.org/wiki/Tile_Map_Service
.. _WMTS de OGC: http://www.opengeospatial.org/standards/wmts
.. _WFS: http://www.opengeospatial.org/standards/wfs
.. _WCS: http://www.opengeospatial.org/standards/wcs
.. _CSW: http://www.opengeospatial.org/standards/cat
.. _WPS: http://www.opengeospatial.org/standards/cat
.. _Sensor Web Enablement: http://www.opengeospatial.org/ogc/markets-technologies/swe

Es habitual que un producto de |sl| cubra más de una funcionalidad de las definidas en la categorización anterior, especialmente con los proyectos más veteranos. La interoperabilidad es otra de las características del |sl| geoespacial y es por ello que la mayoría de los productos suelen intentar implementar aquellos estándares que afectan a su área de interés.

En la siguiente tabla se presentan las características principales de los productos revisados en el contexto de este trabajo. Se puede consultar más información sobre la estructura de la tabla en la  :ref:`introducción <info-tabla>`.

.. figure:: imgs/tabla-principal.png
   :align: center
   :alt: Información general sobre servidores

   Información general sobre servidores

.. figure:: imgs/estandares.png
   :align: center
   :alt: Implementación de estándares OGC

   Implementación de estándares OGC


.. important:: Se puede consultar la versión más reciente, así como los enlaces asociados y anotaciones en la sección de `Servidores`_ del wiki de OSGeo.

.. _Servidores: http://wiki.osgeo.org/wiki/Panorama_SIG_Libre_2014/Servidores


Puntos calientes
--------------------

Este área del |sl| geoespacial está en continua evolución, pese a que la complejidad inherente a desarrollar este tipo de productos es elevada y hace algún tiempo que no aparece ningún producto relevante. Así y todo los proyectos existentes en general gozan de buena salud y no dejan de actualizarse e innovar.

En el área de los servidores de mapas la mejora del rendimiento y en especial de las capacidades de simbolización han facilitado la aplicación de estos productos en proyectos cada vez más complejos, como en el caso del uso de GeoServer_ en el Instituto Geográfico Francés [GeoServerIGN]_. La innovación de aplicar a cartografía un lenguaje de definición de simbologías análogo a las hojas de estilo de las páginas *web* va a facilitar a los especialistas diseñar y mantener los estilos de sus mapas de una forma mucho más sencilla y a la vez expresiva.

.. _GeoServer: http://geoserver.org

En cuanto a los servidores de geoprocesamiento, la capacidad para definir procesos de análisis geográfico utilizando lenguajes de programación de alto nivel como Python o JavaScript entre otros va a facilitar la inevitable transición de este tipo de proyectos desde los clientes de escritorio a los servidores. Así, proyectos como `Zoo Project`_ o el uso de `GeoScript`_ en `GeoServer`_ ponen a disposición de los analistas un entorno de trabajo que soporta varios lenguajes con un rendimiento elevado.

.. _GeoScript: http://geoscript.org/
.. _Zoo Project: http://zoo-project.org/

Los servidores de teselas siguen siendo de momento un *mal necesario* para ofrecer un rendimiento adecuado en proyectos con cartografía que no sufre actualizaciones frecuentes o necesitan estilos dinámicos. Esta situación en cualquier caso se percibe como transitoria ya que están empezando a aparecer productos y servicios que optimizan la presentación de cartografía sirviéndola en un formato vectorial junto con los estilos, siendo responsabilidad del cliente la renderización de la cartografía. Esta variante permite ofrecer cartografía mucho más dinámica tanto en su componente temporal como en la de la simbolización.

Finalmente en el área de los servicios de descubrimiento el desarrollo de GeoNetwork_, el principal servidor de metadatos libre, sigue activo y van apareciendo nuevas alternativas y variantes como el soporte del protocolo CSW por parte de GeoServer, así como la actividad del proyecto PyCSW_.

.. _GeoNetwork: http://geonetwork-opensource.org/
.. _PyCSW: http://pycsw.org/

Software
----------

.. note:: Aquí explicaría en qué campos se suele mover cada elemento sofware. Por ejemplo, Geoserver permite CSW, pero generalmente su uso es más WMS/WFS...

.. todo:: Breve descripción y principal uso de cada |sl| ¿no tiene más sentido esto antes del tema de los puntos calientes?


Curva de aprendizaje y conocimientos previos
------------------------------------------------

.. note:: Metería otra tabla con los conocimientos previos necesarios para trabajar con y en cada software.


Documentación
---------------

.. note:: Enlace al wiki y quizás alguna sugerencia particular en alguna sección.


Referencias
---------------


.. [GeoServerIGN] `Using GeoServer at IGN (the French National Mapping Agency) to create new digital maps <http://blog.geoserver.org/2014/01/07/using-geoserver-at-ign-the-french-national-mapping-agency-to-create-new-digital-maps/>`_
