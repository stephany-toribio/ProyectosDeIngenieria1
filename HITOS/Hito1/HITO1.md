<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">HITO I</h1>
</p>
 
# Descripción del problema 
La presente propuesta surge como respuesta a la carencia de información referente a parámetros ambientales vinculados al monitoreo de la calidad del aire y del suelo en el campus de Santa María del Mar [1], lo que impide comprender el impacto del crecimiento urbano y la expansión industrial en la zona.  

# Estrategia solución 
La implementación de un sistema de monitoreo ambiental para la recolección de datos en tiempo real que permita establecer una línea base sobre la calidad ambiental para futuras investigaciones y proyectos desarrollados por la comunidad universitaria y, de esta manera, contribuir a la investigación científica e innovación tecnológica en materia ambiental. 

## Justificación de la propuesta
Esta propuesta refleja el compromiso con los Objetivos de Desarrollo Sostenible (ODS), incorporando específicamente el ODS 7; “Energía Asequible y No Contaminante”; y ODS 11, “Ciudades y Comunidades sostenibles” centrados en el uso de energías renovables como alternativas para la alimentación del sistema. Esta alternativa busca disminuir la brecha tecnológica con un dispositivo de monitoreo low cost y eficiente, y en el desarrollo de una comunidad universitaria más sostenible a través del monitoreo del impacto de las actividades de la misma en el ambiente para asegurar un espacio propicio para el desarrollo académico y vital para la salud y bienestar de la comunidad universitaria [2]. En concordancia a ello, el proyecto busca establecer una línea base sobre la calidad ambiental para futuras investigaciones y proyectos desarrollados por la comunidad universitaria y, de esta manera, contribuir a la investigación científica e innovación tecnológica en materia ambiental.

## Justificación del área de estudio
La elección de Santa María como sede para la implementación del proyecto se fundamenta en su condición de área relativamente reciente y perteneciente a la Universidad Peruana Cayetano Heredia, donde todavía no se han llevado a cabo estudios exhaustivos en referente a parámetros de calidad del aire y del suelo en la medida necesaria. Ubicada en el km 4.5 de la carretera Panamericana Sur con coordenadas geográficas 12°25’03.87”S y 76°45’18.39”W a una altitud de 424 m.s.n.m, este proyecto se decidió ejecutar en dicha zona en función a la cercanía a la carretera, la cual registra a un alto tránsito vehicular; sobre todo en épocas de verano, donde existe una mayor afluencia de usuarios que se dirigen a las playas del sur. Durante la duración del proyecto, se considerará la transición y los cambios estacionales, puesto que ante el pronosticado “fenómeno del niño global”, la variación de los patrones climáticos será significativa [3]. Lo anterior producirá que las estaciones no se vean marcadas dado que alterará el periodo de verano de enero-marzo, meses en los que se ejecutará el proyecto. Estos cambios estacionales influyen directamente en factores como la dirección y velocidad del viento, deposición húmeda y variación en la temperatura, que están relacionados con la concentración de los contaminantes. En relación con los parámetros del suelo, también contribuye a alterar la presencia de humedad, salinidad y conductividad, por lo que se reitera la importancia de un seguimiento período de estas variables.

# Objetivos

## Objetivo General
Diseñar e implementar un dispositivo de monitoreo de la calidad del aire y del suelo mediante un módulo integral para el estudio de factores de riesgo ambiental en la sede de Santa María - UPCH.

## Objetivos Específicos
- Monitorear la calidad del aire para evaluar la variabilidad climática y la dispersión de los parámetros de estudio con respecto al tiempo.
- Monitorear las condiciones del suelo para evaluar su idoneidad en cuanto a la cobertura vegetal u otros usos.
- Validar y calibrar los sensores low cost de monitoreo en el campus de Santa María. 
- Diseñar un módulo de monitoreo que busque el uso de fuentes de energía renovable para disminuir su huella de carbono e impacto en el ambiente.
- Desarrollar una interfaz de usuario amigable para la visualización de datos en tiempo real.

# Requerimientos de la propuesta 

|-|Proyecto|Hera-Tharu|
|----|-----------------------|------|
|-|Cliente|UNIVERSIDAD PERUANA CAYETANO HEREDIA|
|-|**Páginas:** |2 | 
|-|**Edición:**| 0.2 |
|-|**Proyecto:**|Hera-Tharu| 
|-|**Fecha:**| 06/10/2024|
|-|**Cliente:**| UNIVERSIDAD PERUANA CAYETANO HEREDIA|  
|-|**Elaborado:**| J.H, S.T, B.G, J.C, S.S|

| **Deseo o Exigencia** | **Descripción** | **Responsable** |
|-|-|-|
| **E**                 | **Función principal:** El sistema debe monitorear los parámetros que se establecerán relacionados con el aire y del suelo en la sede de Santa María. Lo anterior según la Norma - ISO 14001 (Sistemas de gestión ambiental) [4] | J.H, S.T, B.G, J.C, S.S |
| **E**                 | **Cuantificación:** Todos los sensores deben estar calibrados de acuerdo con las normativas vigentes y los estándares internacionales de medición para garantizar la precisión de los datos obtenidos. El proceso de calibración debe realizarse de manera periódica, y se implementarán mecanismos de notificación en caso de que algún sensor requiera recalibración. Ello según la Norma - ISO 10012 (Sistemas de gestión de medición) [5] y la Norma - ISO 17025 (Requisitos generales para la competencia de laboratorios de ensayo y calibración) [6] | J.H, S.T, B.G, J.C, S.S |
| **E**                 | **Energía:** Se debe asegurar que el sistema cuente con un suministro de energía adecuado para soportar largos períodos de operación. El sistema utilizará un amperaje de 9 y contará con un panel solar de 20W para recargar la batería. | B.G |
| **E**                 | **Señales (Información):** Los protocolos de comunicación utilizados serán I2C y SPI, conforme a las especificaciones de los sensores. | J.C |
| **E**                 | **Resistencia Estructural:** El peso máximo del prototipo será de 12.8N. Con el soporte metálico y componentes energéticos (panel solar y cargador de batería), el peso total no deberá exceder los 102.5N. | S.S |
| **E**                 | **Electrónico (Hardware):** El sistema estará equipado con nueve sensores diseñados para medir diversos parámetros de la calidad del aire, los cuales incluyen la temperatura y la humedad, la concentración de CO2 en el aire, metano, monóxido de carbono, ozono y parámetros en la calidad del suelo, los cuales incluyen la humedad y CO2 del suelo. | J.H |
| **E**                 | **Software:** <br> **Recopilación de Datos:** El sistema debe ser capaz de recopilar mediciones durante 30 minutos y calcular el promedio para luego ser enviados a la base de datos. Debe implementar los protocolos de comunicación I2C y SPI para la integración con los sensores. <br> **Almacenamiento de Datos:** Los datos recopilados deben ser almacenados en una base de datos (local o en la nube). La base de datos debe poder gestionar múltiples tipos de sensores, almacenando la fecha, hora y ubicación de cada medición. El sistema debe realizar copias de seguridad periódicas para evitar pérdida de datos. <br> **Presentación de Datos:** Se debe desarrollar una página web que permita a los usuarios: Visualizar los datos mediante gráficos interactivos. Descargar los datos en formato CSV o Excel. La página web debe ser accesible desde cualquier navegador y adaptarse a diferentes tamaños de pantalla (responsiva). Lo anterior según la Norma - ISO 27001 [7]. | J.C, B.G, S.S |
| **D**                 | **Predicción:** Se implementarán modelos de machine learning para la predicción de parámetros basados en los datos obtenidos por los sensores. | J.H, S.T, B.G, J.C, S.S |
| **D**                 | **Geometría:** El tamaño del prototipo, incluyendo todos los componentes físicos, no deberá exceder de las dimensiones de 22 cm x 22.5 cm x 13.4 cm. | S.T |
| **E**                 | **Sostenibilidad:** El sistema utilizará materiales sostenibles, como el ácido poliláctico (PLA), un polímero biodegradable que contribuye a la reducción del impacto ambiental. Además, contará con un panel solar y una batería recargable para su funcionamiento. | S.T |
| **E**                 | **Durabilidad:** Se incluirán coberturas protectoras para los sensores y la placa PCB, además de rendijas y sombrillas que prevendrán la entrada de agua de lluvia y otros materiales que puedan afectar el funcionamiento del sistema. | S.T |
| **E**                 | **Escalabilidad:** El sistema será escalable para integrar sensores adicionales o para la expansión de las áreas de monitoreo. Además, se garantizará su compatibilidad con plataformas IoT, facilitando la conexión con dispositivos externos y redes existentes. | J.H, S.T, B.G, J.C, S.S |
| **E**                 | **Integración:** Se diseñará una placa PCB que permitirá la integración de todos los sensores en un solo sistema, evitando el exceso de cableado. | J.H, B.G, S.S |
| **D**                 | **Mantenimiento:** El sistema deberá contar con un plan de mantenimiento que garantice su óptimo funcionamiento. Este plan incluirá la revisión periódica de la calibración de los sensores, la limpieza de los componentes externos, y la verificación del estado del panel solar y de la batería, con el fin de asegurar un suministro de energía constante y un rendimiento fiable del sistema. Se recomienda realizar estas tareas cada dos meses. | J.H, S.T, B.G, J.C, S.S |
| **E**                 | **Costos:** El presupuesto estimado del proyecto es de 2700 soles, con una contingencia de 300 soles. | |

# Marco legal
La Ley N° 28611, Ley General del Ambiente en el artículo 133 
<a href="HITOS/Hito1/Avances/docs/ECAs_Aire_DS-003-2017-minam (1).pdf" target="_blank">ECAs Aire DS-003-2017-MINAM</a>, en la cual se establece que “la vigilancia y el monitoreo ambiental tienen como fin generar la información que permita orientar la adopción de medidas que aseguren el cumplimiento de los objetivos de la política y normativa ambiental. La Autoridad Ambiental Nacional establece los criterios para el desarrollo de las acciones de vigilancia y monitoreo”.
D.S. 003-2017-MINAM, Estándares de Calidad Ambiental  para el aire y establecen disposiciones complementarias.  Así como tambien, se determina los niveles de concentración máxima de contaminantes del aire en su condición de  cuerpo receptor, con la finalidad de garantizar el bienestar de la salud pública y la conservación de la calidad ambiental. A continuación, se muestra la tabla: 
| **Parámetros**                                  | **Período** | **Valor [µg/m³]** | **Criterios de evaluación**             | **Método de análisis**                                       |
|-------------------------------------------------|-------------|-------------------|-----------------------------------------|--------------------------------------------------------------|
| Material Particulado con diámetro menor a 2.5 micras (PM₂.₅) | 24 horas    | 50                | NE más de 7 veces al año               | Separación inercial/filtración (Gravimetría)                  |
|                                                 | Anual       | 25                | Media aritmética anual                  |                                                              |
| Material Particulado con diámetro menor a 10 micras (PM₁₀)  | 24 horas    | 100               | NE más de 7 veces al año               | Separación inercial/filtración (Gravimetría)                  |
|                                                 | Anual       | 50                | Media aritmética anual                  |                                                              |
| Monóxido de Carbono (CO)                        | 1 hora      | 30000             | NE más de 1 vez al año                 | Infrarrojo no dispersivo (NDIR) (Método no automático)        |
|                                                 | 8 horas     | 10000             | Media aritmética móvil                 |                                                              |

*NE: No exceder* 
D.S. 010-2019-MINAM, Protocolo Nacional de Monitoreo de la Calidad Ambiental del Aire 
Conforme al acápite G del Protocolo estipula que los sensores de bajo costo, o también llamados “Low cost sensors”, son considerados como un procedimiento de medición alternativo. Asimismo, los resultados obtenidos a partir de dichos instrumentos sólo pueden ser comparados con los Estándares de Calidad Ambiental (ECA).

En cuánto a las <a href="HITOS/Hito1/Avances/docs/CO2_normas" target="_blank">normas de estadarización del CO2 en el aire</a>
se establecen valores de 300 a 400 ppm.

## Referencias bibliográficas
- [1] "Mapa de la calidad del aire de Lima", IQAir. https://www.iqair.com/es/air-quality-map/peru/lima?srsltid=AfmBOopwM0paCNeouABMqZmJEZUl5LN06b_j0DpkatJDI7UwTqjHL-NP.
  
- [2] R. Quiza, L. A. V. Fajardo, and Y. J. C. Hernández, "Arquitectura de monitoreo inteligente y de bajo costo para sistemas y procesos mecánicos," Low-cost intelligent monitoring architecture for mechanical systems and processes.

- [3] "Fenómeno El Niño", Servicio Nacional de Meteorología e Hidrología del Perú (SENAMHI). [En línea]. Disponible: https://www.senamhi.gob.pe/?p=fenomeno-el-nino, 2024.
  
- [4] ISO 14001:2015(es), Sistemas de gestión ambiental—Requisitos con orientación para su uso. (s. f.). Recuperado 6 de octubre de 2024, de https://www.iso.org/obp/ui#iso:std:iso:14001:ed-3:v1:es
  
- [5] ISO 10012:2003(es), Sistemas de gestión de las mediciones—Requisitos para los procesos de medición y los equipos de medición. (s. f.). Recuperado 6 de octubre de 2024, de https://www.iso.org/obp/ui#iso%3Astd%3Aiso%3A10012%3Aed-1%3Av1%3Aes

- [6] ISO/IEC 17025:2017(es), Requisitos generales para la competencia de los laboratorios de ensayo y calibración. (s. f.). Recuperado 6 de octubre de 2024, de https://www.iso.org/obp/ui/#iso:std:iso-iec:17025:ed-3:v2:es
  
- [7]  ISO 27001—Certificado ISO 27001 punto por punto—Presupuesto Online. (s. f.). Norma ISO 27001. Recuperado 6 de octubre de 2024, de https://www.normaiso27001.es/
