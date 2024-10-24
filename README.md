# Predicción de diabetes en pacientes
## Descripción

Este proyecto es un trabajo en equipo realizado por tres estudiantes de Ingeniería de Sistemas e Informática para la asignatura Introducción a la Inteligencia Artificial en la Universidad Nacional de Colombia. Se hace uso del dataset **prima-indians-diabetes**, el cual contiene datos de 768 pacientes diabéticos y no diabéticos.  Se implementaron árboles de decisión y redes bayesianas gausianas para evaluar su rendimiento y analizar el resultado de las métricas en ambos modelos. 

### Preprocesamiento y Exploración de Datos

- **Limpieza de Datos**: se realizó una imputación de datos utilizando SimpleImputer con la mediana para manejar valores faltantes.
- **Exploración de Datos**: análisis descriptivo de las variables para comprender la distribución y las características de los datos.

### Implementación de árboles de decisión

- Se hizo una comparación de las métricas Gini y Entropía para elegir aquella con mayor precisión y estabilidad a medida que se aumentara la profundidad del árbol.
- Las características con mayor impacto en la variable objetivo fueron elegidas implementando la técnica SelectKBest.
- Para determinar la profundidad máxima, el número de muestras por nodo y hoja se utilizó GridSearchCV.

En ambas implementaciones se obtuvieron matrices de confusión para entrenamiento y prueba, y de la misma manera se calcularon métricas de desempeño.

## Tecnologías y Librerías Utilizadas

- **Librerías de Python**:
  - `matplotlib` y `seaborn`: Para la visualización de datos y gráficos.
  - `numpy` y `pandas`: Para manipulación y análisis de datos.
  - `sklearn`: Para la implementación de de árboles de decisión y redes bayesianas gausianas.
