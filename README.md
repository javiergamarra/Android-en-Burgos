# Android-en-Burgos
Material para el Curso de Android de Betabeers Burgos/AgileCyL

* [Diapositivas del curso](http://kcy.me/23e0b)

## Requisitos Curso De Android en Burgos para Betabeers/CEEI

### Requisitos

  * Ordenador PC con alguno de los siguientes sistemas operativos: Windows 2003 o posterior, MAC OS 10.8.5 o la mayoría de distribuciones Linux.
  * Experiencia en programación con Java (no es indispensable, se puede hacer programación por parejas).
  * Es preferible pero no indispensable disponer de un terminal Android con su cable micro USB de conexión al PC.

### Guión de instalación del entorno

  Utilizaremos el software siguiente:
  * Java SE 7 (Java SE 6 en Mac recomendada)
  * Android Studio
  * Genymotion (opcional)
  
#### Windows

El proceso de instalación (para Windows) se describe brevemente a continuación. El guión de instalación y arranque está descrito en más detalle en la página oficial.
  
* Descargad el bundle de Android Studio + SDK tools. Son 800MB (casi 3GB descomprimidos). El instalador detectará si no encuenta ninguna JDK instalada (o se trata de una JDK8, no compatible). Podéis descargar la JDK 7 desde este enlace.
* Es necesario instalar tanto Android Studio como Android SDK. Android Virtual Device y Intel HAXM es recomemdado pero no obligatorio.
* Tras la instalación, al arrancar Android Studio mostrará el diálogo del SDK y descargará la última versión disponible (tardará un rato).
* Para probar que todo funciona, cread una nueva aplicación Android (Start a new Android Studio project), API 15, Blank Activity y lanzadla sobre vuestro móvil (o Genymotion, leed más abajo), con menú, Run, Run 'app' (cuando termine el proceso de indexing).

Os recomiendo instalar Genymotion (sólo tenéis que registraros y bajar la versión CON VirtualBox). Una vez instalado (tendréis que reiniciar si no teníais virtualbox), os recomiendo bajaros la imagen de un Nexus 5 con Lollipop (5.0). No hace falta instalar el plugin para Android Studio.
  
#### MAC

* Instalad el dmg recomendado. La instalación fallará si no encuentra una JDK 6.
* Tras la instalación, al arrancar Android Studio mostrará el diálogo del SDK y descargará la última versión disponible (tardará un rato).
* Para probar que todo funciona, cread una nueva aplicación Android (Start a new Android Studio project), API 15, Blank Activity y lanzadla sobre vuestro móvil (o Genymotion, leed más abajo), con menú, Run, Run 'app' (cuando termine el proceso de indexing).
  
Os recomiendo instalar Genymotion, pero antes tenéis que instalar VirtualBox. Una vez instalado, os recomiendo bajaros la imagen de un Nexus 5 con Lollipop (5.0). No hace falta instalar el plugin para Android Studio.

## Problemas habituales

* INSTALL_FAILED_OLDER_SDK:
 Compilando para una versión concreta (imagino que 21-22) y tu móvil tiene una versión inferior.
 
 Puedes cambiarlo en el fichero .gradle (despegando el icono de gradle scripts), dónde pone compileSdkVersion. Bájalo a 4.0 (14) y probablemente te pida que bajes el SDK de esa versión. 
