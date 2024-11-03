# Guía del Usuario

Este sitio permite cargar archivos CSV, seleccionar modelos de Machine Learning, ajustar configuraciones y realizar predicciones. A continuación, se detalla cómo utilizar cada función para sacar el máximo provecho de la aplicación.

## 1. Vista Principal

Al ingresar, encontrarás una interfaz sencilla dividida en varias secciones:
- Cargar Dataset (Archivo CSV)
- Selección de Modelo
- Configuración de Parámetros
- Botones de Ejecución
- Visualización de Gráficos

## 2. Subir Archivo CSV

1. **Cargar archivo**: Haz clic en el botón para seleccionar un archivo CSV con los datos que deseas analizar.
2. **Verificación**: Asegúrate de que el archivo tenga una estructura válida y datos bien organizados.

## 3. Elegir un Modelo de Machine Learning

Usa el menú desplegable para escoger el modelo de Machine Learning que deseas aplicar. Las opciones pueden incluir:
- **Regresión**: Para identificar relaciones entre variables.
- **Clasificación**: Para categorizar datos en grupos específicos.
- **Clustering**: Para agrupar datos según sus similitudes.

## 4. Configurar Parámetros del Modelo

Tras seleccionar un modelo, ajusta los parámetros relevantes.

### Porcentaje de Train/Test

- Define el porcentaje de datos para entrenamiento y prueba utilizando el slider o un campo de entrada.
- Ejemplo: 70% para entrenamiento y 30% para prueba.

### Objetivo del Análisis

- Selecciona el propósito de tu análisis: predicción, clasificación, identificación de patrones, entre otros.

### Configuración de Parámetros Específicos

Dependiendo del modelo, deberás ajustar algunos parámetros adicionales:
- **Predicción**: Introduce el rango de valores en el eje X para la predicción.
- **Clasificación**: Indica el número de clases para el modelo.
- **Aprendizaje Supervisado**: Elige las columnas de entrada y salida.

## 5. Botones de Ejecución

### Entrenar

- Haz clic en "Entrenar" para procesar los datos y entrenar el modelo con los parámetros seleccionados.
- La aplicación te indicará si el entrenamiento fue exitoso o si hubo errores.

### Predecir

- Una vez entrenado el modelo, haz clic en "Predecir" para generar predicciones.
- Para modelos de predicción, define el rango de valores en el eje X, si es necesario.

### Mostrar Gráficas

- Pulsa "Mostrar Gráficas" para visualizar los resultados.
- Según el modelo, los gráficos pueden incluir diagramas de dispersión, barras o líneas.

## 6. Visualización de Resultados

### Gráficos

- Las visualizaciones aparecerán en la sección correspondiente, permitiéndote analizar los resultados del modelo.
- Ejemplo: En una regresión, se mostrará cómo los puntos se ajustan a una línea de tendencia.

### Interpretación

- Utiliza los gráficos para comprender los patrones, clasificaciones o predicciones generadas por el modelo.

## 7. Consejos y Recomendaciones

- **Estructura del CSV**: Asegúrate de que el archivo esté bien estructurado, con cada columna claramente encabezada.
- **Configuración Adecuada**: Revisa que los parámetros sean adecuados para el modelo seleccionado.
- **Experimenta**: Prueba con diferentes modelos y configuraciones para lograr un análisis óptimo.

## 8. Resolución de Problemas

- **Error al Cargar el Archivo**: Verifica el formato y estructura del archivo, que debe ser CSV.
- **Error en Entrenamiento o Predicción**: Asegúrate de que las configuraciones estén completas y que los datos del CSV sean compatibles con el modelo.
- **Problemas de Visualización**: Si las gráficas no aparecen, intenta recargar la página y volver a cargar el archivo y el modelo.
