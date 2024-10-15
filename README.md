# Proyecto de Análisis de Crédito

Este repositorio contiene el código y la documentación de un proyecto de análisis de crédito utilizando técnicas de aprendizaje automático. El objetivo es desarrollar un modelo que prediga la probabilidad de que un solicitante de crédito devuelva el préstamo, basándose en datos históricos de clientes.

## Procesos y Análisis:

1. **Lectura y Normalización de Datos:** Se carga un conjunto de datos de clientes con información sobre su historial crediticio. Se separa el conjunto de datos en características (variables predictivas) y etiquetas (variable de respuesta que indica si el crédito fue devuelto o no). Además, se realiza una división en conjuntos de entrenamiento y prueba para evaluar el rendimiento del modelo. Finalmente, se normalizan las características para mejorar el rendimiento de los algoritmos de aprendizaje automático.


2. **Construcción y Evaluación de Modelos:** Se implementan y evalúan diferentes modelos de clasificación para predecir la devolución de los créditos:

    - **K-Nearest Neighbors (KNN):** Se utiliza el algoritmo KNN con diferentes valores de k para determinar la exactitud del modelo en el conjunto de entrenamiento.

    - **Regresión Lineal:** Se ajusta un modelo de regresión lineal a los datos de entrenamiento para predecir la devolución del crédito. Se evalúa su exactitud en el conjunto de entrenamiento mediante la matriz de confusión.

    - **Regresión Logística:** Se entrena un modelo de regresión logística para predecir la probabilidad de devolución del crédito. Se analiza su exactitud en el conjunto de entrenamiento mediante la matriz de confusión.

    - **Árbol de Decisión:** Se construye un árbol de decisión para clasificar los clientes en función de su probabilidad de devolver el crédito. Se evalúa su exactitud en el conjunto de entrenamiento.

3. **Comparación de Rendimiento en el Conjunto de Prueba:** Se evalúa el rendimiento de los modelos en el conjunto de prueba utilizando métricas como la exactitud, el puntaje F1 y el coeficiente de Matthews. Esto permite comparar la calidad predictiva de los modelos y determinar cuál ofrece un mejor rendimiento.

4. **Análisis de Costos:** Se considera un escenario donde el coste de conceder un crédito a un cliente que no lo devuelve es cuatro veces mayor que el coste de no concederlo a un cliente que sí lo devolvería. Se analiza cuál de los modelos evaluados resulta más adecuado desde un punto de vista predictivo en este escenario, teniendo en cuenta la importancia de reducir los falsos negativos.

## Resultados:
Los resultados de la evaluación de los modelos se muestran en el código del proyecto, incluyendo las matrices de confusión, métricas y análisis de costes.

## Conclusiones:
El análisis de los resultados permite determinar cuál de los modelos evaluados ofrece el mejor rendimiento para la predicción de la devolución de créditos en diferentes escenarios. Se identifica el modelo más adecuado teniendo en cuenta la minimización de los costes asociados a las predicciones erróneas.
