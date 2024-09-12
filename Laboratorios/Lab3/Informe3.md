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
El presente informe tiene como objetivo evaluar la capacidad de inferencia del modelo para la identificación correcta de patrones implementando un modelo de TinyML en el microcontrolador Arduino Nano 33 BLE Sense para encender un LED rojo cuando se dibuje un circulo, un LED azul cuando se dibuje el número 3 y un LED verde cuando se dibuje el número 1. En consecuencia, este informe abordará la implementación del modelo, los resultados y las conclusiones obtenidas. 

<p align='center'>
  <img src="https://github.com/user-attachments/assets/94b2adda-3e01-4a65-8c1e-3c935c486853" alt="Descripción de la imagen" style="width: 450px; height: 250px;">
</p>

## Metodología

Este apartado abarcarrá la implementación del modelo en el Arduino Nano 33 BLE Sense mediante los siguientes pasos:

1- Obtención de datos:

El primer paso para entrenar el modelo de TinyML fue la recopilación de los datos de entrada, los cuales son necesarios para que el modelo pueda aprender a identificar los patrones específicos de movimiento: círculo, número 3 y número 1. Para esto, se utilizó el Arduino Nano 33 BLE Sense, que cuenta con sensores de movimiento integrados, como el acelerómetro y el giroscopio.

A través de la plataforma Edge Impulse, se creó un proyecto para capturar estos datos en tiempo real mientras el Arduino realizaba los movimientos correspondientes a cada patrón. Para ello se realizaron los pasos descritos a continuación: 

- Configuración de la plataforma: Se inició el proyecto en Edge Impulse y se conectó el Arduino Nano 33 BLE Sense utilizando el agente de datos de Edge Impulse, lo cual permitió transmitir los datos de los sensores directamente a la plataforma.

- Grabación de los movimientos: Para cada clase de patrón (círculo, número 3 y número 1), se realizaron múltiples grabaciones moviendo el Arduino en el aire para dibujar las formas. Se realizaron al menos 50 muestras por cada patrón con una duración promedio de 3 segundos por muestra para asegurar una cantidad suficiente de datos que permitiera una buena generalización del modelo.

- Ajuste de parámetros: Durante la captura de datos, se ajustaron parámetros como la frecuencia de muestreo a 100 Hz para capturar los cambios más sutiles en los movimientos del dispositivo. Este nivel de precisión fue necesario para asegurar que el modelo pudiera diferenciar entre los patrones, evitando confusiones entre formas similares.

- Segmentación de los datos: Los datos recolectados fueron etiquetados según el patrón correspondiente (círculo, número 3 y número 1).

<p align="center">
  <img src="https://github.com/user-attachments/assets/2effffd3-8027-4ef9-9113-a21f72204b6e" alt="Descripción de la imagen" style="width: 550px; height: 260px;">
</p>

2- Entrenamiento:

El modelo fue entrenado utilizando Edge Impulse, con datos recogidos del acelerómetro y giroscopio del Arduino Nano 33 BLE Sense. La arquitectura del modelo incluyó una capa de entrada con 117 características, dos capas densas (una con 20 neuronas y otra con 10 neuronas) y una capa de salida con 3 clases (círculo, número 3 y número 1). Se entrenó con 30 ciclos (epochs), una tasa de aprendizaje de 0.001 y un tamaño de lote de 32.
El entrenamiento, que duró unos pocos minutos, alcanzó una precisión del 90% y una perdida de 0.09.

![image](https://github.com/user-attachments/assets/144c4ef9-cde0-483d-95c6-b662bd79b990)

## Resultados

![Uploading image.png…]()


[Código](https://github.com/stephany-toribio/ProyectosDeIngenieria1/blob/main/Laboratorios/Lab3/Código.c)

[Modelo en Edge impulse](https://studio.edgeimpulse.com/public/515462/live)

## Conclusiones

  La inteligencia artificial es una de las herramientas mas potentes y utilizadas en la actualidad  debido a que permite a las computadoras o maquinas razonar y aprender tal cual persona humana[2]. El machine learning una rama de la IA, dependiente la configuración humana a través de la experiencia y los datos, nos permite "enseñar" a alguna maquina para así lograr mejoras en la toma de deciciones. Entrando al TinyML nos da la posibilidad de  desplegar modelos de machine learning en sistemas embedios, durante este laboratorio trabajamos esta tecnología junto con un Arduino Nano 33 BLE Sense, entendiendo la facilidad de creación del modelo de ML gracias a Edge impulse, si bien es cierto tuvimos complicaciones en el apartado de ejecutar el código en ArduinoIDE, a pesar de tener una buena base de datos, sin embargo obtuvimos aprendizajes de Tiny machine learning lo cual nos permitira desarrollar proyectos más escalables.

## Referencias

- [1]	Y. Abadade, A. Temouden, H. Bamoumen, N. Benamar, Y. Chtouki, y A. S. Hafid, “A Comprehensive Survey on TinyML”, IEEE Access, vol. 11, pp. 96892–96922, 2023.

- [2] Google Cloud, https://cloud.google.com/learn/what-is-artificial-intelligence?hl=es-419
