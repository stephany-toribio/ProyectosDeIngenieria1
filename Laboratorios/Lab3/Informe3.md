<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">Informe III</h1>
</p>
 
<strong>Docentes:</strong>
- Mg. Umbert Lewis De La Cruz Rodriguez 
- Mg. Marcos Retamozo Ramos
- Mg. Moises Stevend Meza Rodriguez
- Mg. Carol Ordoñez Aquino
- Dr. Harry Anderson Rivera Tito  
- Dr. Pierre Ramos Apestegui 
- Ing. Renzo José Chan Ríos

<strong>Integrantes:</strong>
- Gavidia Crovetto, Bruno Paolo
- Silva Cuzqui, Camilo Sebastián
- Cueva Ramos, José Nilson
- Toribio Alvarado, Stephany Marilyn
- Herrera Valeriano, Jhunior Fernando 

## Introducción

La Inteligencia Artificial (IA), en los ultimos años se ha convertido en uno de los pilares de la transformación digital aportando soluciones innovadoras a diversos campos de investigación. A pesar de ello, la IA no se presenta como una solución inmediata a los problemas que se busca resolver, debido al alto costo de computación que requiere. Es así como surge TinyML, una alternativa que permite realizar tecnología sin la preocupación de los recursos computacionales [1].  
El presente informe tiene como objetivo evaluar la capacidad de inferencia del modelo para la identificación correcta de patrones implementando un modelo de TinyML en el microcontrolador Arduino Nano 33 BLE Sense para encender un LED rojo cuando se dibuje un circulo, un LED azul cuando se dibuje el número 3 y un LED verde cuando se dibuje el número 1. En consecuencia, este informe abordará la implementación del modelo, los resultados y las conclusiones conclusiones obtenidas. 

## Metodología

Este apartado abarcarrá la implementación del modelo en el Arduino Nano 33 BLE Sense mediante los siguientes pasos:

1- Obtención de datos:

El primer paso para entrenar el modelo de TinyML fue la recopilación de los datos de entrada, necesarios para que el modelo pudiera aprender a identificar los patrones específicos de movimiento: círculo, número 3 y número 1. Para esto, se utilizó el Arduino Nano 33 BLE Sense, que cuenta con sensores de movimiento integrados, como el acelerómetro y el giroscopio.

A través de la plataforma Edge Impulse, se creó un proyecto para capturar estos datos en tiempo real mientras el Arduino realizaba los movimientos correspondientes a cada patrón. 
Se siguieron los siguientes pasos.

- Configuración de la plataforma: Se inició el proyecto en Edge Impulse y se conectó el Arduino Nano 33 BLE Sense utilizando el agente de datos de Edge Impulse, lo cual permitió transmitir los datos de los sensores directamente a la plataforma.

- Grabación de los movimientos: Para cada clase de patrón (círculo, número 3 y número 1), se realizaron múltiples grabaciones moviendo el Arduino en el aire para dibujar las formas. Se realizaron al menos 50 muestras por cada patrón, con una duración promedio de 3 segundos por muestra, para asegurar una cantidad suficiente de datos que permitiera una buena generalización del modelo.

- Ajuste de parámetros: Durante la captura de datos, se ajustaron parámetros como la frecuencia de muestreo a 100 Hz para capturar los cambios más sutiles en los movimientos del dispositivo. Este nivel de precisión fue necesario para asegurar que el modelo pudiera diferenciar entre los patrones, evitando confusiones entre formas similares.

**2- Entrenamiento:** 

## Resultados

## Referencias

- [1]	Y. Abadade, A. Temouden, H. Bamoumen, N. Benamar, Y. Chtouki, y A. S. Hafid, “A Comprehensive Survey on TinyML”, IEEE Access, vol. 11, pp. 96892–96922, 2023.

- [2]	R. Sanchez-Iborra y A. F. Skarmeta, “TinyML-enabled frugal smart objects: Challenges and opportunities”, IEEE Circuits Syst. Mag., vol. 20, núm. 3, pp. 4–18, thirdquarter 2020.
