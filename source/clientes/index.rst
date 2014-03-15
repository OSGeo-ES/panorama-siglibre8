********
Clientes
********

Autores
----------

- |jsitjar|
- |rantolin|


Introducción
---------------

Entendemos por Clientes al conjunto de aplicaciones SIG de Escritorio, es decir, aplicaciones en las que se implementan herramientas para llevar a cabo las tareas básicas del trabajo con datos geográficos:
creación o edición, manejo y análisis. Con esta filosofía fueron desarrollados los primeros programas SIG, especialmente para el tratamiento y análisis de datos geográficos, y posteriormente, para dotar a estos de mayor versatilidad, incorporando otras funciones adicionales que facilitaran el trabajo con esos mismos datos. 

Los SIG de escritorio siguen manteniendo su posición como aplicaciones fundamentales, y hablar genéricamente de un SIG implica por lo general hacerlo de una aplicación de escritorio antes que de otros tipos de aplicaciones. 
Por otra parte, las herramientas de escritorio son soluciones en general completas que cubren la totalidad de necesidades que se presentan en el desarrollo de proyectos SIG, y por ello constituyen las herramientas primordiales para llevar estos a cabo. 
Ofrecen un gran numero de herramientas para gran diversidad de usuarios en diversidad de campos. 

Veamos con un poco más de detalle las principales funcionalidades de los SIG de Escritorio:

- **Entrada y salida de datos**: Todas las aplicaciones SIG de escritorio deben obligatoriamente implmentar capacidades para leer datos y, opcionalmente, guardarlos. Pese a ser de tal importancia, la implementación de las capacidades de entrada y salida es muy variable en unos u otros SIG. Una razón por la que esto sucede es el gran número de formatos de fichero distintos. Así, cada SIG de escritorio es capaz de abrir unos u otros formatos de archivo, y mientras que algunas tratan a todos ellos por igual, ciertas aplicaciones trabajan en un formato propio con carácter nativo y son capaces de incorporar datos en otros formatos a través de extensiones o funciones de conversión entre estos y el formato particular del programa. Cabe destacar también la capacidad de conexión a bases de datos o servicios remotos que ofrecen algunos softwares (ahora la mayoría).

- **Visualización**: La visualización es una función fundamental dentro de los SIG y del trabajo con cartografía en general. La gran mayoría de las herramientas de escritorio incluyen un gran número de elementos para representar los datos geográficos con los que se trabaja. En ocasiones, interesa únicamente crear una representación de los datos, pero incluso cuando el trabajo con una herramienta SIG está enfocado a la realización de un análisis, la visualización y exploración visual de los datos de partida es un paso previo. En general, la forma de operar con los elementos de visualización es muy similar entre soluciones SIG distintas y, a diferencia de lo que sucede con la implementación de otras funcionalidades, el manejo es prácticamente igual.  

- **Análisis**: Posiblemente, una de las funcionalidades más destacadas y significativas de un SIG de Escritorio. La tendencia actual es considerar las capacidades de análisis como herramientas modulares que se ejecutan sobre una plataforma base, la cual comprende las capacidades de visualización y entrada y salidad de datos. Todas estas capacidades de análisis son independientes entre sí, auqnué pueden coordinarse y emplearse en conjunto para alcanzar un resultado concreto. 

- **Edición**: Funcionalidades que permiten modificar y corregir los datos geográficos con los que se trabaja en un SIG. Las operaciones de edición pueden emplearse para la actualización de cartografía, pero también para la creación de nuevas capas, que pueden crearse a partir de la digitalización de imágenes o a partir de cualquier otra capa de la que se disponga. Puede distinguirse entre diversas formas de edición: Edición de geometrías de una capa vectorial, edición de atribuos en una capa vectorial, edición de valores en una capa raster. Fundamentalmente, estas capacidades permiten la composición de documentos cartográficos de acuerdo con un diseño dado. En la elaboración del diseño, pueden emplearse todos los elementos que habitualmente podemos encontrar en un mapa: el propio mapa en sí, leyenda, título, escala, orientación, etc.

- **Generación de cartografía**: Capacidades de creación de cartografía impresa, para generar documentos que puedan posteriormente imprimirse y emplearse como una mapa cásico. Las razones para la existencia de tales funcionalidades son muchas, pero la principal sigue siendo la necesidad que aún existe de apoyarse en este tipo de documentos cartográficos para poder incorporarlos a proyectos o estudios como parte de anexos cartográficos. 


(Fuente: Olaya, V. 2012. Libro Libre SIG.)

Los clientes de escritorio ofrecen un amplio rango de aplicaciones, desde simples visualizadores a software de creación de mapas y análisis y tecnología punta en sistemas de edición y análisis profesional. 

En la siguiente tabla se presentan las características principales de los productos revisados en el contexto de este trabajo. 

.. figure:: img/clientes1.png
   :align: center
   :alt: Información general sobre las tecnologías

   Información general sobre tecnologías

.. figure:: img/clientes2.png
   :align: center
   :alt: Implementación de estándares OGC

   Implementación de estándares OGC

Breve descripción de la sección con retrospectiva y evolución incluyendo la tabla de la sección.


Software
----------

En esta sección se describirá brevemente cada uno de los productos evaluados en esta comparativa. 


gvSIG_:

GvSIG es un proyecto de desarrollo de Sistemas de Información Geográfica en software libre,1 que incluye principalmente las aplicaciones gvSIG Desktop y gvSIG Mobile. 
La aplicación gvSIG Desktop fue la primera que se desarrolló dentro del proyecto gvSIG, por lo que también se conoce abreviadamente como gvSIG. 
Este proyecto fue desarrollado por el gobierno local de la Comunidad Valenciana (Generalidad Valenciana) de España, con el objetivo inicial de realizar la gestión de datos geográficos de esa colectividad; precisamente la sigla gvSIG abrevia la denominación Generalitat Valenciana Sistema de Información Geográfica.


QGis_:

Es un Sistema de Información Geográfica que nació en mayo de 2002 y se estableció como proyecto en SourceForge en junio del mismo año. Fue además uno de los ocho primeros proyectos de la fundación OSGeo.
Se trata de una aplicación de escritorio que pretende ofrecer a usuarios con necesidades básicas un entorno sencillo y agradable. 


GRASS_:

Pryoecto ya muy veterano, anterior al nacimiento del FOSS ya que surgió como un proyecto del ejercito norteamericano, más concretamente del Construction Engineering Research Laboratory (CERL) que comenzó el proyecto ante la necesidad de gestionar la gran cantidad de recursos naturales a cargo del ejército en los Estados Unidos.
Actualmente, la infraestructura principal se gestiona entre el Instituto de Cultura de Trento y el Geselleschaft für Datenanalyse und Fernerkundung (GDF) de Hannover. 
La principal característica de GRASS es su gran número de funcionalidades, derivadas de todos los años de desarrollo y de la estructura modular del programa, que favorece que los desarrolladores aporten al proyecto contribuciones individuales. Por otro lado, el mayor problema de cara a su difusión y adopción es su complejidad y su empinada curva de aprendizaje. Aun siendo un software muy potente, carece de una interfaz amigable.


UDig_:

OpenJUMP_:

JUMP (Java Unified Mapping Platform) fue uno de los primeros proyectos de cliente GIS de escritorio en el lenguaje Java. Destaca por hacer uso de la biblioteca JTS para poder realizar algunas operaciones de análisis espacial, así como el soporte del formato GML y el protocolo WMS desde sus aparición.
Este proyecto fue liderado por Vivid Solutions1 pero dada la política de aceptación de contribuciones externas por parte de la empresa motivó la aparición de un nuevo proyecto derivado (llamado fork  en el ámbito FOSS) conocido como The JUMP Pilot Project (JPP) que pretende coordinar de forma más democrática las contribuciones de diferentes equipos de desarrollo para evitar duplicidad de esfuerzos.

Esto último es especialmente importante, ya que es destacable la cantidad de proyectos derivados que han surgido a partir de él:
Open JUMP
Open JUMP Viatoris
DeeJUMP
SkyJUMP
PirolJUMP
Kosmo

En España destaca el proyecto Kosmo, desarrollado por la empresa SAGE, que pretende incorporar a la plataforma JUMP otros desarrollos de interés realizados en otros proyectos.


SAGA GIS_:

Esta herramienta se ha desarrollado sobre todo en Gottingen, Alemania. Se trata de un GIS de escritorio para Windows con una clara separación entre su interfaz de programación (API) y su interfaz de usuario. De hecho la primera tiene una licencia LGPL y la segunda es GPL. Esto permite realizar módulos “cerrados” sin incumplir ninguna licencia. 
Este software destaca por su orientación a la realización de análisis de imágenes y modelos digitales del terreno especialmente.



OPTICKS_:

GEODA_:

TILEMILL_:





Puntos calientes
------------------

Durante los últimos años el software SIG de escritorio ha dominado, pero se prevé que en la próxima década los servidores SIG o SIG web sean el producto dominante. 


Dentro de la sección, hacia donde se está moviendo la comunidad.



Curva de aprendizaje y conocimientos previos
------------------------------------------------

Metería otra tabla con los conocimientos previos necesarios para trabajar con y en cada software.

Documentación
----------------

Enlace al wiki y quizás alguna sugerencia particular en alguna sección.



