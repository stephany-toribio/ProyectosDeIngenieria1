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

| **...** | **Descripción** | 
|-|-|
| **Descripción general**                 | Este sistema esta diseñado para monitorear parámetros clave del **aire** y del **suelo**, el cuál se encuentra equipado con sensores ya calibrados y con un sistema de alimentación por panel solar asegurando el funcionamiento constante para operar.[4]
| **Electrónico (Hardware) e Integración**                 |  El sistema mide la **temperatura, humedad, material particulado, CO2, CO, metano, ozono, radiación UV del aire y CO2 y temperatura del suelo**. Se utilizará una placa **PCB**  que permitirá la integración de todos los sensores en un solo sistema.
| **Software**                 | Recopilación de datos durante **30min** implementando protocolos de **comunicación I2C o SPI**, almacenados en una base de datos, visualizar los datos en gráficos y  descargar los datos en **formato CSV o Excel**. [5]
| **Resistencia y Geometría** |            Presenta un peso máximo : **12.8 N** y el peso del soporte y componentes energéticos es menor igual a  **102.5 N** y las dimensiones del prototipo son de **22 cm x 22.5 cm x 13.4 cm**.
| **Mantenimiento y sostenibilidada** |            El plan de mantenimiento que se realizara cada **2 meses** consta de calibración, limpieza y verificación del estado de los componentes. Por el lado de la sostenibilidad, se utilizará un polímero biodegradable para reducir el impacto ambiental como el ácido poliláctico (**PLA**). 

# Marco legal
Ley N° 28611, Ley General del Ambiente 
En el artículo 133 se establece que “la vigilancia y el monitoreo ambiental tienen como fin generar la información que permita orientar la adopción de medidas que aseguren el cumplimiento de los objetivos de la política y normativa ambiental. La Autoridad Ambiental Nacional establece los criterios para el desarrollo de las acciones de vigilancia y monitoreo”.
D.S. 003-2017-MINAM, Estándares de Calidad Ambiental  para aire y establecen disposiciones complementarias 
Determina los niveles de concentración máxima de contaminantes del aire en su condición de  cuerpo receptor, con la finalidad de garantizar el bienestar de la salud pública y la conservación de la calidad ambiental.

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

## Referencias bibliográficas
- [1] "Mapa de la calidad del aire de Lima", IQAir. https://www.iqair.com/es/air-quality-map/peru/lima?srsltid=AfmBOopwM0paCNeouABMqZmJEZUl5LN06b_j0DpkatJDI7UwTqjHL-NP.
  
- [2] R. Quiza, L. A. V. Fajardo, and Y. J. C. Hernández, "Arquitectura de monitoreo inteligente y de bajo costo para sistemas y procesos mecánicos," Low-cost intelligent monitoring architecture for mechanical systems and processes.

- [3] "Fenómeno El Niño", Servicio Nacional de Meteorología e Hidrología del Perú (SENAMHI). [En línea]. Disponible: https://www.senamhi.gob.pe/?p=fenomeno-el-nino, 2024.

- [4] ISO 14001:2015(es), Sistemas de gestión ambiental—Requisitos con orientación para su uso. (s. f.). Recuperado 6 de octubre de 2024, de https://www.iso.org/obp/ui#iso:std:iso:14001:ed-3:v1:es
  
- [5] ISO 27001—Certificado ISO 27001 punto por punto—Presupuesto Online. (s. f.). Norma ISO 27001. Recuperado 6 de octubre de 2024, de https://www.normaiso27001.es/
