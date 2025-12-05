# Construcción automatizada de modelos 3D de árboles, a partir de datos LiDAR  🌳

Este repositorio presenta una implementación completa de un flujo de trabajo automatizado para la construcción de modelos 3D de árboles a partir de datos LiDAR. El objetivo es generar representaciones geométricas del arbolado urbano en distintos Niveles de Detalle (LOD), mediante un proceso reproducible que integra clasificación, segmentación, depuración y modelado.

## 📁 Conjunto de datos

Para el desarrollo de este proyecto se emplean datos LiDAR provenientes del Actueel Hoogtebestand Nederland (AHN3), disponibles públicamente en los Países Bajos. La nube de puntos AHN3 incluye una clasificación básica distribuida en cinco clases principales:
- Sin clasificar
- Terreno (suelo)
- Edificaciones
- Agua
- Estructuras civiles

## 💻 Notebook

Se incluye un notebook Jupyter con el código fuente completo del proyecto, el cual permite reproducir el proceso completo de construcción automatizada de modelos 3D de árboles paso a paso.

## 📝 Documentos

Se incluye un reporte en formato de artículo que describe detalladamente la implementación, el procesamiento y la generación de modelos 3D de árboles a partir de datos LiDAR, incluyendo las etapas de clasificación, segmentación, depuración y construcción de los diferentes Niveles de Detalle (LOD).

## 🗺️ Resultados 

Se incluyen cuatro archivos .cityjson que corresponden a los modelos 3D generados para cada Nivel de Detalle (LOD):

LOD0 – Representación básica en planta

LOD1 – Volúmenes extruidos

LOD2 – Modelos paramétricos con copa y tronco diferenciados

LOD3 – Modelos ajustados directamente a la nube de puntos

Cada archivo refleja el resultado del modelamiento automatizado a partir de los datos LiDAR procesados en este proyecto.

Para la visualización interactiva de los archivos generados en formato .cityjson, se utilizó la plataforma web CityJSON Ninja, disponible en:

🔗 https://ninja.cityjson.org/

Además, se anexa un video que muestra el proceso de carga y visualización de cada archivo .cityjson, permitiendo observar de manera comparativa cómo se representan los árboles en cada Nivel de Detalle (LOD).

## 🗃️ Salidas_procesamiento

Esta carpeta contiene los productos intermedios generados durante las etapas de clasificación, segmentación, limpieza y extracción de parámetros morfométricos a partir de la nube de puntos LiDAR. Cada archivo corresponde a un paso específico dentro del flujo de trabajo que culmina con la creación de los modelos 3D en CityJSON.

## 🙌 Créditos

Este trabajo es una implementación de de la línea base presentada en [\"Automatic construction of 3D tree models in
multiple levels of detail from airborne LiDAR data\"](https://repository.tudelft.nl/record/uuid:3e169fc7-5336-4742-ab9b-18c158637cfe), Geert Jan (Rob) de Groot, TU Delft - Architecture and the Built Environment, Master Thesis (2020).

Repositorio Github: [\"TreeConstruction\"](https://github.com/RobbieG91/TreeConstruction/tree/master)


