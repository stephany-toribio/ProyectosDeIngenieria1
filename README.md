# Proyecto:  Monitoreo de la calidad del aire y el suelo

Somos un grupo de 5 estudiantes de la carrera de Ingeniería informatíca en la Universidad Peruana Cayetano Heredia,
durante este periodo nosotros como equipo decidimos desarollar  un modulo de parametrización de la calidad del aire y del suelo.

<p align="center"><img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/Imagenes/Grupo/Grupo.jpeg" width="700" height="500" style="margin: auto;"></p>

|Integrantes |Carrera|Cargo|Contacto|
|------------|-------|-----|--------|
|Stephany M. Toribio Alvarado|Ingeniería Informática|Coordinadora de Modelado 3D|stephany.toribio@upch.pe|
|Jose N. Cueva Ramos|Ingeniería Informática|Coordinador de Desarrollo Web |jose.cueva@upch.pe|
|Camilo S. Silva Cuzqui|Ingeniería Informática|Coordinador de IT |camilo.silva@upch.pe|
|Bruno P. Gavidia Crovetto|Ingeniería Informática|Coordinador de Software|bruno.gavidia@upch.pe|
|Jhunior F. Herrera Valeriano|Ingeniería Informática|Coordinador de Hardware|[Linkedin](https://www.linkedin.com/in/jhunior-herrera-valeriano-358350294/)|

## Justificación de la propuesta
La presente propuesta surge como respuesta a la necesidad de generar información referente a parámetros ambientales vinculados al monitoreo de la calidad del aire y del suelo en el campus de Santa María del Mar a través del desarrollo y la implementación de un sistema de monitoreo continuo para la recolección de datos en tiempo real, así como evaluar las posibles rutas de dispersión de fuentes contaminantes del entorno asociados al crecimiento urbano y expansión industrial cerca a la sede, y el diseño de un sistema que busque adaptarse para abordar estas amenazas.

## Objetivos

### Objetivo General

Diseñar e implementar un dispositivo de monitoreo de la calidad del aire y del suelo mediante un módulo integral para el estudio de factores de riesgo ambiental en la sede de Santa María - UPCH.

### Objetivos Específicos

<ul>
    <li>Monitorear la calidad del aire para evaluar la variabilidad climática y la dispersión de los parámetros de estudio con respecto al tiempo.</li>
    <li>Monitorear las condiciones del suelo para evaluar su idoneidad en cuanto a la cobertura vegetal u otros usos.</li>
    <li>Validar y calibrar los sensores low cost de monitoreo en el campus de Santa María.</li>
    <li>Diseñar un módulo de monitoreo que busque el uso de fuentes de energía renovable para disminuir su huella de carbono e impacto en el ambiente.</li>
    <li>Desarrollar una interfaz de usuario amigable para la visualización de datos en tiempo real.</li>
</ul>

## ODS
La propuesta refleja el compromiso de la universidad alineado con los Objetivos de Desarrollo Sostenible (ODS), incorporando específicamente el ODS 7; “Energía Asequible y No Contaminante”; y ODS 11, “Ciudades y Comunidades sostenibles” centrados en el uso de energías renovables como alternativas para la alimentación del sistema, en buscar disminuir la brecha tecnológica con un dispositivo de monitoreo low cost y eficiente, y en el desarrollo de una comunidad universitaria más sostenible a través del monitoreo del impacto de las actividades de la misma en el ambiente para asegurar un espacio propicio para el desarrollo académico y vital para la salud y bienestar de la comunidad universitaria.

<div style="display: flex; justify-content: center; align-items: center; gap: 20px;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/ca/Sustainable_Development_Goal-es-11.jpg" width="400px"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/d/d3/Sustainable_Development_Goal-es-07.jpg" width="400px"/>
</div>

## SENSORES
| **Parámetro**              | **Sensor**   | **Características técnicas**| **Funcionamiento**  |
|----------------------------|--------------|-----------------------------|---------------------|
| **Temperatura**  **Humedad relativa**  **Presión atmosférica**          |              | Voltaje de alimentación: 1.8V - 3.3V DC<br>Rango de Presión: 300 a 1100 hPa<br>Rango de Temperatura: -40°C a 85°C<br>Rango de Humedad Relativa: 0-100% RH                        | Sensor de temperatura, humedad y presión atmosférica.                                                                                     |
| **Radiación UV**           | Piranómetro      | Voltaje de operación: Generalmente, no requiere fuente de alimentación externa(depende del modelo, algunos pueden requerir entre 5V y 12V si tienen amplificador integrado)| El sensor de radiación solar mide la radiación global solar de 300 hasta 2800 nm, con un amplificador de señal interno y una carcasa impermeable que no requiere mantenimiento solo limpieza incidentalmente del domo de cuarzo.|
| **Ozono (O₃)**             | MQ-131       | Voltaje de Operación: 5V DC<br>Rango de detección: 10 a 1000 ppb<br>Resistencia de calefacción: 41 Ohm<br>Tiempo de respuesta: 60 s                                             | Mide concentraciones de Ozono en el aire capaz de detectar concentraciones de hasta 1000 ppb.                                                                                   |
| **Velocidad del viento**   | Anemómetro   | Voltaje del motor: 5-12V DC<br>Voltaje del encoder: 3.3-5V DC  | Mediciones de la velocidad mediante pulsaciones y la variación de voltaje.   |
| **Dirección del viento**  | Veleta |           | Medición de la dirección del viento.       |
| **Material particulado (PM2.5)** | PMS5003      | Rango: 0.3; 1.0; 2.5; 10 µm<br>Voltaje de alimentación: 4.5-5.5V DC<br>Resolución: 1 µg/m³<br>Humedad (trabajo): 0-99% | Principio de dispersión láser para irradiar las partículas en suspensión en el aire.|
| **Monóxido de carbono (CO)** | MQ-7 | Voltaje de alimentación: 5V DC<br>Rango de detección: 20-2000 ppm<br>Resist. de calentamiento: 33Ω ±5%<br>Concentración de Oxígeno: 21% | Sensor electroquímico que varía su resistencia al contacto con el gas.|
| **Dióxido de carbono (CO₂)** | MH-Z19B | Voltaje de alimentación: 3.6-5.5V DC<br>Rango de medición: 0-5000% VOL<br>Humedad de trabajo: 0 - 95% RH (sin condensación)<br>Temperatura de trabajo: 0 - 50°C | Sensor infrarrojo de CO₂, permite detectar dióxido de carbono en el aire. |
| **Metano**  | MQ-4    | Voltaje de operación: 5V<br>Tiempo de respuesta: 10s<br>Potencia de consumo: menor a 900 mW<br>Resistencia de carga: 20kΩ<br>Detección de concentraciones: 200-10000 ppm        | Sensor que mide distintos gases naturales entre ellos el Metano. |
| **Humedad del suelo**       | YL-69        | Voltaje de alimentación: 3.3-5V DC<br>Corriente de alimentación: 35 mA<br>Vatios: 0.175 W  | El sensor detecta la humedad del suelo utilizando una técnica de detección resistiva.  |
| **Otros módulos** | ESP32 (Wi-Fi & Bluetooth) | Voltaje de alimentación: 3.3V DC<br>Corriente de alimentación: 20 mA<br>Vatios: 0.066 W    | Microcontroladores que conectan datos digitales provenientes de los módulos, WiFi y Bluetooth; y permiten que señales electromagnéticas se comuniquen con el router.     


## TRL 1

### Contexto
El proyecto se enfoca en el monitoreo ambiental utilizando sensores especializados para evaluar la calidad del aire, la radiación solar y la calidad del suelo.

### 1. Sensor de Temperatura, Humedad y Presión (BME280)
**Principio tecnológico:** El sensor BME280 es un dispositivo avanzado diseñado para medir temperatura, humedad y presión atmosférica de manera precisa. Emplea un termistor para la detección de temperatura, un sensor de humedad capacitivo para medir la humedad relativa y un sensor piezorresistivo para la medición de presión. Su elección se fundamenta en la combinación de precios competitivos y resultados altamente precisos.

### 2. Piranómetro Solar
**Principio tecnológico:** Este instrumento está diseñado para medir la radiación solar obteniendo espectros magnéticos entre 300 nm a 2800 nm. Este sensor tiene una conexión con salida de señal analógica para que nos dé un espectro continuo en cada tiempo con respuesta ≤ 1 segundo. Su elección se fundamenta en los resultados altamente precisos en comparación con otros sensores.

### 3. Sensor de Ozono (MQ-131)
**Principio tecnológico:** Este sensor está compuesto por un elemento sensible de óxido de estaño (SnO₂) que varía su resistencia en presencia de ozono. Un circuito de medición detecta el cambio de resistencia y lo convierte en una señal eléctrica.

**Ecuación de la recta:**
\[ y = mx + b \]

**Pendiente:**
\[ m = \frac{[\log(y) - \log(y_0)]}{[\log(x) - \log(x_0)]} = \frac{\log(yy_0)}{\log(xx_0)} \]

**Intercepción de Y:**
\[ b = \log(y_b) - m \cdot \log(x_b) = \log(x) = \frac{[\log(y) - b]}{m} \]

**Valor aproximado en ppm:**
\[ x = 10^{\log(y) - bm} \]

### 4. Anemómetro (para Velocidad del Viento)
**Principio tecnológico:** El anemómetro utiliza un rotor con aspas que, al girar con el viento, genera pulsos eléctricos. Estos pulsos son detectados por un encoder que mide el número de rotaciones y las convierte en una señal de voltaje.

### 5. Veleta (para Dirección del Viento)
**Principio tecnológico:** La veleta mide la dirección del viento a través de un sistema mecánico que ajusta un eje en función de la variación en la dirección del viento. Un potenciómetro conectado al eje genera un voltaje variable que refleja dicha dirección. El microcontrolador interpreta este voltaje y lo convierte en un ángulo de dirección del viento, que se visualiza en la interfaz de usuario. Su diseño fue modelado e impreso en material PLA.

### 6. Sensor de Material Particulado (PMS5003)
**Principio tecnológico:** El sensor PMS5003 utiliza un láser y un fotodiodo para detectar partículas en el aire. El láser ilumina las partículas suspendidas, y el fotodiodo mide la luz dispersada. El sensor envía esta información en forma de datos digitales al microcontrolador a través de una interfaz serial UART, que calcula la cantidad y el tamaño de las partículas presentes en el aire (PM2.5, PM10).

### 7. Sensor de Monóxido de Carbono (CO) MQ-7
**Principio tecnológico:** El sensor MQ-7 utiliza un material semiconductor que cambia su resistencia al detectar la presencia de monóxido de carbono.

**Modelo Matemático:**

**Ecuación de la recta:**
\[ y = mx + b \]

**Pendiente:**
\[ m = \frac{[\log(y) - \log(y_0)]}{[\log(x) - \log(x_0)]} = \frac{\log(yy_0)}{\log(xx_0)} \]

**Intercepción de Y:**
\[ b = \log(y_b) - m \cdot \log(x_b) = \log(x) = \frac{[\log(y) - b]}{m} \]

**Valor aproximado en ppm:**
\[ x = 10^{\log(y) - bm} \]

### 8. Sensor de Dióxido de Carbono (CO₂) MH-Z19B
**Principio tecnológico:** Este sensor infrarrojo utiliza el principio de absorción de luz para medir el CO₂. El sensor emite luz infrarroja que pasa a través del aire y es absorbida por el CO₂ en ciertas longitudes de onda. La cantidad de luz absorbida es medida y convertida en un valor de concentración de CO₂, que es transmitido al microcontrolador mediante una señal UART.

### 9. Sensor de Metano (MQ-4)
**Principio tecnológico:** El sensor MQ-4 utiliza un material sensible que cambia su resistencia al estar en contacto con el gas. La variación de resistencia genera una señal que es convertida en voltaje por un circuito.

**Ecuación de la recta:**
\[ y = mx + b \]

**Pendiente:**
\[ m = \frac{[\log(y) - \log(y_0)]}{[\log(x) - \log(x_0)]} = \frac{\log(yy_0)}{\log(xx_0)} \]

**Intercepción de Y:**
\[ b = \log(y_b) - m \cdot \log(x_b) = \log(x) = \frac{[\log(y) - b]}{m} \]

**Valor aproximado en ppm:**
\[ x = 10^{\log(y) - bm} \]

### 10. Sensor de Humedad del Suelo (YL-69)
**Principio tecnológico:** El sensor YL-69 mide la humedad del suelo utilizando una sonda resistiva. A medida que la humedad en el suelo aumenta, la resistencia entre las sondas disminuye. El microcontrolador mide esta resistencia y calcula la cantidad de agua presente en el suelo, permitiendo un monitoreo preciso de las condiciones del suelo.
