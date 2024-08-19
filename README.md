# Implementación de Regresión Lineal usando el Conjunto de Datos "articulos_ml.csv"

Este proyecto implementa un modelo de regresión lineal para predecir el número de acciones compartidas (`# Shares`) de artículos basándose en la cantidad de imágenes y videos (`# Images video`) y el número de comentarios (`# of comments`). Utilizamos el conjunto de datos "articulos_ml.csv" que contiene información sobre diferentes artículos relacionados con inteligencia artificial y aprendizaje automático.

## Contenido

- [Justificación del Algoritmo](#justificación-del-algoritmo)
- [Descripción del Diseño del Modelo](#descripción-del-diseño-del-modelo)
- [Evaluación y Optimización del Modelo](#evaluación-y-optimización-del-modelo)
- [Enlace al Repositorio](#enlace-al-repositorio)

## Justificación del Algoritmo

Se eligió el algoritmo de **Regresión Lineal** debido a su simplicidad y efectividad en problemas donde se desea predecir una variable continua en función de una o más variables independientes. Dado que el objetivo es predecir un valor numérico (número de acciones compartidas), la regresión lineal es una opción adecuada.

## Descripción del Diseño del Modelo

1. **Carga y Preprocesamiento de Datos**:
   - Se cargaron los datos desde el archivo `articulos_ml.csv`.
   - Se exploraron los datos para identificar las variables más relevantes para la predicción (`# Images video`, `# of comments`).

2. **Separación de Variables**:
   - Variables independientes: `# Images video`, `# of comments`.
   - Variable dependiente: `# Shares`.

3. **División de Datos**:
   - Se dividieron los datos en conjuntos de entrenamiento y prueba en una proporción de 80/20.

4. **Entrenamiento del Modelo**:
   - Se utilizó el algoritmo de Regresión Lineal para entrenar el modelo con los datos de entrenamiento.

5. **Optimización del Modelo**:
   - Se realizó una búsqueda de hiperparámetros usando `GridSearchCV` para optimizar el modelo.
   - Se entrenó un nuevo modelo con los mejores hiperparámetros encontrados.

## Evaluación y Optimización del Modelo

- **Evaluación Inicial**:
   - Se evaluó el modelo utilizando el coeficiente de determinación \( R^2 \) y el error cuadrático medio (MSE).
   - Se visualizó la comparación entre los valores reales y las predicciones.

- **Optimización**:
   - Se utilizaron técnicas de validación cruzada repetida (`RepeatedKFold`) para mejorar la robustez del modelo.
   - Se optimizó el modelo utilizando `GridSearchCV` para encontrar los mejores hiperparámetros y se volvió a entrenar el modelo con estos.

## Enlace al Repositorio

Puedes encontrar el código fuente completo y el modelo entrenado en el siguiente [repositorio de GitHub](https://github.com/carlop13/regresion-lineal-articulos-ml).

---

## Requisitos

- Python 3.8+
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Ejecución

1. Clona este repositorio:

   ```bash
   git clone https://github.com/carlop13/regresion-lineal-articulos-ml.git
   cd regresion-lineal-articulos-ml
