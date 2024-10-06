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
El propósito de este informe es desarrollar una simulación de esfuerzos estáticos en un componente mecánico de nuestro proyecto a desarrollar ene le curso, en el contexto de los proyectos de ingeniería expuestos en la guía de diseño y ensayo de modelos 3D para piezas impresas o diseñadas para nuestro proyecto. Esta simulación tiene como objetivo analizar el comportamiento del componente bajo ciertas condiciones de carga.

## 2. Descripción del Componente
El componente seleccionado para la simulación es una **Insertar nombre dle objeto** de soporte para un componente electrónico, que será sometido a diferentes tipos de esfuerzos mecánicos, incluyendo torsión, tracción y flexión. La carcasa está modelada con las siguientes características clave que afectan su resistencia:
- **Material**: 
- **Geometría**: 
- **Dimensiones**:

## 3. Configuración de la Simulación
La simulación fue realizada en **SimScale**, empleando los siguientes pasos de configuración:

### 3.1 Creación del Proyecto
- Se creó un proyecto bajo el nombre **"Proyectos_de_ingenieria_1"**.
- Se seleccionaron las unidades de medida en metros.

### 3.2 Importación de Geometría
- Se importó la geometría del componente desde **OnShape**, asegurando que las piezas se visualizaran correctamente.
<p align="center">
  <img src="https://github.com/user-attachments/assets/8e35b7e0-61da-4fe1-812e-1a888b67f292" width="200">
</p>


### 3.3 Configuración de Contactos
- Se definieron los contactos entre las piezas como **"bonded"** (soldados), ya que no se preveían movimientos entre las diferentes partes del soporte.

### 3.4 Asignación de Materiales
- Se asignó *Iron** como el material del componente, debido a sus propiedades de alta resistencia en el ambiente determinado.
- Las propiedades del material fueron configuradas de acuerdo a los estándares del software.

<p align="center">
  <img src="https://github.com/user-attachments/assets/979b1fbc-ae18-47bf-809b-4c0e21cfc4ba" width="300">
</p>


### 3.5 Condiciones de Soporte y Carga
- Las caras inferiores de la carcasa fueron fijadas para simular su anclaje a una base sólida.
- Se aplicó una carga de **-1000 N** en el eje Z, simulando la presión de un componente que descansa sobre la carcasa.


### 3.6 Ejecución de la Simulación
- La simulación se ejecutó en varios pasos incrementales para obtener una mayor precisión en los resultados.
<p align="center">
  <img src="https://github.com/user-attachments/assets/87e12ded-0c2c-4cbf-b516-fc8fef239f94" width="600">
</p>


## 4. Resultados de la Simulación
Los resultados de la simulación revelaron los siguientes puntos clave:

<p align="center">
  <img src="https://github.com/user-attachments/assets/8faa6f9a-279e-4f6b-ab26-acbea55c238d" width="400" height="400">
  <img src="https://github.com/user-attachments/assets/e777a577-4970-47bb-a913-7c0e905b72e9" width="400" height="400">
</p>




