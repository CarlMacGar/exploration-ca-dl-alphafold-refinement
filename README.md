# Exploración del uso de autómatas celulares y técnicas de aprendizaje profundo para el refinamiento de regiones de baja confianza en modelos generados por AlphaFold.

### [🌐 English version / Versión en inglés ](README.en.md)

## Descripción

AlphaFold2 predice estructuras de proteínas con precisión atómica, pero genera una única conformación estática por proteína. Esto resulta insuficiente para representar el carácter heterogéneo y dinámico de las regiones intrínsecamente desordenadas (IDRs) y de regiones altamente flexibles como los bucles largos, cuya precisión disminuye de forma sistemática a medida que aumenta su longitud.

Este proyecto explora el diseño de un modelo híbrido que integra Autómatas Celulares (CA) y técnicas de Deep Learning (DL) para generar conjuntos conformacionales en regiones de baja confianza estructural (pLDDT < 70), buscando un equilibrio entre rigor estructural y eficiencia computacional frente a métodos tradicionales basados en Dinámica Molecular.

## Objetivos

### General

Diseñar un modelo basado en CA y técnicas de DL para el refinamiento de regiones con baja confiabilidad estructural (pLDDT bajo) en modelos de proteínas generados por AlphaFold.

### Específicos

1. Analizar las limitaciones actuales de AlphaFold en la predicción de regiones intrínsecamente desordenadas o con baja confianza estructural, mediante una revisión sistemática.
2. Diseñar un modelo conceptual que integre CA y DL para el refinamiento de dichas regiones.
3. Desarrollar una herramienta experimental que implemente el modelo, entrenada con pares de estructuras AlphaFold–nativas.
4. Evaluar la efectividad del enfoque mediante métricas estructurales y de confianza, comparando contra los modelos originales de AlphaFold.

## Tecnologías
* ***Lenguaje***: Python ≥ 3.14
* ***DL***: PyTorch ≥ 2.10
* ***Bioinformática***: BioPython ≥ 1.86, formato PDB
* ***Análisis de datos***: NumPy ≥ 2.4, Pandas ≥ 3.0, SciPy
* ***Evaluación estructural***: TM-align / TM-score, pLDDT
* ***Visualización***: Seaborn, PyMOL
* ***Entornos***: Jupyter Notebook, Google Colab (GPU)