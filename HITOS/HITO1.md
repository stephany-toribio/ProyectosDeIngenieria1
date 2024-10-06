<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">HITO I</h1>
</p>
 
# Justificación de la propuesta

La presente propuesta surge como respuesta a la necesidad de generar información referente a parámetros ambientales vinculados al monitoreo de la calidad del aire y del suelo en el campus de Santa María del Mar a través del desarrollo y la implementación de un sistema de monitoreo continuo para la recolección de datos en tiempo real, así como evaluar las posibles rutas de dispersión de fuentes contaminantes del entorno asociados al crecimiento urbano y expansión industrial cerca a la sede, y el diseño de un sistema que busque adaptarse para abordar estas amenazas. Asimismo, la propuesta refleja el compromiso de la universidad alineado con los Objetivos de Desarrollo Sostenible (ODS), incorporando específicamente el ODS 7; “Energía Asequible y No Contaminante”; y ODS 11, “Ciudades y Comunidades sostenibles” centrados en el uso de energías renovables como alternativas para la alimentación del sistema, en buscar disminuir la brecha tecnológica con un dispositivo de monitoreo low cost y eficiente, y en el desarrollo de una comunidad universitaria más sostenible a través del monitoreo del impacto de las actividades de la misma en el ambiente para asegurar un espacio propicio para el desarrollo académico y vital para la salud y bienestar de la comunidad universitaria
En concordancia a ello, el proyecto busca establecer una línea base sobre la calidad ambiental para futuras investigaciones y proyectos desarrollados por la comunidad universitaria y, de esta manera, contribuir a la investigación científica e innovación tecnológica en materia ambiental. Este dispositivo busca abordar desafíos futuros para asegurar el bienestar de la comunidad herediana a largo plazo con la visión de convertirse en un campus universitario en los próximos años, el sistema permitirá conocer la calidad ambiental del entorno.


# Objetivos

## Objetivo General
Diseñar e implementar un dispositivo de monitoreo de la calidad del aire y del suelo mediante un módulo integral para el estudio de factores de riesgo ambiental en la sede de Santa María - UPCH.

## Objetivos Específicos
Monitorear la calidad del aire para evaluar la variabilidad climática y la dispersión de los parámetros de estudio con respecto al tiempo.
Monitorear las condiciones del suelo para evaluar su idoneidad en cuanto a la cobertura vegetal u otros usos.
Validar y calibrar los sensores low cost de monitoreo en el campus de Santa María. 
Diseñar un módulo de monitoreo que busque el uso de fuentes de energía renovable para disminuir su huella de carbono e impacto en el ambiente.
Desarrollar una interfaz de usuario amigable para la visualización de datos en tiempo real.

## Justificación del área de estudio
La selección de Santa María como sede para la implementación del proyecto se fundamenta en su condición de área relativamente reciente y perteneciente a la Universidad Peruana Cayetano Heredia, donde todavía no se han llevado a cabo estudios exhaustivos en referente a parámetros de calidad del aire y del suelo en la medida necesaria. Ubicada en el km 4.5 de la carretera Panamericana Sur con coordenadas geográficas 12°25’03.87”S y 76°45’18.39”W a una altitud de 424 m.s.n.m (ver Anexo I), este proyecto se ha decidido ejecutar en dicha zona en función a la cercanía a la carretera, la cual registra a un alto tránsito vehicular; sobre todo en épocas de verano, donde existe una mayor afluencia de usuarios que se dirigen a las playas del sur. Aquello contribuye con elevadas tasas de emisión de material particulado, monóxido de carbono, óxidos de nitrógeno, y compuestos orgánicos volátiles (COVs) perjudiciales para el bienestar humano y ambiental. Durante la duración del proyecto, se considerará la transición y los cambios estacionales, puesto que ante el pronosticado “fenómeno del niño global”, la variación de los patrones climáticos será significativa (Senamhi, 2023). Lo anterior producirá que las estaciones no se vean marcadas dado que alterará el periodo de verano de enero-marzo, meses en los que se ejecutará el proyecto. Estos cambios estacionales influyen directamente en factores como la dirección y velocidad del viento, deposición húmeda y variación en la temperatura, que están relacionados con la concentración de los contaminantes. En relación con los parámetros del suelo, también contribuye a alterar la presencia de humedad, salinidad y conductividad, por lo que se reitera la importancia de un seguimiento período de estas variables.
Dada la aspiración de la Universidad de convertir este campus en un centro de investigaciones multidisciplinarias, consideramos que la propuesta contribuirá significativamente a impulsar la implementación de tecnologías y la aplicación de ciencias, reiterando el enfoque de salud ambiental y bienestar social, impulsando el desarrollo de futuras investigaciones en busca de soluciones innovadoras.

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
Asociación Automotriz del Perú (2021). 2021: PERÚ CON LA PEOR CALIDAD DE AIRE ENTRE LOS PAÍSES DE LA REGIÓN. AAP Perú. Recuperado de https://aap.org.pe/iqair-calidad-de-aire-peru-mala-aap/#:~:text=De%20otro%20lado%2C%20si%20revisamos,de%20aire%20m%C3%A1s%20deficiente%20con
National Geographic (2020). Riesgo para los desiertos. Recuperado de  https://www.nationalgeographic.es/medio-ambiente/riesgos-para-los-desiertos
Organización Mundial de la Salud (2018). Nueve de cada diez personas en el mundo respiran aire contaminado. Recuperado  de    https://www.who.int/es/news/item/02-05-2018-9-out-of-10-people-worldwide-breathe-polluted-air-but-more-countries-are-taking-action
“Niño global comenzó en el mundo, pero aún no en Perú, ¿ Cuándo se sentirán los efectos ?” (2023). El Peruano. Recuperado de https://www.elperuano.pe/noticia/216933-nino-global-comenzo-en-el-mundo-pero-aun-no-en-peru-cuando-se-sentiran-sus-efectos
Servicio Nacional de Metereología e Hidrología del Perú. (2023). Fenómeno El Niño: Condiciones actuales de El Niño: Se mantiene el estado de alerta de El Niño Costero. Recuperado de https://www.senamhi.gob.pe/?p=fenomeno-el-nino

