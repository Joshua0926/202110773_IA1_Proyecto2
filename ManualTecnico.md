# Manual Técnico

## 1. Propósito del Proyecto

Desarrollar un sitio web interactivo utilizando HTML y JavaScript, orientado a la práctica de conceptos de Machine Learning. El sitio permitirá a los usuarios cargar archivos CSV, elegir modelos de Machine Learning y ajustar sus parámetros para entrenar y realizar predicciones, utilizando la biblioteca `tytus.js`. La aplicación se publicará en GitHub Pages para su acceso en línea.

## 2. Requisitos

- **Lenguajes y tecnologías**: JavaScript, HTML, CSS (opcional para estilos).
- **Bibliotecas**: Uso obligatorio de `tytus.js` para los modelos de Machine Learning y visualización, además de cualquier biblioteca JavaScript sin frameworks ni entornos adicionales.
- **Entorno**: El código se ubicará en un repositorio público en GitHub y se desplegará en GitHub Pages.

## 3. Estructura del Proyecto

- **index.html**: Define la estructura del sitio web.
- **styles.css**: Opcional, para estilizar la página y ofrecer una interfaz amigable y simple.
- **script.js**: Controla la lógica del sitio, incluyendo la carga de archivos, la selección de algoritmos, la configuración de parámetros, el entrenamiento, la predicción y la visualización de resultados.
- **tytus.js**: Biblioteca principal para los modelos de Machine Learning, almacenada en la carpeta `lib/` o enlazada directamente desde el repositorio de `tytus.js`.

## 4. Componentes del Sitio

- **Cargador de archivos CSV**: Permite a los usuarios cargar datasets, procesándolos para extraer columnas y filas e identificar variables.
  
- **Selector de modelos de Machine Learning**: Un menú desplegable con modelos disponibles en `tytus.js`, como regresión, clasificación, clustering, entre otros. Este menú se conecta con la biblioteca para instanciar el modelo seleccionado.

### Parámetros Configurables

- **Porcentaje de Train/Test**: Slider o campo de entrada para ajustar la proporción de datos de entrenamiento y prueba.
- **Objetivo de Entrenamiento**: Opciones de selección como checkbox o radio buttons para elegir entre predicción, clasificación, tendencia, etc.
- **Parámetros específicos**: Ajustes adicionales dependiendo del modelo (ej. número de clases para clasificación).
- **Entrada de rango (predicción)**: Campo de entrada para definir el rango de valores en el eje X si el modelo permite predicción.
- **Variables de entrada y salida (supervisado)**: Permite seleccionar las variables de salida y de entrada desde el dataset.

### Botones de Acción

- **Entrenar**: Inicia el proceso de entrenamiento con los parámetros seleccionados.
- **Predecir**: Realiza predicciones basadas en el modelo entrenado.
- **Mostrar Gráficas**: Genera una visualización de los resultados, utilizando gráficos adecuados según el tipo de modelo (ej. dispersión para regresión, barras para clasificación).

## 5. Implementación de Funcionalidades

- **Carga de Datos**: Emplear el API de `FileReader` de JavaScript para procesar el archivo CSV y extraer datos para el entrenamiento.
- **Instanciación de Modelos**: Utilizar `tytus.js` para cargar y ejecutar modelos de Machine Learning.

  ```javascript
  const modelo = new Tytus.Modelo('nombreModelo');
  modelo.train(data, options);

Entrenamiento y Predicción: Lógica para enviar datos a los métodos de entrenamiento y predicción, incluyendo configuración de porcentajes de train/test y manejo de errores o advertencias para configuraciones incorrectas.

Visualización de Resultados: Usar gráficos básicos con canvas o bibliotecas JavaScript como Chart.js. La visualización variará según el tipo de modelo, mostrando gráficos de dispersión, de barras, etc.

6. Consideraciones Adicionales
Validaciones: Verificar que el archivo cargado sea un CSV y que se hayan completado todos los parámetros requeridos antes de iniciar el entrenamiento.
Compatibilidad y Rendimiento: Optimizar el uso de tytus.js y asegurar compatibilidad en navegadores modernos.
Estilo y UX: Opcionalmente, añadir estilos en styles.css para lograr una interfaz limpia y moderna.
7. Despliegue en GitHub Pages
Asegurarse de que el repositorio esté configurado como público.
Publicar el sitio en GitHub Pages activando la opción en Settings y seleccionando la rama adecuada (usualmente main o docs).
Verificar el enlace de GitHub Pages para confirmar que el sitio esté funcionando correctamente.
8. Pruebas y Validación
Realizar pruebas de carga con diversos archivos CSV y configuraciones de modelos, validando que cada parámetro configurable funcione correctamente. Probar que cada botón de acción cumpla con su función esperada y muestre los resultados adecuados.