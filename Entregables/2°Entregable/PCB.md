<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">Nueva PCB</h1>
</p>

Partiendo de nuestra primera configuración de circuito electrónico, fue impresa por un servicio de terceros obteniendo nuetra primera placa PCB.

<p align="center">
  <img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/HITOS/Hito1/Avances/imgs/PCB%20inicial.jpg" alt="PCB incial" width=55%> 
<p align="center" class="note text-center note-white">FUENTE: Figura 1(PCB). Elaboración Propia</p>

Posteriormente, teninedo posesion de la pcb comensamos a soldar y colocar los respectivos sensores, resitencias, transitores y borneras como se observara en las imagenes de acontinuación.

<p align="center">
  <img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/HITOS/Hito1/Avances/imgs/PCB%20ENSAMBLADA.jpg" alt="PCB ensamblada" width="40%">
  <img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/HITOS/Hito1/Avances/imgs/PCB-ENSABLADA2.jpg" alt="PCB ensamblada 2" width="40%">
</p>
<p align="center" class="note text-center note-white">FUENTE: Figura 2(PCB). Elaboración Propia</p>


En la siguiente carpeta tendra una carpeta de imagenes con la visualizacion del funcionamiento de la mayoria de lo sensores(antes de soldarlo en la pcb), sensores en especifico(BM280, MQ-131, MQ-4, MQ-7) y una carpeta de videos en donde observara el funcionamiento de los sensores conectados

[Carpeta Evidencias](https://github.com/stephany-toribio/ProyectosDeIngenieria1/tree/main/Entregables/2%C2%B0Entregable/Evidencia)

<p align="left">
  <h2 align="center">Modificación posterior</h2>
</p>

Nuestro circuito electronico ha sufrido cambios comparado con la pcb que mostramos con anterioridad, primero explicaremos las conexiones y luego mencionaremos los cambios que se realizaron.


1. Teensy (microcontrolador)
     - El microcontrolador Tensy recibira todas las señales de los sensores conectados a sus pines.
     - Su voltaje al cual haremos funcionar sera de 5v y sus pines de funcionaran a 3.3v.
2. MQ-7
     - Se encontrara conectado a traves de un divisor de voltaje formado con resistencias al Teensy.
     - Su voltaje de operacion es de 5v y debido al divisor de voltaje logra conectarse al teensy trabaja a 3.3v.
     - Medira el monoxido de oxigeno.
3. MQ4
    - Se encontrara conectado a traves de un divisor de voltaje formado con resistencias al Teensy.
    - Su voltaje de operacion es de 5v y debido al divisor de voltaje logra conectarse al teensy trabaja a 3.3v.
    - Medira el metano 
4. MQ-131
    - Se encontrara conectado a traves de un divisor de voltaje formado con resistencias al Teensy.
    - Su voltaje de operacion es de 5v y debido al divisor de voltaje logra conectarse al teensy trabaja a 3.3v.
    - Medira el ozono.
5. MHZ-19
    - Se encontrara conectado directamente al Teensy.
    - Su voltaje de alimentacion es de 5v y su voltaje de operacion es de 3.3v, por tanto en este caso no requiere de un divisor de voltaje.
    - Medira el dioxido de carbono.
6. GY-BME-280
    - Se encontrara conectado directamente al Teensy.
    - Su voltaje de alimentacion es de 3.3v y su voltaje de operacion es de 3.3v, por tanto en este caso no requiere de un divisor de voltaje.
    - Medira Temperatura y humedad en el ambiente.
7. YL-69
    - Se encontrara conectado a traves de un divisor de voltaje formado con resistencias al Teensy.
    - Su voltaje de operacion es de 5v y debido al divisor de voltaje logra conectarse al teensy trabaja a 3.3v.
    - Medira la humedad del suelo
8. PMS-5003
    - Se encontrara conectado directamente al Teensy.
    - Su voltaje de alimentacion es de 5v y su voltaje de operacion es de 3.3v, por tanto en este caso no requiere de un divisor de voltaje.
9. Piranometro
    - Se encontrara conectado a un transceptor de comunicación (MAX 485) necesario para la comunicacion con el microcontrolador, en este caso el teensy.
    - Su voltaje de operacion es de 12 v por tanto a traves de un transistor se reducira su voltaje de operacion a 5v para poder usar el max485.
    1. Max-485
        - Se encontrara conectado directamente al Teensy.
        - Su voltaje de alimentacion es 3.3v y su voltaje de operacion es de 3.3v, por tanto en este caso no requiere de un divisor de voltaje.
    - Medira la radiacion solar
10. SIM800L
    - Se encontrara conectado directamente al Teensy.
    - Su voltaje de alimentacion es de 5v y su voltaje de operacion es de 3.3v, por tanto en este caso no requiere de un divisor de voltaje.
    - Mandara la informacion recolectada a Thingspeak (software de visualizacion de datos).

### Comparación

A continuacion explicaremos los cambios realizados y comparando con la antigua pcb.

1. Se cambio el microcontrolador de esp32 a teensy, para optimizar las conexiones de los puertos uart y los demas pines.
2. Se agrego una bornera para la sim800l y se dejo de utilizar el SC16IS750, placa usada para ampliar puertos uart
3. Cambios todos los pines por borneras para un mayor compacto y seguridad con las conexiones.


<p align="center">
  <img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/HITOS/Hito1/Avances/imgs/Circuito_antiguo.png" alt="PCB ensamblada" width="48%">
  <img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/HITOS/Hito1/Avances/imgs/Circuito_PI_G3.jpg" alt="PCB ensamblada 2" width="48%">
</p>
<p align="center" class="note text-center note-white" > Izquierda circuito antiguo --- Derecha circuito actualizado </p>
<p align="center" class="note text-center note-white">FUENTE: Figura 3(Circuito electricos). Elaboración Propia</p>
