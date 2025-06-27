# Proyecto del curso Introducción al Machine Learning UdeA
[![Machine Learning](https://img.shields.io/badge/Asignatura-Modelos%20y%20simulación%20de%20sistemas%20II-red)](https://jdariasl.github.io/Intro_ML_2025/intro.html)
[![Semestre](https://img.shields.io/badge/Semestre-2025%201-blue)]()
[![Universidad](https://img.shields.io/badge/Universidad-UdeA-green)]()
[![Carrera](https://img.shields.io/badge/Carrera-Ingeniería%20de%20sistemas-orange)]()


> [!WARNING]  
> Antes de ejecutar la **primera celda del notebook 01** (Ya sea de la carpeta de regresión o clasificación) debe tener cargado en el entorno de trabajo su token de Kaggle, en el archivo 'kaggle.json'. Esto es debido a que el dataset con el que se trabaja está en dicha plataforma. Recuerde cambiar la ruta de su token si es necesario.

> [!TIP]
> Los notebook 01 al final exportan los datos preprocesados a un archivo llamado 'data.csv' para el enfoque de regresión y 'data_class.csv' para el enfoque de clasificación. Recuerda descargarlos y subirlos al entorno de los notebooks 02, 03, 04, 05, 06, 07 y 09 antes de ejecutarlos. Para ejecutar el notebook 08 recuerda cargar el archivo 'data_sfs.csv' el cual es exportado en el notebook 07. 

## Estructura del proyecto
El trabajo se divide en 2 carpetas:
- Regresión
- Clasificación (Enfoque principal)

En cada carpeta hay un enfoque diferente para el proyecto. En el enfoque de "Regresión" se trabaja el proyecto tratando de predecir la variable **'TimeInShelterDays'**, la cual es numérica discreta. En el enfoque de "Clasificación" se trabaja el proyecto tratando de predecir la variable **'AdoptionLikelihood'**. Por lo que se dan resultados diferentes. Se logra obtener un nivel de generalización diferente para cada modelo. 

### Estructura general de los enfoques
Cada carpeta contiene 9 notebooks de colab. 
1. **Exploración y preprocesado de los datos**: En este notebook se realiza una exploración, se muestran algunas gráficas que permiten observar las distribuciones de las variables, la matriz de correlación y se escalan los datos numéricos. También para los datos categóricos se realiza una codificación OneHot.
2. **Notebooks donde se entrenan los modelos**: En Notebooks desde el 01 hasta el 06 se entrenan los modelos Regresión lineal o logística, según sea el enfoque, un KNN, un Random Forest, un MLP y un SVM.
3. **Notebook de selección de características**: En el notebook 07 se realiza la selección de características con un SFS.
4. **Notebook de prueba de SFS**: En el notebook 08 se realiza nuevamente el entrenamiento de los 2 modelos con mejores métricas, con los datos que salen del notebook 07 y se sacan las métricas.
5. **Notebook de extracción de características**: En el notebook 09 se realiza PCA a los datos que salen del notebook 01 y nuevamente la prueba con los datos resultantes de los datos obtenidos aplicando PCA.   
