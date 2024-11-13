# Capítulo 6. Electroneumática

**Armar el siguiente circuito Electroneumático.**

![electroneumtico basico](video/eletroneumatica_basico_1.gif)

## Ejercicio 1

Realizar un circuito electroneumático, el cual al presionar un botón salga el vástago, se suelta el botón; el vástago se mantiene fuera, con otro botón se regresa el vástago, se debe usar una válvula biestable con solenoide.

<details markdown="1">
    <img src="video/eletroneumatica_basico_2.gif" alt="circuito">
    <br>
</details>

## Sistema de enclavamiento (interlock)

Realizar el circuito de control eléctrico para cualquiera de estos dos circuitos. Al presionar un botón (S1) se debe salir el vástago, se suelta el botón (S1) y el vástago continua afuera, se presiona otro botón (S2) y el vástago regresa a su posición original. S1 es un botón normalmente abierto, S2 es un botón normalmente cerrado.

![ejercicio enclavamiento](imgs/ejercicio_enclavamiento.png)

<details markdown="1">
    <img src="imgs/electro_enclavamiento.png" alt="circuito">
    <br>
    <img src="video/enclavamiento_simple_efecto.gif" alt="circuito simple efecto">
    <br>
    <img src="video/enclavamiento_doble_efecto.gif" alt="circuito doble efecto">
</details>

### Ejercicio 2

Control de cilindro de simple efecto con válvula de 3/2 monoestable accionada por solenoide con retorno de muelle, el vástago debe salir de forma suave. Controlada por botón.

### Ejercicio 3

Control de cilindro de simple efecto con válvula de 3/2 monoestable accionada por solenoide con retorno de muelle, el vástago debe salir de forma suave. Controlada por botón de enclavamiento con luces indicativas.

### Sensores

#### Final de carrera (Limit switch)

Este sensor seria lo equivalente a una `válvula accionada por rodillo`. Este tipo de sensor nos ayuda a saber la posición del algún elemento, como podría ser el vástago, o cualquier otro elemento mecánico que lo toque o lo presione.
Nos puede ayudar a contar algún objeto, las veces que lo toca o empuja.

<figure markdown="1">
    <img src="imgs/limit_switch_simbolo.png" alt="limit switch símbolo">
<figcaption>Limit Switch Símbolo NA (Normalmente abierto), NA (Normalmente cerrado)</figcaption>
</figure>

<figure markdown="1">
    <img src="imgs/Limit-switches.png" alt="limit switch físico">
<figcaption>Limit Switch Físico</figcaption>
</figure>

##### Circuito

Se muestra como se utiliza en el siguiente circuitos electroneumático

![limit switch](imgs/limit_switch_1.png)
![limit switch](imgs/limit_switch_2.png)

![limit animacion](video/limit_switch.gif)

##### Ejercicio 4 (1A+ 2A+  1A-2A-)

Realizar el circuito electroneumático para el diagrama de movimientos indicado con **electroválvulas monoestables** y cilindros de doble efecto. Pulsadores de un ciclo, paro y repetición de ciclos por impulso momentáneo.
Al pulsar SB1 y estar los dos vástagos dentro, debe salir el vástago de 1A. El vástago de 1A acciona 1B2, que hace salir al vástago de 2A. El vástago de 2A acciona 2B2, que hacen entrar a ambos vástagos a la vez.

![diagrama de mov 4](imgs/diagrama_movi_electro_exer_4.png)

<details markdown="1">
    <img src="imgs/exerc_4_solution.png" alt="circuito">
    <br>
</details>

#### Sensor inductivo (Reed)

![símbolo](imgs/sensor_inductivo_reed.png)

El sensor inductivo nos ayuda a conocer la posición del embolo, que esta dentro del cilindro. Estos están colocados sobre el cuerpo del cilindro.
![reed](imgs/reed.jpg)

![cilindro reed](imgs/cilindro_reed.jpeg)

La salida de la señal del sensor nos ayuda a alimentar la bobina del relay y realizar las acciones necesarias que necesitemos.

La forma de conexión es la siguiente:

![sensor](imgs/conexion_sensor.png)

![sensor1](imgs/sensor_1.png)

![sensor gif](video/sensor_1.gif)

## Compuertas lógicas con contactos

![compuertas](imgs/puertas-logicas-contactos.png)

## Aplicaciones

## Prensa de placas

En una estación se colocan a presión placas de características sobre cuerpos de válvulas.
En un primer lugar, se colocan las placas de características en los rebajes que poseen los cuerpos de las válvulas para tal fin.
Un cilindro aplica presión sobre ellas, para que queden embutidas. La operación de prensado del cuerpo de la válvula se activa mediante un pulsador.
Una vez sujeto el cuerpo de la válvula, se inicia la operación de prensado. Cuando el cilindro de prensado alcanza su posición delantera de final de carrera, ambos cilindros deben retroceder.

![prensa](imgs/prensa_de_placas.png)

## Sistema transportador

Los paquetes que llegan por transportador son elevados por un cilindro neumático A (1.0) y desplazados a otro transportador, mediante un segundo cilindro B (2.0), el regreso del actuador A será en el momento que el actuador B desplace la caja, *el actuador B regresará a su posición de inicio cuando A alcance su posición de reposo*.

![sistema transportador](imgs/Sistema_transportador.png)

## Sistema de taladrado

Unas piezas cúbicas de acero son alimentadas desde un almacén de carga por gravedad a una máquina de mecanizado, fijadas, mecanizadas y expulsadas. Un cilindro de doble efecto dispuesto horizontalmente, con el aire de escape estrangulado (1.0) empuja las piezas fuera del almacén bajo el husillo de la taladradora y las mantiene sujetas contra un tope fijo. El husillo de taladrado (2.0) avanza empujado por un cilindro, haciendo descender la broca. Una vez se ha alcanzado la profundidad deseada, fijada por una válvula de accionamiento por rodillo, empieza la carrera de retroceso sin restricción. Al finalizar la carrera de retroceso, la pieza es expulsada por un cilindro de simple efecto (3.0). Después de un período t = 0,6 segundos, empieza la carrera de retroceso rápida. Cuando el cilindro expulsor haya alcanzado la posición final retraída se acciona una cuarta válvula de rodillo, cuya señal puede utilizarse para permitir el inicio de un nuevo ciclo.

![sistema de taladro](imgs/Sistema_de_taladro.png)

## Cargador para alimentación de ejes

En numerosas máquinas de montaje o mecanizado es necesario alimentar ejes, tubos y similares. Esta operación suele ser automática. En la gráfica se aprecia un cargador de barras apiladas del que salen las piezas una a una. El tamaño del cargador puede adaptarse a la longitud de las piezas. En la salida del cargador hay una palanca basculante (vibratoria) para evitar atascos (ocasionados por la fricción y el peso de las piezas). Este sistema podría ser utilizado, por ejemplo, para alimentar piezas a una máquina lijadora. En el dibujo "b" se muestra una alternativa frente al cargador de piezas apiladas con salida mediante palanca basculante. En este caso se trata de un cargador con salida mediante un segmento que recoge las piezas una a una.

![cargador para alimentar de ejes](imgs/Cargador_para_alimentacion_de_ejes.png)

## Prensa Latas

Diseñar el sistema de control electroneumático de una prensadora de latas, para esto deberá utilizar electroválvulas monoestables, la secuencia deberá ejecutarse de manera manual. Es decir, al presionar el pulsador que comience la secuencia, que realice todos los pasos y para volver a iniciar, se debe presionar de nuevo el botón

![prensa de latas](imgs/Prensado_de_latas.png)

## Selector de cajas

Observar la siguiente animación, la cual consiste en controlar 2 cilindros, los cuales están montados sobre una banda transportadora.
El sistema debe detectar 3 tamaños de cajas, y con base a su altura se deben desplazar hacia otro sitio. Como se muestra en la animación.

![ejemplo neumatica](video/ejemplo_neumatica_2.gif)
