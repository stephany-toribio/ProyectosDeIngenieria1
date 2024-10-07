
<h1 align="center">Ficha técnica</h1>

<h1 align="center">THARU</h1>



## **ESP32** 

**Definición:** El ESP32, es un microcontrolador y de alto desempeño. Este dispositivo cuenta con un procesador Tensilica Xtensa LX6, disponible en versiones de uno o dos núcleos, y ofrece conectividad Wi-Fi y Bluetooth. Su amplia gama de periféricos lo convierte en una opción muy flexible para aplicaciones de Internet de las Cosas (IoT), sistemas embebidos y  proyectoselectrónicos variados.

**Características técnicas**

* **Arquitectura del CPU:** Xtensa 32-bit LX6 dual-core  
* **Frecuencia del CPU:** Hasta 240 MHz  
* **Memoria RAM:** 520 KB SRAM  
* **Memoria Flash:** Hasta 4 MB (integrada o externa)  
* **Wi-Fi:** 802.11 b/g/n, soporte para 2.4 GHz  
* **Bluetooth:** Bluetooth v4.2 BR/EDR y BLE  
* **GPIOs:** 34 pines GPIO, configurables para diversas funciones  
* **Interfaces de comunicación:** SPI, I2S, I2C, UART, CAN, Ethernet MAC  
* **ADC:** 18 canales de 12 bits  
* **DAC:** 2 canales de 8 bits  
* **PWM:** Soporta múltiples canales de PWM  
* **Sensores integrados:** Sensor de temperatura, sensor táctil capacitivo  
* **Seguridad:** Soporte para encriptación AES, SHA-2, RSA, y gestión de claves  
* **Voltaje de operación:** 2.2V \- 3.6V  
* **Consumo de energía:** Modo de bajo consumo (Deep-sleep) \< 10 µA, modo de operación activa \< 240 mA  
* **Temperatura de operación:** \-40°C a 85°C  
* **Soporte de software:** SDK Espressif IDF, Arduino Core, Micropython, y otros  
* **Dimensiones del chip:** Depende del módulo, típicamente 18 mm x 25.5 mm (ESP32-WROOM-32)

[https://www.espressif.com/sites/default/files/documentation/esp32\_datasheet\_en.pdf](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)  
## **GY-BME 280**  
**Definición:** El GY-BME280 es un sensor ambiental versátil que mide la presión barométrica, la temperatura y la humedad relativa. Fabricado por Bosch, este sensor es preciso y eficiente, y se utiliza en una variedad de aplicaciones, como estaciones meteorológicas, dispositivos portátiles, sistemas domóticos y proyectos de IoT. El GY-BME280 proporciona salidas digitales que se pueden integrar fácilmente con microcontroladores y plataformas de desarrollo como Arduino y Raspberry Pi.

**Características técnicas**

* Tipos de medición: Temperatura, humedad y presión barométrica  
* Rango de temperatura: \-40°C a \+85°C  
* Precisión de temperatura: ±1.0°C (rango de \-40°C a \+85°C)  
* Rango de humedad: 0% a 100% RH  
* Precisión de humedad: ±3% RH (rango de 20% a 80% RH)  
* Rango de presión: 300 hPa a 1100 hPa  
* Precisión de presión: ±1 hPa (rango de 300 hPa a 1100 hPa)  
* Interfaz de comunicación: I2C (dirección por defecto 0x76 o 0x77), SPI  
* Voltaje de operación: 1.8V a 3.6V (típicamente 3.3V para módulos comunes)  
* Consumo de energía: Modo normal: 0.6 mA a 1.2 mA, modo de reposo: 0.1 µA  
* Tasa de medición: Hasta 25 Hz en modo de alto rendimiento  
* Dimensiones del módulo: Aproximadamente 15 mm x 10 mm   
* Sensores integrados: Sensor de temperatura, sensor de humedad, sensor de presión  
* Temperatura de almacenamiento: \-40°C a \+85°C
<p align="center">
  <img src="https://github.com/user-attachments/assets/705e78db-bdc0-44ae-8ce1-f2272d130ee7" width="400">
</p>


[https://www.mouser.com/datasheet/2/783/BST-BME280-DS002-1509607.pdf](https://www.mouser.com/datasheet/2/783/BST-BME280-DS002-1509607.pdf)   
## **MQ-7**  
**Definición:** El MQ-7 es un sensor de gas diseñado para detectar monóxido de carbono (CO) en el aire. Utiliza un sensor electroquímico para medir la concentración de CO y genera una señal analógica que puede ser interpretada por microcontroladores como Arduino. Es ampliamente utilizado en aplicaciones de monitoreo de calidad del aire y sistemas de seguridad debido a su alta sensibilidad y rápida respuesta.

**Características técnicas**

* Tipos de medición: Monóxido de carbono (CO)  
* Rango de detección: 20 ppm a 2000 ppm  
* Tiempo de calentamiento: 24 horas  
* Voltaje de operación: 5V ± 0.1V  
* Consumo de energía: 150mA  
* Interfaz de comunicación: Salida analógica  
* Tiempo de respuesta: ≤ 20 segundos  
* Tiempo de recuperación: ≤ 30 segundos  
* Temperatura de operación: \-20°C a \+50°C  
* Humedad de operación: 0% a 95% RH  
* Vida útil: ≥ 5 años  
* Dimensiones del módulo: Aproximadamente 32 mm x 22 mm x 27 mm  
* Sensores integrados: Sensor de gas MQ-7  
* Temperatura de almacenamiento: \-20°C a \+50°C

<p align="center">
  <img src="https://github.com/user-attachments/assets/ae96865a-70ba-46e3-8cff-cd24a88a8535" width="400">
</p>

[https://www.pololu.com/file/0j313/mq7.pdf](https://www.pololu.com/file/0j313/mq7.pdf)   
[https://www.sparkfun.com/datasheets/Sensors/Biometric/MQ-7.pdf](https://www.sparkfun.com/datasheets/Sensors/Biometric/MQ-7.pdf) 

## **ML851** 

**Descripción:** El sensor ML851 utiliza tecnología óptica para detectar y contar partículas en el aire. Funciona mediante el uso de un diodo emisor de luz (LED) y un fotodetector. Cuando las partículas pasana traves del haz de luz emitido por el LED, dispersan la luz, que es detectada por el fotodetector. La cantidad de luz dispersada es proporcional al número  y tamaño de las partículas presentes, lo que permite determinar la concentración de partículas en el aire.

**Características técnicas** 

* Tipos de sensor: Sensor de radiación ultravioleta (UV)  
* Rango de medición UV: 280 nm a 390 nm (UV-A y UV-B)  
* Tiempo de calentamiento: 24 horas  
* Salida analógica: Tensión de salida proporcional a la intensidad UV  
* Voltaje de operación: 2.7V a 3.6V (típicamente 3.3V)  
* Corriente de operación: 300 µA (típico)  
* Modo de ahorro de energía: Modo de espera: 0.1 µA (máx.)  
* Tiempo de respuesta: Menos de 1ms  
* Sensibilidad: Alta sensibilidad con salida analógica lineal  
* Salida máxima de tensión: Aproximadamente 1V (bajo ninguna radiación UV) a 3V (bajo radiación UV intensa)  
* Rango de temperatura de operación: \-20°C a \+70°C  
* Dimensiones del módulo: Aproximadamente 9.5 mm x 8.2 mm x 2.2 mm  
* Conexiones: VCC, GND, OUT (salida analógica), EN (habilitación, se conecta a VCC para activar el sensor)

<p align="center">
  <img src="https://github.com/user-attachments/assets/c98fa77b-06f7-4cd8-b2c1-7c1aebe34b66" width="400">
</p>


[https://cdn.sparkfun.com/datasheets/Sensors/LightImaging/ML8511\_3-8-13.pdf](https://cdn.sparkfun.com/datasheets/Sensors/LightImaging/ML8511_3-8-13.pdf)  
## **MQ-4**

**Definición:** El MQ-4 es un sensor de gas semiconductor diseñado principalmente para detectar gas metano (CH4) y gases naturales. Este sensor es conocido por su alta sensibilidad y su rápida respuesta a las concentraciones de gas, lo que lo hace ideal para aplicaciones como la detección de fugas de gas y la monitorización ambiental.

**Características técnicas:**

* Tipo de sensor: Sensor de gas semiconductor    
* Gases detectados: Metano (CH₄), Gas natural  
* Rango de detección: 200 ppm a 10,000 ppm  
* Tiempo de respuesta: ≤ 10 segundos (típico)  
* Tiempo de calentamiento: ≥ 24 horas  
* Voltaje de operación: 5V ± 0.1V (para el circuito de calentamiento)  
* Corriente de calentamiento: ≤ 150 mA  
* Salida de señal: Analógica, resistencia variable del sensor proporciona  
   a la concentración de gas  
* Sensibilidad: Alta sensibilidad a metano (CH₄)  
* Temperatura de operación: \-20°C a \+50°C  
* Humedad de operación:   95% RH (máximo)  
* Dimensiones del módulo: Aproximadamente 32 mm x 20 mm x 22 mm (puede variar ligeramente según el fabricante del módulo)  
* Calibración: Necesita ser calibrado en el entorno específico de aplicación para obtener resultados precisos  
* Salidas de conexión: VCC, GND, AO (Salida Analógica), DO (Salida Digital, con umbral ajustable en algunos módulos)


<p align="center">
  <img src="https://github.com/user-attachments/assets/9ed38e41-4341-4007-a91c-282f7ad87505" width="400">
</p>



[https://www.sparkfun.com/datasheets/Sensors/Biometric/MQ-4.pdf](https://www.sparkfun.com/datasheets/Sensors/Biometric/MQ-4.pdf) 

## **PMS5003**

**Definición:** El PMS5003 es un sensor de partículas basado en tecnología láser  que se utiliza para medir la concentración de partículas en el aire, tales como  polvo, polen, humo y otras partículas. Es conocido por su alta precisión y capacidad de medición en tiempo real.

**Características técnicas:**

* Tipo de sensor: Sensor de partículas láser  
* Gases detectados:No detecta gases, detecta partículas (PM2.5)  
* Rango de detección: 0 \- 500 µg/m³  
* Tiempo de respuesta:Menos de 10 segundos  
* Tiempo de calentamiento: Menos de 30 segundos  
* Voltaje de operación: 4.5 a 5.5 V DC  
* Corriente de calentamiento: Promedio: ≤ 100mA, Pico: ≤ 200mA  
* Salida de señal:UART (9600bps, 8N1) con datos digitales  
* Sensibilidad: Resolución de 1 µg/m³  
* Temperatura de operación: \-10°C a 60°C  
* Humedad de operación: 0 a 99% RH  
* Dimensiones del módulo: 50 x 38 x 21 mm  
* Calibración: Calibrado de fábrica, no requiere calibración frecuente  
* Salidas de conexión: UART, interfaz de comunicación digital

<p align="center">
  <img src="https://github.com/user-attachments/assets/7de13545-5347-4eb1-b54c-84f6ff79e1c2" width="400">
</p>



[https://www.aqmd.gov/docs/default-source/aq-spec/resources-page/plantower-pms5003-manual\_v2-3.pdf](https://www.aqmd.gov/docs/default-source/aq-spec/resources-page/plantower-pms5003-manual_v2-3.pdf) 

## **MQ-131**

**Definición:** El MQ-131 es un sensor de gas que se utiliza para la detección de  ozono (O3) en el aire. Es conocido por su alta sensibilidad y capacidad para detectar concentraciones bajas de ozono.

**Características del sensor:**

* Tipo de sensor: Sensor de gas semiconductor  
* Gases detectados: Ozono (O3)  
* Rango de detección: 10 ppb a 1 ppm  
* Tiempo de respuesta: Menos de 60 segundos  
* Tiempo de calentamiento: Aprox. 24 horas para alcanzar la máxima   
  estabilidad  
* Voltaje de operación: 5V ± 0.1V DC  
* Corriente de calentamiento: Aproximadamente 150mA  
* Salida de señal: Analógica (variación de resistencia)  
* Sensibilidad: Alta sensibilidad al ozono; también responde a NO2  
* Temperatura de operación: \-10°C a 50°C  
* Humedad de operación: 20% a 90% RH  
* Dimensiones del módulo: 32 mm x 20 mm x 22 mm   
* Calibración: Requiere calibración en aire limpio y seco para una  
   alta precisión  
* Salidas de conexión: Pines estándar para VCC, GND y salida   
  de señal (analog output)  
* Tiempo de vida: 5 años

<p align="center">
  <img src="https://github.com/user-attachments/assets/d70ec779-f4c1-4230-b51c-4636a88e35ef" width="400">
</p>



## **MH-Z19** 

## **Definición:** Mide la concentración de Dióxido de Carbono (CO2) en el aire. Posee un rango de 0 a 5000ppm, compensación por temperatura y la medición es independiente del nivel de oxígeno. Posee dos tipos de salida: UART y PWM. 

**Características del sensor:**

* Tipo de Sensor: NDIR (Non-Dispersive Infrared)  
* Rango de Medición: 0-5000 ppm (partes por millón)  
* Precisión: ± (50 ppm \+ 3% del valor medido)  
* Tiempo de Respuesta: \< 120 segundos  
* Tipos de salida: UART y PWM.   
* Voltaje de Operación: 3.6V \- 5.5V DC  
* Corriente de Operación: \< 18mA  
* Interfaz de Salida: UART (TTL nivel)  
* Tiempo de precalentamiento: \< 3 minutos  
* Vida Útil del Sensor: \> 5 años (bajo uso normal)  
* Temperatura de Operación: 0°C a 50°C  
* Humedad de Operación: 0%-95% RH (sin condensación)  
* Aplicaciones Típicas: Monitoreo de calidad del aire interior, control de  
   ventilación, sistemas de HVAC, seguridad en espacios cerrados.  
* Dimensiones: 33mm x 20mm x 6.8mm  
* Compatibilidad: Compatible con una variedad de microcontroladores y  
   sistemas de adquisición de datos.  
* Instrucciones de Uso: Requiere conexión a un microcontrolador o dispositivo  compatible con UART para recibir y procesar los datos   
* Precauciones: Evitar la exposición a gases corrosivos o inflamables que puedan  dañar el sensor.

<p align="center">
  <img src="https://github.com/user-attachments/assets/402409a8-d5cf-428e-a84e-cc675175a367" width="400">
</p>


[https://www.winsen-sensor.com/d/files/infrared-gas-sensor/mh-z19c-pins-type-co2-manual-ver1\_0.pdf](https://www.winsen-sensor.com/d/files/infrared-gas-sensor/mh-z19c-pins-type-co2-manual-ver1_0.pdf)

## **YL-69 / Medir humedad del suelo**

**Definición:** El sensor YL-69 es un dispositivo utilizado para medir la humedad en el suelo. Este sensor se compone de dos partes principales: la sonda, que se inserta en el terreno para detectar la humedad, y el módulo electrónico, que procesa la señal y la convierte en un valor que puede ser interpretado por un microcontrolador o una plataforma de desarrollo, como Arduino o ESP32. El YL-69 es ampliamente empleado en proyectos de jardinería inteligente, sistemas de riego automático y aplicaciones agrícolas, ya que permite monitorear y mantener niveles óptimos de humedad en el suelo de manera eficiente.

**Características del sensor:**

* Tipo de sensor: Analógico  
* Rango de medición: 0% a 100% humedad relativa del suelo  
* precisión: 5% \- 10% (típico)  
* Voltaje de Operación : 3.3 V \- 5V DC  
* Corriente de Operación: \<35mA  
* Interfaz de Salida: Analógica  
* Temperatura de Operación: \-10°C a 50°C  
* Dimensiones : Compacto y fácil de instalar en el suelo  
* Compatibilidad: Compatible con una variedad de microcontroladores y  
   sistemas de adquisición de datos  
* Instrucciones de Uso: Insertar las puntas del sensor en el suelo y medir  
  la salida analógica para determinar el nivel de humedad del suelo  
* Precauciones : Evitar exposición prolongada a la humedad, calibración   
  periódica puede ser necesaria según las condiciones ambientales y el   
* Tipo de suelo: Evitar exposición prolongada a la humedad, calibración  
   periódica puede ser necesaria según las condiciones ambientales

<p align="center">
  <img src="https://github.com/user-attachments/assets/b71fa090-c769-472d-9c90-63547a7fa7eb" width="400">
</p>

[https://www.electronicoscaldas.com/datasheet/YL-69-HL-69.pdf](https://www.electronicoscaldas.com/datasheet/YL-69-HL-69.pdf) 

## **PIRANÓMETRO**

**Descripción:** El piranómetro GS-WV es el instrumento ideal para mediciones de radiación solar, planificación del riego y automatización de invernaderos. El sensor de radiación solar mide la radiación global solar de 300 hasta 2800 nm, con un amplificador de señal interno y una carcasa impermeable que no requiere mantenimiento solo limpieza incidentalmente del domo de cuarzo.

**Características del sensor:** 

* Tipo de sensor: Sensor de radiación solar (piranómetro)  
* Rango de medición: 0 a 2000 W/m² (puede variar según el modelo)  
* Espectro de respuesta: 300 nm a 2800 nm   
* Sensibilidad: 10 µV/W/m² (típico, puede variar según el modelo)  
* Precisión: ±5% (típico, puede variar según el modelo)  
* Tiempo de respuesta: ≤ 1 segundo (típico)  
* Voltaje de operación: Generalmente, no requiere fuente de alimentación externa   
  (depende del modelo, algunos pueden requerir entre 5V y 12V si tienen amplificador integrado)  
* Temperatura de operación: \-40°C a \+80°C (puede variar según el modelo)  
* Humedad de operación: 0% a 100% RH (resistente a la intemperie)  
* Dimensiones del sensor: Aproximadamente 70 mm de diámetro y 50 mm de altura  
   (puede variar según el modelo)  
* Aplicaciones: Aproximadamente 300 g (puede variar según el modelo)  
* Conexiones: Salida de señal analógica (algunos modelos pueden tener  
   opciones de salida digital, RS-232, o interfaces USB)
<p align="center">
  <img src="https://github.com/user-attachments/assets/e9df7707-526b-40d2-96e0-1b7651a5aad9" width="400">
</p>

