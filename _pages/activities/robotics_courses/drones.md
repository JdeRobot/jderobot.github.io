---
permalink: /activities/robotics_courses/drones
title: "Courses"

youtubeId1: rIkTImMyoXw
youtubeId2: UqEOn0mZ0Uc
youtubeId3: pZJa6olGOlc
youtubeId4: SGrTKwqr_Uw
youtubeId5: Ze92AmFn19Q
youtubeId6: Y5VvQAP6cMI
youtubeId7: ZfGN53v56AI
youtubeId8: NoCWVHyjkqM
youtubeId9: -hcbU0POiWc

sidebar:
  nav: "docs"

toc: true
toc_label: "TOC Programación de drones"
toc_icon: "cog"
---

## Programación de drones

Los robots aéreos (drones) son plataformas capaces de volar por sí mismas. Los hay de tamaño pequeño, mediano (unos 50 cms) y mayores. Hasta hace unos años la construcción de drones era costosa y eran robots principalmente de centros de investigación o para usos militares. En los últimos años han aparecido varias plataformas comerciales a precio asequible, se han popularizado y se ha disparado el abanico de aplicaciones que estos robots abren: juegos, grabación de escenas para cine o anuncios, transporte de mercancías, vigilancia de instalaciones, etc. 

El interés en este tipo de robots es enorme actualmente y se están explorando activamente las posibilidades reales de nuevas aplicaciones. Por ejemplo, empresas punteras como Google ([Project Wing](https://www.youtube.com/watch?v=cRTNvWcx9Oo)) o Amazon ([PrimeAir](https://www.youtube.com/watch?v=98BIu9dpwHU) y [PrimeAir2](https://www.youtube.com/watch?v=MXo_d6tNWuY)) han enseñado prototipos de drones que llevan mercancía de un lugar a otro. 

Un tipo de drone muy exitoso son los cuadricópteros, que incorporan un sistema de vuelo, con cuatro hélices y motores. Se puede manejar en interiores y son capaces de estabilizarse en un punto, a diferencia de los aviones. Además de los actuadores, estos robots están dotados de sensores como GPS, inclinómetros, cámaras, etc. que les proporcionan información y dispositivos de comunicaciones. La inteligencia y funcionalidad reside en su software, en los programas que ejecuta. Este software recoge la información de los sensores, los transmite o no a tierra, se comunica con la estación base para recibir órdenes o toma autónomas decisiones de vuelo. 

Tras el éxito de las tres primeras ediciones (febrero, junio del 2015, febrero 2016) realizaremos una <font color="red">cuarta edición en noviembre 2016</font>, con la plataforma de prácticas renovada y la posibilidad de <font color="red">matriculación telemática y participación a distancia en el curso</font>. Las clases son presenciales y además serán retransmitidas en directo por streaming a los matriculados, que también podrán hacer preguntas en tiempo real desde su ubicación. Para la parte práctica conveniene que tengas tu propio ordenador, si vienes a clase presencial vente con tu portátil. Adicionalmente, los asistentes a este curso estarán preparados para participar en la segunda edición del [campeonato de programación de drones](http://wiki.jderobot.org/Campeonato-programacion-de-robots), que organizamos a finales de enero de 2017. 

{% include youtubePlayer.html id=page.youtubeId1 %}

<br/>


[Página oficial de la URJC del curso](http://www.urjc.es/estudios/titulos-propios/888-curso-superior-universitario-en-programacion-de-drones)

[Instrucciones para inscribirse y matricularse](http://wiki.jderobot.org/Programacion-de-drones/#CALENDARIO_e_INSCRIPCI.C3.93N) de modo completamente telemático. 

<br/>


## OBJETIVOS

El objetivo del curso es **enseñar a programar un cuadricóptero**, crear una aplicación completa que le dota de comportamiento autónomo. Sirve de introducción a esta tecnología novedosa de robots aéreos. La aplicación contiene una parte perceptiva, de procesamiento de imágenes de la cámara a bordo del drone, y una parte de control, de toma de decisiones de movimiento en función de lo que ve con la cámara. 

* Desarrollo de aplicaciones para robots aéreos

* Procesamiento sensorial y de imágenes, empleo de OpenCV para visión 

* Técnicas básicas de control reactivo

El curso tiene un marcado carácter práctico. Utilizaremos lenguaje Python para programar la inteligencia de un cuadricóptero, el simulador Gazebo y JdeRobot como plataforma. Se proporcionan varios componentes software, ya desarrollados, para manejar al cuadricóptero y para insertar el código que gobierna su comportamiento. Los mejores trabajos podrán probar el cuadricóptero real ArDrone de Parrot. 

**ArDrone real sigue un objeto en el suelo:**

{% include youtubePlayer.html id=page.youtubeId2 %}

<br/>

**ArDrone real sigue un objeto en el espacio tridimensional:**

{% include youtubePlayer.html id=page.youtubeId3 %}

<br/>

<br/>


## PROGRAMA

* Presentación del curso (0.5h)

* Introducción a la robótica y robots aéreos (2h)

* Instalación y configuración del entorno de prácticas (Python, simulador Gazebo en Linux) (1h)

* Teleoperación de un cuadricóptero (0.5h)

* Procesamiento de imágenes, filtros de color, segmentación (manejo OpenCV) (3.5h)

* Técnicas de control reactivo (control PID, control borroso) (3.5h)

* Evaluación (1h)

**ArDrone simulado sigue una carretera:**

{% include youtubePlayer.html id=page.youtubeId4 %}

<br/>

**ArDrone simulado sigue una pelota roja por el espacio**

{% include youtubePlayer.html id=page.youtubeId5 %}

<br/>


<br/>


## DESTINATARIOS

El curso está diseñado para aquellas personas motivadas en aprender una nueva tecnología, los robots aéreos, que ya estén terminando sus estudios o trabajando. No es necesario disponer de una titulación concreta para este curso, pero si es recomendable tener conocimientos medios de programacion y/o orientación a objetos. 

<br/>


## PROFESORADO

* [José María Cañas Plaza](https://gsyc.urjc.es/jmplaza/) (Profesor de la ETS Ing. Telecomunicación de la URJC). Dirige el grupo de robótica de la URJC, es doctor por la UPM y su investigación desde 1997 se centra en la programación de robots y la visión computacional. Ha desarrollado varios proyectos de robótica industrial y sensores con empresas. Ha realizado estancias de investigación en Carnegie Mellon University y Georgia Tech entre otros. 

* [Eduardo Perdices](https://wiki.jderobot.org/Eperdices_PhD) (Ing. Software en AFC Ingenieros). Es ingeniero informático por la URJC y master en Sistemas Telemáticos e Informáticos. Actualmente está terminando su tesis doctoral sobre técnicas de autolocalización 3D visual robusta, en particular a bordo de humanoides y a bordo de drones, con algoritmos de alta eficiencia computacional.

* [Alberto Martín Florido](https://wiki.jderobot.org/Amartinflorido-tfg) (Ingeniero en visión artificial, Xactware - Geospatial Solutions). Es graduado en Ingeniería de Computadores en la URJC y actualmente está aumentando su formación en el Master de Visión Artificial de la misma universidad. En su Trabajo Fin de Grado desarrolló la infraestructura para el cuadricóptero ArDrone en la plataforma JdeRobot y una aplicación de control para que el drone siguiera objetos, tanto en el suelo como por el espacio 3D.

<br/>


## CALENDARIO e INSCRIPCIÓN

<font color="red">Cuarta edición</font><br/>

* <font color="red">11 de noviembre 2016 de 17h a 20:40h</font>

* <font color="red">18 de noviembre 2016 de 17h a 20:40h</font>

* <font color="red">25 de noviembre 2016 de 17h a 20:40h</font>

<font color="red">Aula 323, Aulario III, Campus de Fuenlabrada de la URJC</font>
<br/>
<font color="red">INSCRIPCIÓN: del 7 al 23 de octubre de 2016</font><br/>

<font color="red">MATRÍCULA: del 29 de octubre 2016 al 7 de noviembre del 2016</font>

<br/>

Tercera edición 

* 5 de febrero 2016 de 17h a 20:40h

* 12 de febrero 2016 de 17h a 20:40h

* 19 de febrero 2016 de 17h a 20:40h

Segunda edición 

* 12 de junio 2015 de 17h a 20:40h

* 19 de junio 2015 de 17h a 20:40h

* 26 de junio 2015 de 17h a 20:40h

Primera edición 

* 13 de febrero 2015 de 17h a 20:30h

* 20 de febrero 2015 de 17h a 20:30h 

* 27 de febrero 2015 de 17h a 20:30h

[Página oficial de la URJC del curso](http://www.urjc.es/estudios/titulos_propios/drones/index.html)

El curso cuesta 150 euros. Los trámites previos a empezar el curso son inscribirse y matricularse, ambos se pueden hacer de modo completamente telemático. 

**Para inscribirte** en el curso debes realizar la petición a través del portal de GESTIÓN DE SOLICITUDES TELEMÁTICAS de la Universidad Rey Juan Carlos. Las plazas se adjudicarán según orden de inscripción. El plazo de inscripción se ha extendido hasta 2015/05/30. 

* Accede al [portal](https://miportal.urjc.es/GestionSolicitudes/): [http://miportal.urjc.es/GestionSolicitudes/](http://miportal.urjc.es/GestionSolicitudes/)

* Click en "Titulos Propios"

* Click en "Usuarios Nuevos sin cuenta en la URJC" (si no eres alumno de la URJC, si sí lo eres, "Usuarios con cuenta en la URJC")

* En el siguiente formulario rellena tus datos. El tipo de acceso selecciona "Estudiante" y en "Planes Ofertados" selecciona el curso de Programación de drones:

```bash
   4357 	 	Curso Superior Universitario en Programación de drones
```

* Acepta la solicitud.

* A continuación recibirás un correo electrónico con tus datos de acceso (usuario y contraseña) (para terminar la inscripción deberás subir tu Curriculum en formato PDF)

* Accede al portal: [http://miportal.urjc.es/GestionSolicitudes/](http://miportal.urjc.es/GestionSolicitudes/)

* Click en "Titulos Propios"

* Click en "Usuarios con cuenta en la URJC"

* Haz login con tus nuevas credenciales

* En el último apartado "PASO 1" haz click en "Añadir documentos" para subir tu Currículum Vitae. Con esto quedará tu solicitud de inscripción entregada.

**Para matricularte:**

* <font color="red">entra en el enlace</font> [Solicitud de matrícula títulos propios de la URJC](https://www.urjc.es/estudiar-en-la-urjc/admision/276-titulos-propios-admision#matr%C3%ADcula) <font color="red">con tu usuario y contraseña, los que te ha dado el sistema al inscribirte</font>

* <font color="red">chequea que tienes este curso/asignatura</font>

* <font color="red">valida tu matrícula</font>

* <font color="red">imprime la carta de pago y abona los 150 euros (en Bankia o Banco Santander)</font>

* <font color="red">envía el justificante de pago escaneado a titulopropio.alumnos@urjc.es con copia a josemaria.plaza AT urjc.es.</font>

Si tienes problemas con la matrícula contacta con la URJC vía correo electrónico: titulopropio.info@urjc.es o a titulopropio.alumnos@urjc.es

Para más información o dudas, contacta con JoseMaría por correo electrónico (josemaria.plaza AT urjc.es) 

<br/>


## MATERIAL DOCENTE

<font color="red">(noviembre 2016) El alumno puede optar entre descargar una máquina virtual Docker con todo el material ya incluido, o por el contrario, realizar la instalación en su máquina nativa. Hemos preparado un paquete debian para Ubuntu Linux 16.04 que simplifica la instalación de todo lo necesario para la realización de las prácticas del curso:</font>

* Entorno de programación JdeRobot 5.4

* Simulador Gazebo 7, junto con los mundos, modelos y plugins que se utilizarán durante el curso

* El código fuente de las prácticas donde el alumno tendrá que incorporar sus algoritmos


### Instalación del entorno

Instrucciones para la instalación del entorno de desarrollo JdeRobot y el entorno de prácticas TeachingRobotics: 

* **Ubuntu 16.04 y Debian stable:** [aquí](https://wiki.jderobot.org/Robotics-Academy#Installation_and_use)

* **Windows 64 bits (contenedores docker):** [aquí](https://wiki.jderobot.org/Robotics-Academy#Local_installation_on_Windows_machines)

* **Instalación con máquina virtual (vmware 12.5):** [aquí](https://wiki.jderobot.org/store/jmplaza/uploads/teaching/curso-drones/Ubuntu_programacion_drones_2016_gzweb.tar.gz) (contraseña la decimos por AulaVirtual) 


**Prueba de la instalación para Ubuntu 16.04 y Debian stable**

Para comprobar que todo el entorno se ha instalado correctamente vamos a realizar una prueba para teleoperar el Ar.Drone simulado. Para ello sigue los siguientes pasos: 

* En un terminal ejecutaremos el simulador Gazebo con un cuadricóptero simulado:

```bash
gazebo ArDrone.world
```

* En otro terminal ejecuta el componente uav_viewer:

```bash
uav_viewer --Ice.Config=uav_viewer_simulated.cfg
```

*  Con uav_viewer en ejecución puedes teleoperar el ArDrone pulsando las siguientes teclas:

```bash
T - para despegar
L - para aterrizar
C - cambiar cámara
W - para elevar el drone
S - para descender el drone
A - para rotar el drone en sentido contrario a las manecillas del reloj
D - para rotar el drone en sentido de las manecillas del reloj
8 - para mover el drone hacia delante
2 - para mover el drone hacia atrás
6 - para mover el hacia la derecha
4 - para mover el hacia la izquierda
```

<br/>

**Prueba de la instalación para Windows 64 bits**

Próximamente 


**Entorno de desarrollo**

Se recomienda que el alumno utilice algún entorno de desarrollo para Python. Si no estás familiarizado con ninguno quizás puedas probar PyCharm Community Edition. 

**Instalación de PyCharm Community Edition en Ubuntu 16.04:**

```bash
sudo add-apt-repository ppa:mystic-mirage/pycharm
sudo apt update
sudo apt install pycharm-community
```


**Instalación de PyCharm Community Edition en Windows:** [descarga](https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC)


<br/>


## PRÁCTICAS (videos)

### Práctica Filtros de color

* **Vídeo 1:** [descarga](https://wiki.jderobot.org/store/amartinflorido/uploads/curso/pelota_roja.avi)

* **Vídeo 2:** [descarga](https://wiki.jderobot.org/store/amartinflorido/uploads/curso/pelotas_roja_azul.avi)

* **Vídeo drone 1:** [descarga](http://wiki.jderobot.org/store/amartinflorido/uploads/curso/drone1.mp4)

* **Vídeo drone 2:** [descarga](http://wiki.jderobot.org/store/amartinflorido/uploads/curso/drone2.mp4)

<br/>

{% include youtubePlayer.html id=page.youtubeId6 %}

<br/>

<br/>


### Práctica Control en posición con PID

<br/>

{% include youtubePlayer.html id=page.youtubeId7 %}

<br/>

<br/>


### Práctica Atrapa a la tortuga

* **Código fuente:**

<br/>

{% include youtubePlayer.html id=page.youtubeId8 %}

<br/>

<br/>


### Práctica Tu cuadricóptero sigue una carretera desde el aire

<br/>

{% include youtubePlayer.html id=page.youtubeId9 %}

<br/>

