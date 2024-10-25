# Prácticas de clase - Circuitos Neumáticos

## Ejercicios Construyendo circuitos básicos

Construir el siguiente circuito neumático.

Accionar un cilindro de simple efecto con retorno de muelle, con una válvula 3/2 de accionamiento manual con retorno de muelle.

![básico](imgs/basico_1.png)

![básico](video/basico_1.gif)

---

## Tipos de accionamientos

![accionamientos](imgs/accionamientos.png)

### Accionamiento directo

![accionamiento directo](imgs/accionamiento_directo.png)

![accionamiento directo](imgs/accionamiento_directo.png)

### Accionamiento indirecto

![accionamiento indirecto](imgs/accionamiento_indirecto.png)

![accionamiento indirecto](video/accionamiento_indirecto.gif)

!!! note
    El accionamiento correcto es el control indirecto, dado que es el más seguro para el usuario ante cualquier falla o contingencia.

---

## Ejercicios

### Ejercicio 1

Control de un cilindro de simple efecto con retorno de muelle, gobernado por una válvula de presión con retorno de muelle; las válvulas de control restantes son a elección propia del ingeniero (*Es con control indirecto*).

Solución:

<details>
    <img src="imgs/circuito_1.png" alt="circuito">
</details>

### Ejercicio 2

Control de un cilindro de simple efecto con retorno de muelle, gobernado por una válvula de presión biestable, las válvulas de control restantes son a elección propia del ingeniero.

Solución

<details>
<img src="imgs/circuito_2.png" alt="circuito">
</details>

### Nomenclatura de circuitos neumáticos

#### Ejercicio 3

Reproducir el siguiente diagrama y describir su funcionamiento

![doble or](video/circuito_doble_or.gif)

---

## Accionamiento por rodillo

Presentación y configuración por accionamiento de rodillo:

![rodillo1](imgs/accionando_rodillo.png)

### Configuración de la válvula por rodillo y cilindro

Primero damos doble click sobre el rodillo o el cilindro

![paso 1](imgs/paso_1.png)

Si damos doble click sobre el rodillo, nos saldrá esta ventana donde colocamos la referencia que nos servirá para identificarlo. Por convención, se usa **A, B, C,...**

![paso 2](imgs/paso_2.png)

Damos **Aceptar**, y nos quedara la referencia del rodillo.

![paso 3](imgs/paso_3.png)

Ahora, si damos doble click sobre el cilindro, nos saldrá la siguiente ventana y  nos vamos a la pestaña "Etiquetas de accionamiento".

En esta sección debemos agregar la marca que se vinculara con el rodillo o sensor

![paso 4](imgs/paso_4.png)

Se coloca la marca **"A"** y en la posición que queremos que exista el sensor o que se accione, en este caso solo queremos que este unicamente al final del cilindro.

![paso 5](imgs/paso_5.png)

Aceptamos, y nos quedara la marca sobre el cilindro, dependiendo de donde lo hayamos configurado.

![paso 6](imgs/paso_6.png)

![paso 7](imgs/paso_7.png)

<details>
    <img src="video/accionando_rodillo.gif" alt="circuito">
</details>

---

#### Ejercicio 4

**1. Se debe controlar un cilindro de doble efecto, por medio de un botón, *Y* al mismo tiempo debe estar presionado una válvula por rodillo. Para que regrese el vástago del cilindro debe ser presionado otro botón**

Solución:

<details>
    <img src="imgs/accionamiento_rodillo.png" alt="circuito">
    <br>
    <img src="imgs/ejercicio_1_1.png" alt="circuito">
    <br>
    <img src="imgs/ejercicio_1_2.png" alt="circuito">
    <br>
    <img src="video/ejercicio_rodillo.gif" alt="circuito">

</details>

---

### Circuito A+ B+ A- B-

Se debe accionar una válvula de manera manual para hacer salir el vástago del cilindro de doble efecto 1, cuando éste al 100% deber hacer salir el vástago del cilindro de doble efecto 2, cuando éste vástago este al 100% debe hacer regresar al vástago del cilindro de doble efecto 1 y el cilindro de doble efecto 2.

<details markdown="1">
    <img src="imgs/a_mas_b_mas.png" alt="circuito">
    <img src="imgs/a_mas_b_mas_2.png" alt="circuito">
    <img src="video/a_mas_b_mas.gif" alt="circuito">
</details>

### Circuito A+ B+ B- A- (Descapotable)

Limites 95 y 5

<details markdown="1">
    <img src="imgs/A+B+B-A-_descapotable.png" alt="circuito">
</details>

---

## Control de salida del vástago

![](video/estranguladora_check_1.gif)

---

## Aplicaciones

### Control de puerta de un autobús

**El control de apertura y cierre de la puerta de un autobús es llevada a cabo por el chofer que acciona un botón para abrirla y otro botón para cerrarla. Pero para que este sistema funcione el autobus debe estar detenido, es decir, se debe estar presionando el freno (accionamiento por rodillo). Ademas, por fuera, debe existir un botón de enclavamiento (accionamiento por bloqueo con retorno de muelle), el cual debe abrir la puerta del autobus.
La entrada y salida del vástago es lenta, a un 50% en su cierre y a un 30% su apertura.**

### Elevador Simple

Tenemos un elevador, el cual se controla por medio de dos pulsadores, con uno podemos subir la plataforma (PS), y con el otro podemos bajar la plataforma (PB). Realiza un circuito neumático para el control, estos pulsadores esta en la parte inferior donde el operador realiza el control.

![elevador](imgs/eleveador_simple.png)

<details markdown="1">
    <img src="imgs/elevador_diagama.png" alt="circuito">

</details>

---

### Elevador (completo)

Ahora el elevador tiene doble control, es decir, cuenta con 4 botones para hacerlo funcionar. Tenemos 2 botones dentro del cajon que sube y en la parte inferior de la plataforma.
2 botones para subir, uno arriba y otro abajo, otros 2 para subir, arriba y abajo.

![elevador](imgs/elevador_full.png)

<details markdown="1">
    <img src="imgs/elevador_full_circuito.png" alt="circuito">
    <br>
    <img src="imgs/elevador.png" alt="circuito">
    <br>
    <img src="video/elevador.gif" alt="circuito">`

</details>

---

### Martillo neumático

---

### Papas a la francesa

**Se debe realizar un circuito neumático para el control del cortador de papas. Para que este funcione se deben cumplir 2 condiciones, con el pie el usuario lo debe activar, en la parte superior debe haber otra aplacan, cuando ambos estén accionados, la maquina comienza a operar automáticamente, es decir, saliendo y entrando el vástago del cilindro. Cuando se desactive por medio de la aplacan o el pedal, se debe detener.
De protección, se debe colocar una válvula principal para detener el flujo de aire del sistema.**

![papas a la francesa](video/ejemplo_neumatica_5.gif)
