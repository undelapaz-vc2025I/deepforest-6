# Análisis de Imágenes Aéreas con DeepForest

Este proyecto consiste en aplicar un modelo preentrenado de DeepForest para detectar árboles en imágenes aéreas y realizar un análisis cuantitativo a partir de los resultados obtenidos. Todo el trabajo se desarrolla en el notebook `analisis_arboles.ipynb`.

## Objetivo General

Detectar árboles en una imagen aérea mediante un modelo de deep learning (DeepForest) y analizar sus características utilizando técnicas de visión por computador y análisis de datos.

## Requisitos

- Python 3.7+
- DeepForest (instalación detallada en: https://deepforest.readthedocs.io/en/v1.5.0/getting_started/install.html)
- Librerías adicionales listadas en `requirements.txt`

## Desarrollo de la Actividad

A continuación se describe cada una de las tareas realizadas en el notebook:

### 1. Carga de la imagen y predicción

- Se carga una imagen aérea en formato RGB.
- Se utiliza el modelo preentrenado de DeepForest para detectar árboles.
- Como salida se obtiene una lista de bounding boxes con coordenadas y confianza de detección.

### 2. Visualización con identificadores únicos

- Se asigna un identificador único a cada árbol detectado.
- Se visualiza la imagen original con las cajas delimitadoras (bounding boxes) y los identificadores sobrepuestos.

### 3. Cálculo de áreas de los árboles detectados

- Se calcula el área de cada caja detectada en píxeles mediante la fórmula:
