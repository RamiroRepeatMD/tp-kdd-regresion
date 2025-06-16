# Proceso KDD – Trabajo Práctico de Regresión

Este repositorio contiene el desarrollo completo de un trabajo práctico grupal que aplica el proceso de descubrimiento de conocimiento en bases de datos (KDD) para resolver un problema de regresión utilizando un dataset público de viviendas en California.

## Objetivo

Predecir el valor medio de una propiedad (`median_house_value`) a partir de atributos socioeconómicos y geográficos como ingreso medio, cantidad de habitaciones y ubicación.

## Metodología

Se aplicó el proceso KDD en sus diferentes fases:

1. Selección del dataset:  
   Dataset público `housing.csv` de California.

2. Limpieza de datos:  
   - Imputación de valores faltantes utilizando la media.
   - Revisión de tipos y formato.

3. Selección de atributos:  
   - Análisis de correlación.
   - Selección manual de variables relevantes para el modelo.

4. Transformación:  
   - Escalado de atributos numéricos con `StandardScaler`.
   - División del dataset en entrenamiento y prueba (80/20).

5. Minería de datos:  
   - Modelos utilizados:
     - Regresión Lineal
     - Random Forest Regressor

6. Evaluación:
   - Métricas: R² (coeficiente de determinación), MAE y RMSE.
   - Mejor desempeño obtenido con Random Forest (R² = 0.811).

## Archivos incluidos

- `notebook.ipynb`: desarrollo completo del análisis.
- `housing.csv`: dataset utilizado.
- `requirements.txt`: dependencias necesarias para reproducir el entorno.
- `.gitignore`: exclusión de carpetas como el entorno virtual y archivos temporales.

## Instrucciones para ejecutar

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/<TU_USUARIO>/<TU_REPO>.git
   cd <TU_REPO>
## Crear entorno virtual

python3 -m venv venv (en macos)
python -m venv venv (en windows)
source venv/bin/activate
pip install -r requirements.txt
