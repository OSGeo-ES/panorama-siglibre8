.. _conclusiones:

************
Conclusiones
************

En este artículo hemos tratado de recoger cuál es el estado actual de las herramientas libres para el procesado de datos geoespaciales. Para ello, hemos agrupado en seis categorías diferentes (**Servidores**, **Webmapping**, **Librerías**, **Clientes**, **Móviles** y **Bases de Datos**) los proyectos que ofrecen soluciones para el almacenamiento, procesado, análisis, publicación, visualiación y, en general, cualquier actividad relacionada con datos geoespaciales. 

Tanto los servidores, como los clientes de escritorio y las bases de datos han alcanzado ya una madurez plena y ofrecen una muy alta calidad de productos capaces de competir y superar conocidos paquetes comerciales. Sin embargo, en el caso de los clientes de escritorio se observa que van perdiendo relevancia en favor de proyectos dedicados al Webmapping. Por su parte, las nuevas tecnologías móviles, con la incorporación de sistemas GPS están, incentivando la aparición de software dedicado a geolocalización. También son numerosos los nuevos proyectos enfocados a la manipulación de datos LiDAR.  

Python se está convirtiendo en el lenguaje más extendido en el mundo SIG libre. De hecho, existe una tendencia en casi todas las categorías a la utilización de Python, bien sea para el propio desarrollo de los proyectos o bien para dotarlos de una herramienta de *scripting*. 

A continuación se incorporan unas conclusiones más detalladas de cada una de las categorías de proyectos tratados en este escrito.

Servidores
==========

Tras revisar el estado de los principales proyectos encargados de ofrecer servicios geoespaciales, se aprecia una elevada madurez de la mayoría de productos: no han aparecido proyectos nuevos relevantes en los últimos dos años y los proyectos más veteranos siguen en pleno desarrollo, sin dejar de ofrecer nuevas funcionalidades y mejoras. Cabe destacar también la relevancia que van adquiriendo proyectos desarrollados en Python, uniéndose como base tecnológica a la de proyectos más veteranos escritos en C/C++ y Java.

Webmapping
==========

Tras revisar el estado de los principales proyectos encargados de la visualización interactiva de mapas en el navegador, se aprecia una elevada aparición de distintos proyectos que ofrecen la integración de componentes variados integrándolos en una aplicación mucho más completa y robusta. Además hay que destacar la aparición de frameworks que hacen que la interacción con el usuario sea más interactiva, aprovechando los beneficios de HTML5 y CSS3.

PD: Opinión personal
Para mí creo que la evolución de las librerías destinadas al webmapping han avanzado gracias a la integración de componentes externos haciéndolas evolucionar a portales muchos más completos y añadiéndole funcionalidades que a primera instancia no se incluían, dándole a las herramientas otra dimensión más.

Librerías
=========

La aparición de librerías en Python y soluciones de scripting sencillas aplicables a diversas plataformas y lenguajes de programación, es lo más destacable en los últimos tiempos. En ese ámbito estarían Shapely o GeoScript. Cada vez más son las librerías que intentan ofrecer soluciones para trabajar con datos LiDAR y, aunque todas ellas ofrecen lectura y escritura de datos, sólo algunas aportan capacidad de procesado y análisis. La librería Geotools es una librería Java consolidada y con un desarrollo muy activo que sigue añadiendo componentes, tanto para procesamiento geoespacial como para visualización. Las librerías para el cálculo de rutas están congiendo más relevancia debido a la oferta de datos públicos. 

Clientes
========
Debido a la larga trayectoria de todos los clientes de escritorio, es destacable su gran madurez en todos sus aspectos. De hecho no ha aparecido ningún nuevo proyecto en los últimos años y todos han seguido un desarrollo constante. Cabe destacar, quizás, el caso de QGIS cuya popularidad ha ido en aumento convirtiéndose en el SIG de Escritorio libre más popular. En gran parte, esto se ha sido debido a la integración de Python tanto para la creación de *script* como para la implementación de nuevos módulos, que le confieren una gran versatilidad.

Móviles
=======

La disponibilidad del GPS en los dispositivos móviles, hace que se prevea un crecimiento del mercado de aplicaciones móviles basadas en la geolocalización. La utilización de aplicaciones Web a través del navegador del dispositivo móvil se convierte en una solución muy eficaz al problema de la multiplataforma. En cuanto a soluciones nativas en Java-Android para aplicaciones de visualización cartográfica y geolocalización, tanto OSMDroid (mapas de tiles) como Mapsforge (mapas vectoriales) tienen un desarrollo activo y evolucionan a buena velocidad. La reciente aparición de Graphhopper con soluciones móviles de routing apoyándose en Mapsforge promete dar un impulso a ambos proyectos.

Bases de Datos
==============

El ecosistema de bases de datos geográficas está bastante maduro, ofreciendo tanto una gran calidad como una variedad de tipos; casi todos ellos muy alineados con la compatibilidad OGC, haciendo que el cambio de una base de datos a otra sea prácticamente transparente. En cuanto a las bases de datos NoSQL, están experimentando una interesante evolución que habrá que seguir de cerca los próximos años.