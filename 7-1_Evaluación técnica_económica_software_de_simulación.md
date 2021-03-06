### 7.1 Evaluación técnica económica de software de simulación

Las simulaciones en robótica permiten al investigador o desarrollador agilìzar
el desarrollo de etapas que de otro modo deberían ser realizadas con prototipos reales.
Estas simulaciones, debido al aumento del poder computacional de los últimos años, han ido
ganando popularidad debido a que disminuyen el costo de desarrollo en robótica, ya sea el costo en tiempo,
ya que es posible comprimir el espacio temporal de pruebas de larga duración, así como el costo
monetario de realizarlas con prototipos reales. Una ventaja derivada de lo anterior es la depuración más
rápida de los algoritmos utilizados, debido a la capacidad de las simulaciones de ser repetibles y controlables
[1] Petry et al. (2011)

Los simuladores permiten la integración de diferentes etapas del proceso de desarrollo de robots. Se
realizará una descripción y comparación de los simuladores principales.

#### Gazebo

Es un simulador multirobot 3D, que ofrece la capacidad de simular eficientemente poblaciones de robots
en ambientes complejos en interiores o exteriores. Posee motores de física robustos, gràficos de alta 
calidad e interfaces gráfigas convenientes para la programación.

Posee una comunidad muy activa en el desarrollo Open Source del producto, y es gratuito.
Actualmente la versión estable es Gazebo5, sin embargo Gazebo6 será lanzado en Julio del 2015
y añadirá soporte para Windows, además del actual soporte para las plataformas GNU/Linux y Mac.

**Características principales:**

* Incluye motores físicos como ODE, Bullet, Simbody y DART
* Utiliza OGRE para los gráficos 3D incluyendo luces, sombras y texturas de alta calidad.
* Puede generar datos de sensores, opcionalmente con ruido, desde *laser range finders*, 
cámaras 2D/3D, sensores tipo Kinect, sensores decontacto, sensores de fuerza y torque, etc.
* Se pueden realizar *plugins*(extensiones) personalizadas para robots, sensores y control del entorno.
* Existen modelos de robots pre-creados como PR2, Pioneer2DX, iRobot Create y TurtleBot, además
permite crear nuevos usando el editor SDF.
* Permite ejecutar simulaciones en servidores remotos y conectarlos a Gazebo mediante el protocolo
TCP/IP usando Google Protobufs.
* Permite realizar simulación en la nube usando CloudSim para ejecutar Gazebo en Amazon, SoftLayer
u OpenStack.
* Posee herramientas de línea de comandos que facilitan el control de las simulaciones.

#### Webots

Es un entorno de desarrollo que se usa para modelar, programar y simular robots móviles.
Permite modelar cada objeto y sus características como forma, textura, masa, fricción, etc.
Posee una gran cantidad de sensores y actuadores para equipar cada robot.
Es bastante usado en universidades y centros de investigación alrededor del mundo (hasta 1200).

**Características Principales:**

* Está disponible para Windows, Mac y Linux
* Posee una versión educativa que es más barata aunque limitada.
* Se puede programar con C/C++, Java, Python, Matlab, URBI y usar librerías externas como OpenCV.
* Se puede realizar una interfaz con ROS (*Robot Operating System*)
* Los modelos 3D se pueden diseñar en Solidworks, AutoCAD, Blender, 3D Studio Max, Sketchup, etc.
* Librerías pre diseñadas de objetos como mesas y sillas.
* Dispositivo de simulación de cámaras integradas con el robot
* Se pueden crear y personalizar los motores utilizados.
* Posee una ventana de simulación 3D interactiva con gráficos realistas
* Y cuenta con librerías de robots populares como Nao y epuck.
* Usa ODE para la simulación de la física del entorno.


#### USARSim

Es un simulador de alta fidelidad basado en el motor gráfico y físico del juego Unreal Tournament.
Es Open Source sin embargo el motor gráfico del juego no lo es por lo que se debe pagar el valor del juego (USD$19.99).
Tiene fines de investigación y es la base para la competencia RoboCUP rescate virtual con robots.

**Características Principales:**

* Soporta principalmente robots bípedos y móviles, sin embargo es posible añadir otros tipos de robots.
* Los robots y objetos se crean en programas CAD 3D y los ambientes se crean usando una utilidad incluida.
* Los robots pueden ser programados usando la utilidad UNREAL Script o controlados sobre una conexión de red usando el protocolo UDP implementado en USARSim.
* Posee procesamiento multihilo
* Es altamente extensible
* El motor gráfico de Unreal Tournament está basado en PhysX que es desarrollado por Nvidia y posee mejores características y algoritmos optimizados en comparación con ODE.

#### Microsoft Robotics Developer Studio

Está orientado para una amplia gama de usuarios, desde amateurs hasta profesionales para el desarrollo de aplicaciones robóticas.

**Caracterítsticas principales:**

* Utiliza PhysX como simulador de alta fidelidad de física
* Posee soporte para Kinect
* Procesamiento paralelo
* No permite crear sensores
* Se programa prncipalmente en C++ o C# Además del lenguaje VLP (Visual Programming Languaje)
* Existe una gran cantidad de robots y sensores
* Solo puede se usado en Windows
* Existen ambientes simulados prediseñados (Casa, fábrica, exteriores, urbana)
* Es de licencia gratuita
* No tiene soporte desde el 2012 y Microsoft canceló la división encargada de desarrollar el software.

