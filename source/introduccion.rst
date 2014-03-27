.. _intro:

************
Introducción
************

A la hora de abordar este proyecto lo primero que nos planteamos es cómo lo queríamos hacer, es decir, qué requerimientos tendríamos que cumplir. De ahí salió la lista siguiente:

¿Qué requerimientos tenemos?
============================

* Toda la discusión debía ser en abierto
* Todo el contenido en abierto y versionado
* A ser posible autopublicado
* Tener un seguimiento semanal para tener claras las tareas y quién está haciendo qué.

¿Cómo lo hacemos?
=================

Tras esto la forma en la que empezamos a montar toda esta vorágine, fue mediante la `lista de correo`_ y la `wiki de OSGeo`_.  La lista fue el punto de partida, fue el sitio donde nos comprometimos a colaborar y a realizar esta presentación.

¿Cómo nos organizamos?
======================

A partir de aquí surgió la forma en la que nos debíamos organizar, mediante una reunión semanal a través de irc_, para evaluar el estado de consecución de los objetivos marcados.
Teniendo en cuenta que cada una de estas reuniones tienen su acta en la `wiki de OSGeo`_, además del *log* correspondiente para aquél que no haya podido asistir.

Todas las discusiones relacionadas con el contenido de cada sección las llevamos a cabo mediante la generación de tickets_ (issues) en GitHub, de forma que se creasen hilos de conversación en paralelo sobre los principales temas a discutir y no enviáramos ruido a la lista. Aunque a pesar de tener estos hilos, en la lista se seguían notificando las cosas más importantes.

¿Cómo contribuimos los contenidos?
==================================

Disponemos de un repositorio_ en el que se alojan todos los archivos fuentes del artículo, así como todos los recursos relacionados con la presentación.

.. _repositorio: https://github.com/OSGeo-ES/panorama-siglibre8
Para ello tenemos habilitadas en el repositorio dos ramas:

* ``gh-pages``: Rama para el desarrollo de la presentación
* ``paper``: Rama para el desarrollo del artículo

La rama `gh-pages`_, que empleamos para el desarrollo de la presentación, se ha fabricado mediante RevealJS_, un framework javascript para el desarrollo de presentaciones dinámicas basadas en HTML5 Y CSS3.

La rama paper_, que empleamos para el desarrollo del artículo, se ha fabricado mediante Sphinx_, un generador de documentación escrito en Python, que hace que se genere la estructura por defecto de un proyecto base para la generación de un artículo, tal y como el que aquí se presenta.

Para contribuir y hacer crecer esta documentación únicamente tendremos que realizar nuestro *fork* del repositorio y dependiendo de lo que queramos modificar, tendremos que seleccionar una u otra rama. Para trabajar con la presentación, simplemente tendremos que modificar el fichero :file:`index.html` que se encuentra en la rama `gh-pages`_. En cambio para trabajar con el artículo, tendremos que modificar el archivo :file:`index.rst` dentro de la carpeta de la sección con la que queremos colaborar.

En cuanto tengamos los cambios listos para subir, debemos realizar el correspondiente *commit* y sucesivo *pull request*. Una vez éste esté aceptado, se procederá a la actualización automática de la documentación alojada en la *web*.

¿Cómo publicamos los contenidos?
================================

La publicación del contenido de la presentación se realiza de manera automática mediante el uso de `GitHub Pages`_.

La publicación del contenido del artículo se realiza de manera automática mediante el uso de una herramienta denominada `Read the Docs`_, haciéndola fácil de encontrar y ofreciendo opción de búsqueda.
Esta herramienta nos permite subir la documentación generada con Sphinx_ mediante la dirección al repositorio de Git. La documentación será compilada cada vez que se realice un commit, de forma que tendremos siempre la última versión de nuestra documentación disponible en la web.

.. _info-tabla:

Sobre la tabla de información de productos
==============================================

En todas las secciones de este trabajo se utiliza una tabla de descripción de productos que utiliza un juego de campos común. A continuación se describen qué significan esos campos.

.. figure:: _static/tabla-principal-encabezado.png
   :align: center
   :alt: Encabezados de las tablas de productos

   Encabezados de las tablas de productos

**name**:
  Nombre del producto
**year**:
  Año de aparición del producto como |sl|
**OSGeo**:
  Indica si el producto forma parte de la fundación OSGeo_, especificando si el producto está Graduado o en Incubación.
**Live**:
  Indica si el producto forma parte del *Live DVD* que empaqueta el proyecto `OSGeo Live`_.
**License**:
  Se especifica la licencia con la que se distribuye el producto
**Ohloh**:
  Ofrece un enlace, si existe, a la página del producto en la web de estadísticas de proyecso de |sl| `Ohloh.net`_
**Tech**:
  Indica la tecnología principal con la que se ha desarrollado el producto.



.. _Ohloh.net: http://ohloh.net
.. _GitHub: https://github.com/
.. _wiki de OSGeo: http://wiki.osgeo.org/wiki/Panorama_SIG_Libre_2014
.. _Sphinx: http://sphinx-doc.org/
.. _Read the Docs: https://readthedocs.org/
.. _irc: http://webchat.freenode.net/#
.. _paper: https://github.com/moiarcsan/panorama-siglibre8/tree/paper
.. _gh-pages: https://github.com/moiarcsan/panorama-siglibre8/tree/gh-pages
.. _RevealJS: http://revealjs.com/
.. _GitHub Pages: http://pages.github.com/
.. _lista de correo: http://lists.osgeo.org/mailman/listinfo/spanish
.. _tickets: https://github.com/OSGeo-ES/panorama-siglibre8/issues/27#issuecomment-38474599
