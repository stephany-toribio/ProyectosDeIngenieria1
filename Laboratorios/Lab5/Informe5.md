<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">Informe V</h1>
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

<p align="left">
  <h1 align="center">Simulación de esfuerzo mecánico</h1>
</p>

## 1. Introducción
La creación de los soportes en 3D es fundamental para la protección de componentes electrónicos, debido a que durante el desarrollo de estas estructuras se incorporaron elementos esenciales, como chaflanes para optimizar la resistencia y reducir las tensiones concentradas en las partes críticas [1]. Es así como se presenta el uso del software de simulación SimScale como una herramienta para analizar las estructuras y detectar los posibles errores que podria presentar la impresión 3D, analizando la tensión y deformación del material y proporcionando una mejor selección de materiales para mejorar la seguridad. De esa forma, se evalúa el comportamiento de las estructuras bajo condiciones de carga y se reduce costos al evitar posibles fallos [2].

Por lo anteriormente mencionado, el propósito de este informe es desarrollar una simulación de esfuerzos estáticos en un componente mecánico del proyecto a desarrollar en el curso, permitiendo analizar el comportamiento del componente bajo ciertas condiciones de carga.

## 2. Metodología 

### 2.1. Descripción del Componente
El componente seleccionado para la simulación es una **Soporte Metálico**, el cual será sometido a diferentes tipos de esfuerzos mecánicos, incluyendo torsión, tracción y flexión. Este componente esta  modelado con las siguientes características clave que afectan su resistencia:

- **Dimensiones**: 1793mm x 476.408mm x 90mm

<p align="center"><strong>Figura 1: Soporte Métalico en Onshape</strong></p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/dc929bb6-7f32-481c-bc64-cbf00eb65527" width="320" height="380">
</p>

<p align="center" class="note text-center note-white">FUENTE: Figura 1. Elaboración Propia</p>

### 2.2. Configuración de la Simulación
La simulación fue realizada en **SimScale**, empleando los siguientes pasos de configuración:

### Creación del Proyecto
- Se creó un proyecto bajo el nombre **"Proyectos_de_ingenieria_1"**.
- Se seleccionaron las unidades de medida en metros.

### Importación de Geometría
- Se importó la geometría del componente desde **OnShape**, asegurando que las piezas se visualizaran correctamente.

<p align="center"><strong>Figura 2: Importación del componente desde Onshape</strong></p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8e35b7e0-61da-4fe1-812e-1a888b67f292" width="380" height= "450">
</p>

<p align="center" class="note text-center note-white">FUENTE: Figura 2. Elaboración Propia</p>

### Configuración de Contactos
- Se definieron los contactos entre las piezas como **"bonded"** (soldados), ya que no se preveían movimientos entre las diferentes partes del soporte.

### Asignación de Materiales
- Se asignó **Iron** como el material del componente, debido a sus propiedades de alta resistencia en el ambiente determinado.
  
- Las propiedades del material fueron configuradas de acuerdo a los estándares del software.

<p align="center"><strong>Figura 3: Asignación del material</strong></p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/979b1fbc-ae18-47bf-809b-4c0e21cfc4ba" width="300">
</p>

<p align="center" class="note text-center note-white">FUENTE: Figura 3. Elaboración Propia</p>

### Condiciones de Soporte y Carga
- Las caras inferiores de la carcasa fueron fijadas para simular su anclaje a una base sólida.
- Se aplicó una carga de **-1000 N** en el eje Z, simulando la presión de un componente que descansa sobre la carcasa.

### Ejecución de la Simulación
- La simulación se ejecutó en varios pasos incrementales para obtener una mayor precisión en los resultados.
  
<p align="center"><strong>Figura 4: Simulación</strong></p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/87e12ded-0c2c-4cbf-b516-fc8fef239f94" width="400">
</p>

<p align="center" class="note text-center note-white">FUENTE: Figura 4. Elaboración Propia</p>

## 3. Resultados

La simulación en SimScale del componente metálico reveló aspectos sobre su comportamiento bajo diversas condiciones. En primer lugar, se analizó la distribución de tensiones y la deformación resultante para determinar cómo responde el material a la carga aplicada. Esto permitió evaluar su resistencia estructural y determinar posibles áreas de refuerzo. Además, se estudió la resistencia del componente para predecir el ciclo de vida y posibles fallos por desgaste. Estos resultados son fundamentales para validar la viabilidad del diseño, optimizar el material utilizado y reducir riesgos de fallos futuros.
Los resultados de la simulación revelaron los siguientes puntos clave:

<p align="center"><strong>Figura 5: Resultados de la Simulación</strong></p>
<div align="center">
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/8faa6f9a-279e-4f6b-ab26-acbea55c238d" width="330" height="330" style="margin: auto;"></td>
    <td><img src="https://github.com/user-attachments/assets/e777a577-4970-47bb-a913-7c0e905b72e9" width="330" height="330" style="margin: auto;"></td>
  </tr>
</table>
</div>

<p align="center" class="note text-center note-white">FUENTE: Figura 5. Elaboración Propia</p>

## 4. Referencias Bibliográficas
- [1] I. A. Domínguez, L. Romero, M. M. Espinosa, y M. Domínguez, "Impresión 3D de maquetas y prototipos en arquitectura y construcción," Revista de la construcción, vol. 12, no. 2, pp. 39-53, 2013.
  
- [2] V. Pachacama, A. Jorque, C. Ulcuango, y R. Passo, "El software de simulación como herramienta para el análisis de estructuras metálicas automotrices," CONECTIVIDAD, vol. 5, no. 3, pp. 44-61, 2024.