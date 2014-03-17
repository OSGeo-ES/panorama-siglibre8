.. _intro:

************
Introducción
************

La metodología de trabajo que se emplea para colaborar con este proyecto se centra principalmente en el uso de GitHub_. Para organizar todo el trabajo relacionado con la producción del documento, hemos compuesto un equipo de desarrollo con permisos sobre el propio repositorio, que nos permitirá realizar las modificaciones del documento. Para el correcto funcionamiento del grupo, tenemos habilitada la opción de crear "issues", de forma que la coordinación a la hora de tomar las decisiones que afecten a la producción del artículo sea más eficiente. Además de una reunión semanal mediante irc_ para evaluar el estado de cosecución de los objetivos marcados, cuyas actas se encuentran alojadas en la `wiki de OSGeo`_, que también usamos para la repartición de las distintas secciones, así como para una primera aproximación del contenido de cada una de ellas, además de la generación de las tablas del artículo.

Disponemos de un repositorio en el que se alojan todos los archivos fuentes del artículo, así como todos los recursos relacionados con la presentación.

Para ello tenemos habilitadas en el repositorio dos ramas:

* gh-pages: Rama para el desarrollo de la presentación
* paper: Rama para el desarrollo del artículo

La rama `gh-pages`_, que empleamos para el desarrollo de la presentación, se ha fabricado mediante RevealJS_, un framework javascript para el desarrollo de presentaciónes dinámicas basadas en HTML5 Y CSS3, publicando el contenido de la misma mediante una `GitHub Pages`_.

La rama paper_, que empleamos para el desarrollo del artículo, se ha fabricado mediante Sphinx_, un generador de documentción escrito en Python, que hace que se genere la estructura por defecto de un proyecto base para la generación de un artículo, tal y como el que aquí se presenta.

Empleamos además una herramienta, `Read the Docs`_, que nos facilita el publicar esta documentación en la web, haciéndola fácil de encontrar y ofreciendo opción de búsqueda.
Esta herramienta nos permite subir la documentación generada con Sphinx_ mediante la dirección al repositorio de Git. La documentación será compilada cada vez que se realice un commit, de forma que tendremos siempre la última versión de nuestra documentación disponible en la web.

Para contribuir y hacer crecer esta documentación únicamente tendremos que realizar nuestro fork del repositorio y dependiendo de lo que queramos modificar, tendremos que seleccionar una u otra rama. Para trabajar con la presentación, simplemente tendremos que modificar el fichero index.html que se encuentra en la rama `gh-pages`_. En cambio para trabajar con el artículo, rendremos que modificar el archivo "index.rst" dentro de la carpeta de la sección con la que queremos colaborar.

En cuanto tengamos los cambios listos para subir, debemos realizar el correspondiente commit y sucesivo pull request. Una vez éste esté aceptado, se procederá a la actualización de la documentación alojada en la web de manera automática.

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