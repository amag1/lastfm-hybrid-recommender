# lastfm-hybrid-recommender
Sistema de recomendación utilizando tanto Colaborative Filtering como Content-Based Recommendations para el dataset de [LastFM](https://grouplens.org/datasets/hetrec-2011/)


## Descripción
sistema de recomendación híbrido que combina técnicas de filtrado colaborativo y modelos basados en contenido, utilizando datos reales de la red social Last.fm. A través de este enfoque, se busca generar recomendaciones de artistas musicales basadas en ratings implícitos, afrontando los problemas que suelen surgir en sistemas de este tipo

## Dataset
El dataset utilizado es el de [LastFM](https://grouplens.org/datasets/hetrec-2011/), que contiene información sobre usuarios, artistas y sus interacciones. En el directorio dataset pueden encontrarse los archios `.dat` originales, un readme con información adicional y una directorio `remapped` con los mismos datos pero realizando un mapeo de ids para facilitar su uso.

## Estructura
En la raíz del proyecto se encuentran los siguientes notebooks:
   - `eda.ipynb`: Análisis exploratorio de los datos
   - `baseline.ipynb`: Modelo baseline para comparar con el sistema híbrido
   - `main.ipynb`: Implementación del sistema basado en LightFM y exploración de hipermarámetros
   - `coldstart.ipynb`: Implementación de un sistema de recomendación para artistas nuevos usando los embeddings de los artistas

En el directorio `notebooks` se pueden hallar otros notebooks experimentales con pruebas que sirven como base para el desarrollo del sistema híbrido.

Además, se incluye el informe final del proyecto en formato `.pdf` en el directorio `docs`. En él se detallan los pasos seguidos para la implementación del sistema híbrido, los resultados obtenidos y las conclusiones del trabajo.