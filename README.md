# PRACTICA-2-REPO-1

## Descripción del proyecto

Este proyecto analiza los pasos de modelado, calibracion e incertidumbre del modelo LightGBM sin balanceado, tras elegirlo como modelo "ganador".
El trabajo parte de datos previamente procesados y divididos en distintos conjuntos para entrenamiento, validación, calibración y test.
---

# Objetivos

Los principales objetivos de la práctica son:

1. Optimizar modelos de Machine Learning mediante **Optuna**.
2. Comparar modelos **LightGBM** y **CatBoost**.
3. Evaluar métricas de calibración.
4. Aplicar técnicas de calibración probabilística.
5. Medir la incertidumbre de las predicciones.
6. Seleccionar el modelo final más robusto y fiable.

---
# Estructura del trabajo

El notebook se divide en tres bloques principales:

## 1. Optimización con Optuna
Se entrenan los siguientes modelos:
* LightGBM balanceado
* LightGBM sin balanceado
* CatBoost balanceado
* CatBoost sin balanceado
Evaluando para cada uno de ellos Log Loss, Brier Score, ROC AUC. 

## 2. Calibración de probabilidades

Se estudia si las probabilidades generadas por los modelos reflejan correctamente la probabilidad real de pertenecer a cada clase.
Para ello se utilizan las siguientes estrategias: 
* Reliability diagrams
* Brier decomposition
* Expected Calibration Error (ECE)
* Spiegelhalter Z-Test
* Log Loss

## 3. Medida de incertidumbre

Se implementan técnicas para detectar predicciones inciertas o poco fiables.
A traves de:
* Venn-Abers Calibration
* Evaluación de confianza probabilística
* Derivación de casos ambiguos a un agente externo


Uso académico y educativo.

