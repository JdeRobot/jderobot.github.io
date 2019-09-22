---
permalink: /activities/robotics_courses/advanced_drones
title: "Courses"

youtubeId1: UqEOn0mZ0Uc
youtubeId2: pZJa6olGOlc
youtubeId3: SGrTKwqr_Uw
youtubeId4: Ze92AmFn19Q
youtubeId5: icyLbQFEJa0
youtubeId6: 6MUzWs3k8-I
youtubeId7: JR5OH_XHw7U
youtubeId8: c0heCUeDm7I


sidebar:
  nav: "docs"

toc: true
toc_label: "TOC Programación avanzada de drones"
toc_icon: "cog"
---

## Programación avanzada de drones

Los robots aéreos (drones) son plataformas capaces de volar por sí mismas. Los hay de tamaño pequeño, mediano (unos 50 cms) y mayores. Hasta hace unos años la construcción de drones era costosa y eran robots principalmente de centros de investigación o para usos militares. En los últimos años han aparecido varias plataformas comerciales a precio asequible, se han popularizado y se ha disparado el abanico de aplicaciones que estos robots abren: juegos, grabación de escenas para cine o anuncios, transporte de mercancías, vigilancia de instalaciones, etc. 

El interés en este tipo de robots es enorme actualmente y se están explorando activamente las posibilidades reales de nuevas aplicaciones. Por ejemplo, empresas punteras como Google ([Project Wing](https://www.youtube.com/watch?v=cRTNvWcx9Oo)) o Amazon ([Prime Air](https://www.youtube.com/watch?v=98BIu9dpwHU)) han enseñado prototipos de drones que llevan mercancía de un lugar a otro. DHL ([ParcelCopter](https://www.youtube.com/watch?v=HrcwGHrc0zQ)) y Wallmart también están trabajando en ello. 

Un tipo de drone muy extendido son los cuadricópteros, que incorporan un sistema de vuelo, con cuatro hélices y motores. Se puede manejar en interiores y son capaces de estabilizarse en un punto, a diferencia de los aviones. Además de los actuadores, estos robots están dotados de sensores como GPS, inclinómetros, cámaras, etc. que les proporcionan información y dispositivos de comunicaciones. La inteligencia y funcionalidad reside en su software, en los programas que ejecuta. Este software recoge la información de los sensores, los transmite o no a tierra, se comunica con la estación base para recibir órdenes o toma autónomas decisiones de vuelo. 

Tras el éxito de la primera edición en febrero del 2015 y la segunda en junio 2015 realizamos ahora una <font color="red">tercera edición en noviembre 2015</font>, con nuevas prácticas, un poco más complejas, profundizando en técnicas más sofisticadas de percepción y control. Este curso, de nuevo, <font color="red">se puede seguir distancia</font>. Las clases son presenciales y además serán retransmitidas en directo por streaming a los matriculados, que también podrán hacer preguntas en tiempo real desde su ubicación. Para la parte práctica conveniene que tengas tu propio ordenador, si vienes a clase presencial vente con tu portátil. 


[Página oficial de la URJC del curso](http://www.urjc.es/estudios/titulos-propios/1587-curso-superior-universitario-en-programacion-avanzada-de-drones)

[Instrucciones para inscribirse y matricularse](http://wiki.jderobot.org/Programacion-avanzada-de-drones#CALENDARIO_e_INSCRIPCI.C3.93N) de modo completamente telemático. 


<br/>


## OBJETIVOS

Este curso es la continuación del “Curso Superior Universitario en Programación de drones”, en el cual se daba una introducción básica a la materia. Sin embargo en este segundo curso el objetivo es **profundizar en técnicas más potentes de procesamiento de imágenes y en técnicas de control más completas**. 

Si en el curso básico se presentaba OpenCV y los filtros de color, en el curso avanzado se abordan la homografía y la detección de patrones. En la parte de toma de decisiones, si en el curso básico se explicaba el control PID, en éste se hace énfasis en los autómatas de estado finito y en la navegación exploratoria.

* Desarrollo de aplicaciones para robots aéreos

* Procesamiento avanzado de imágenes: detección de patrones, homografías.

* Técnicas de control basado en autómatas 

* Algoritmos de navegación exploratoria

El curso tiene un marcado carácter práctico, con la programación (en Python) de tres aplicaciones autónomas del cuadricóptero simulado (en Gazebo). Las tres contienen una parte perceptiva, de procesamiento de imágenes de la cámara a bordo, y una parte de control, de toma de decisiones de movimiento en función de lo que ve con la cámara y de su posición 3D. 

**ArDrone real sigue un objeto en el suelo:**

{% include youtubePlayer.html id=page.youtubeId1 %}

<br/>

**ArDrone real sigue un objeto en el espacio tridimensional:**

{% include youtubePlayer.html id=page.youtubeId2 %}

<br/>

<br/>


## PROGRAMA

* Técnicas avanzadas de percepción y control a bordo de drones

**ArDrone simulado sigue una carretera:**

{% include youtubePlayer.html id=page.youtubeId3 %}

<br/>

**ArDrone simulado sigue una pelota roja por el espacio:**

{% include youtubePlayer.html id=page.youtubeId4 %}

<br/>

<br/>


## DESTINATARIOS

El curso está diseñado para aquellas personas motivadas en aprender una nueva tecnología, los robots aéreos, que ya estén terminando sus estudios o trabajando. No es necesario disponer de una titulación concreta para este curso, pero si es recomendable tener conocimientos medios de programacion y/o orientación a objetos. Es condición necesaria haber realizado el “Curso Superior de Programación de Drones” ofrecido por esta misma universidad. 

<br/>


## PROFESORADO

* [José María Cañas Plaza](https://gsyc.urjc.es/jmplaza/) (Profesor de la ETS Ing. Telecomunicación de la URJC). Dirige el grupo de robótica de la URJC, es doctor por la UPM y su investigación desde 1997 se centra en la programación de robots y la visión computacional. Ha desarrollado varios proyectos de robótica industrial y sensores con empresas. Ha realizado estancias de investigación en Carnegie Mellon University y Georgia Tech entre otros. 

* [Alberto Martín Florido](https://wiki.jderobot.org/Amartinflorido-tfg) (Experto en visión de Verisk Analytics). Es graduado en Ingeniería de Computadores en la URJC y actualmente está aumentando su formación en el Master de Visión Artificial de la misma universidad. En su Trabajo Fin de Grado desarrolló la infraestructura para el cuadricóptero ArDrone en la plataforma JdeRobot y una aplicación de control para que el drone siguiera objetos, tanto en el suelo como por el espacio 3D.

* [Eduardo Perdices](https://wiki.jderobot.org/Eperdices_PhD) (Ing. Software en AFC Ingenieros). Es ingeniero informático por la URJC y master en Sistemas Telemáticos e Informáticos. Actualmente está terminando su tesis doctoral sobre técnicas de autolocalización 3D visual robusta, en particular a bordo de humanoides y a bordo de drones, con algoritmos de alta eficiencia computacional.


<br/>


## CALENDARIO e INSCRIPCIÓN

* Plazo de Preinscripción: desde el 26/10 al 3 de noviembre del 2015

* Plazo de Matrícula: desde el 5 al 9 de noviembre del 2015

* Clase <font color="red">13 de noviembre de 17h a 20:40h</font>

* Clase <font color="red">20 de noviembre de 17h a 20:40h</font>

* Clase <font color="red">27 de noviembre de 17h a 20:40h</font>

<font color="red">Aula 207, Aulario-II, Campus de Fuenlabrada de la URJC</font> 

[Página oficial de la URJC del curso](http://www.urjc.es/estudios/titulos_propios/drones/index.html)

El curso cuesta 150 euros. Los trámites previos a empezar el curso son inscribirse y matricularse, ambos se pueden hacer de modo completamente telemático.

**Para inscribirte** en el curso debes realizar la petición a través del portal de GESTIÓN DE SOLICITUDES TELEMÁTICAS de la Universidad Rey Juan Carlos. Las plazas se adjudicarán según orden de inscripción. El plazo de inscripción se ha extendido hasta 2015/05/30. 

* Accede al [portal](http://miportal.urjc.es/GestionSolicitudes/): [http://miportal.urjc.es/GestionSolicitudes/](http://miportal.urjc.es/GestionSolicitudes/)

* Click en "Titulos Propios"

* Click en "Usuarios Nuevos sin cuenta en la URJC" (si no eres alumno de la URJC, si sí lo eres, "Usuarios con cuenta en la URJC")

* En el siguiente formulario rellena tus datos. El tipo de acceso selecciona "Estudiante" y en "Planes Ofertados" selecciona el curso de Programación de drones:


```bash
   4400 	 	Curso Superior Universitario en Programación Avanzada de drones
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

<font color="red">El alumno puede optar entre descargar una máquina virtual con todo el material ya incluido, o por el contrario, realizar la instalación en su máquina nativa. Hemos preparado un paquete debian para Ubuntu Linux 14.04 que simplifica la instalación de todo lo necesario para la realización de las prácticas del curso:</font>

* <font color="red">Entorno de programación JdeRobot 5.3</font>

* <font color="red">Simulador Gazebo 5.0.1, junto con los mundos, modelos y plugins que se utilizarán durante el curso</font>

* <font color="red">Introrob_py, el código fuente de las prácticas donde el alumno tendrá que implementar sus algoritmos</font>

<br/>

### Máquina virtual

Si se opta por utilizar la máquina virtual es necesario descargar el software de virtualización VMWare Player 7 (previo registro). 

* **Software virtualización**: [VMWare Player 7](https://my.vmware.com/web/vmware/free#desktop_end_user_computing/vmware_player/7_0)

* **Máquina virtual**: (en la web de Aula Virtual de la URJC) 

* **Usuario**: curso **Contraseña**: curso 

Con la máquina virtual descargada el siguiente paso es importarla a VMWare Player 7: 

* **Con la máquina virtual descargada el siguiente paso es importarla a VMWare Player 7:**

* Configura la máquina virtual acorde a las características de tu equipo (**Edit virtual machine settings**)

* Arranca la máquina virtual y reinstala las VMWare Tools (**Virtual Machine -> Reinstall VMWare Tools**)

**Nota: Si notas que la máquina virtual no funciona de una manera fluida, intenta iniciar sesión con otro gestor de escritorio. La máquina virtual dispone de gnome 3 y gnome classic.**

<br/>



### Desinstalación de versiones previas de JdeRobot

**Este paso no es necesario si has optado por la opción de la máquina virtual**

**Si tienes una versión anterior de JdeRobot, por favor eliminalá siguiendo los siguientes pasos**

* Desinstalación de JdeRobot

```bash
sudo apt-get remove --purge jderobot
```

* Eliminación del repositorio de JdeRobot. Abre el fichero /etc/apt/sources.list:

```bash
sudo gedit /etc/apt/sources.list
```

* Y elimina las siguientes líneas

```bash
# for ubuntu 14.04 LTS (32/64 bit)

deb http://jderobot.org/apt trusty main
deb-src http://jderobot.org/apt trusty main
```

* Actualiza los índices

```bash
sudo apt-get update
```

<br/>


### Instalación de JdeRobot en Ubuntu 14.04

**Este paso no es necesario si has optado por la opción de la máquina virtual**

**Si tienes una versión antigua de JdeRobot, por favor eliminalá primero**

* Añadimos el repositorio para el simulador gazebo:

```bash
sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-latest.list'
wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -
```

* Añadimos el repositorio de PCL:

```bash
sudo add-apt-repository ppa:v-launchpad-jochen-sprickerhof-de/pcl
```

* Añadimos el repositorio de JdeRobot (simplemente copia y pega todo en tu terminal):

```bash
sudo sh -c 'cat<<EOF>/etc/apt/sources.list.d/jderobot.list
# for ubuntu 14.04 LTS (32/64 bit)

deb http://jderobot.org/apt trusty main
deb-src http://jderobot.org/apt trusty main
EOF'
```

* Obtenemos la clave pública del repositorio:

```bash
wget http://jderobot.org/apt/jderobot-key.asc -O - | sudo apt-key add -
```

* Actualizamos el repositorio:

```bash
$ sudo apt-get update
```

* Instalamos JdeRobot:

```bash
$ sudo apt-get install jderobot-core
```

<br/>


### Configuración de Gazebo 5

**Este paso no es necesario si has optado por la opción de la máquina virtual**

* Lo primero es ejecutar gazebo para que descargue los modelos de su base de datos:

```bash
$ gazebo
```

* Una vez ejecutado (y después de esperar un par de minutos) puedes volver a cerrarlo.

* Copiamos los modelos de JdeRobot al directorio de gazebo

```bash
$ cp -r /usr/local/share/jderobot/gazebo/models/* ~/.gazebo/models/
```

* Creamos del directorio donde almacenaremos los mundos y los ficheros de configuración:

```bash
$ mkdir ~/.gazebo/cfg
```

* Copiamos los mundos para las prácticas el curso:

```bash
$ cp /usr/local/share/jderobot/gazebo/worlds/ArDrone.world ~/.gazebo/cfg
$ cp /usr/local/share/jderobot/gazebo/worlds/ArDrone_labyrinth.world ~/.gazebo/cfg
$ cp /usr/local/share/jderobot/gazebo/worlds/ArDrone_rescue-people.world ~/.gazebo/cfg
$ cp /usr/local/share/jderobot/gazebo/worlds/carColorBeacon.world ~/.gazebo/cfg
```

* Copiamos los ficheros de configuración de los plugins de gazebo:

```bash
$ cp /usr/local/share/jderobot/gazebo/plugins/quadrotor/ardroneplugin.cfg ~/.gazebo/cfg
$ cp /usr/local/share/jderobot/gazebo/plugins/quadrotor/imuplugin.cfg ~/.gazebo/cfg
$ cp /usr/local/share/jderobot/gazebo/plugins/car/carMotors.cfg ~/.gazebo/cfg
```

* Establecemos las variables de entorno necesarias para gazebo

```bash
$ cat /usr/local/share/jderobot/gazebo/gazebo-setup.sh >> ~/.bashrc 
```

* Ejecutamos lo siguiente para que los cambios tengan efecto:

```bash
$ source ~/.bashrc
```

<br/>


### Introrob_py

**Este paso no es necesario si has optado por la opción de la máquina virtual**

Para que introrob_py funcione en tu equipo en primer lugar es necesario tener instalado JdeRobot

Copia el fichero de configuración de introrob_py a tu directorio de trabajo: 

```bash
cp /usr/local/share/jderobot/conf/introrob_py_simulated.cfg .
```

Antes de ejecutar introrob_py asegúrate de que has ejecutado Gazebo con algún mundo de ArDrone, por ejemplo: 

```bash
cd ~/.gazebo/cfg
gazebo ArDrone.world
```

En una terminal distinta ejecuta introrob_py del siguiente modo: 

```bash
introrob_py --Ice.Config=introrob_py_simulated.cfg
```

<br/>

{% include youtubePlayer.html id=page.youtubeId5 %}

<br/>

<br/>



## PRÁCTICAS

### Práctica 1: Aterrizando encima de un coche

{% include youtubePlayer.html id=page.youtubeId6 %}

<br/>

<br/>


### Práctica 2: Escapando de un laberinto con flechas de ayuda

<img src="/assets/images/activities/roboticsCourses/arrowsLab1.png" width="60%" height="40%">


{% include youtubePlayer.html id=page.youtubeId7 %}

<br/>

<br/>


### Práctica 3: Búsqueda de personas tras una catástrofe

<img src="/assets/images/activities/roboticsCourses/rescue.png" width="60%" height="40%">


{% include youtubePlayer.html id=page.youtubeId8 %}


