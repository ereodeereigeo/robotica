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

