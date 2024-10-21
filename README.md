# Proyecto:  Monitoreo de la calidad del aire y el suelo

Somos un grupo de 5 estudiantes de la carrera de Ingeniería informatíca en la Universidad Peruana Cayetano Heredia,
durante este periodo nosotros como equipo decidimos desarollar  un modulo de parametrización de la calidad del aire y del suelo.

<p align="center"><img src="https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/Imagenes/Grupo/Grupo.jpeg" width="700" height="700" style="margin: auto;"></p>

|Integrantes |Carrera|Cargo|Contacto|
|------------|-------|-----|--------|
|Stephany M. Toribio Alvarado|Ingeniería Informática|Coordinadora de Modelado 3D|stephany.toribio@upch.pe|
|Jose N. Cueva Ramos|Ingeniería Informática|Coordinador de Desarrollo Web |jose.cueva@upch.pe|
|Camilo S. Silva Cuzqui|Ingeniería Informática|Coordinador de IT |camilo.silva@upch.pe|
|Bruno P. Gavidia Crovetto|Ingeniería Informática|Coordinador de Software|bruno.gavidia@upch.pe|
|Jhunior F. Herrera Valeriano|Ingeniería Informática|Coordinador de Hardware|[Linkedin](https://www.linkedin.com/in/jhunior-herrera-valeriano-358350294/)|


## ODS
 La propuesta refleja el compromiso de la universidad alineado con los Objetivos de Desarrollo Sostenible (ODS), incorporando específicamente el ODS 7; “Energía Asequible y No Contaminante”; y ODS 11, “Ciudades y Comunidades sostenibles” centrados en el uso de energías renovables como alternativas para la alimentación del sistema, en buscar disminuir la brecha tecnológica con un dispositivo de monitoreo low cost y eficiente, y en el desarrollo de una comunidad universitaria más sostenible a través del monitoreo del impacto de las actividades de la misma en el ambiente para asegurar un espacio propicio para el desarrollo académico y vital para la salud y bienestar de la comunidad universitaria.

<div style="display: flex; justify-content: space-between;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/ca/Sustainable_Development_Goal-es-11.jpg" width="500px"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/d/d3/Sustainable_Development_Goal-es-07.jpg" width="500px"/>
</div>

## SENSORES
| **Parámetro**              | **Sensor**   | **Características técnicas**| **Funcionamiento**  |
|----------------------------|--------------|-----------------------------|---------------------|
| **Temperatura**            |              | Voltaje de alimentación: 1.8V - 3.3V DC<br>Rango de Presión: 300 a 1100 hPa<br>Rango de Temperatura: -40°C a 85°C<br>Rango de Humedad Relativa: 0-100% RH                        | Sensor de temperatura, humedad y presión atmosférica.                                                                                     |
| **Humedad relativa**       |              |                                 |                  |
| **Presión atmosférica**    |              |                                 |                  |
| **Radiación UV**           | ML8511       | Voltaje de alimentación: 5V DC<br>Corriente de alimentación: 300 µA<br>Vatio: 0.0015 W<br>Rango de detección: 280-390 nm  | Convertidor analógico digital, que convierte la foto-corriente en voltaje en función de la cantidad de radiación UV.     |
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
