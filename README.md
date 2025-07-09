# Proyecto de Machine Learning para la predicción de la adopción de mascotas en refugios
[![Machine Learning](https://img.shields.io/badge/Asignatura-Modelos%20y%20simulación%20de%20sistemas%20II-red)](https://jdariasl.github.io/Intro_ML_2025/intro.html)
[![Semestre](https://img.shields.io/badge/Semestre-2025%201-blue)]()
[![Universidad](https://img.shields.io/badge/Universidad-UdeA-green)]()
[![Carrera](https://img.shields.io/badge/Carrera-Ingeniería%20de%20sistemas-orange)]()

**Integrantes:**
- Ana Isabel Patiño Osorio - CC. 1036690333
- Cristian Daniel Muñoz Botero - CC. 1007460166

**Video de presentación del proyecto:**
https://drive.google.com/file/d/1MG15C2KdUxPIYo4VnHZDXK9yvDxDPuHm/view?usp=sharing

> [!TIP]
> Puedes acceder al video con cualquier cuenta de Google


> [!WARNING]  
> Antes de ejecutar la **primera celda del notebook 01** debe tener cargado en el entorno de trabajo su token de Kaggle, en el archivo 'kaggle.json'. Esto es debido a que el dataset con el que se trabaja está en dicha plataforma. Recuerde cambiar la ruta de su token si es necesario.

> [!TIP]
> Los notebook 01 al final exportan los datos preprocesados a un archivo llamado 'data_class.csv'. Recuerda descargarlos y subirlos al entorno de los notebooks 02, 03, 04, 05, 06, 07 y 09 antes de ejecutarlos. Para ejecutar el notebook 08 recuerda cargar el archivo 'data_sfs.csv' el cual es exportado en el notebook 07. 

### Estructura general del proyecto
La carpeta Clasificación contiene 9 notebooks de colab. 
1. **Exploración y preprocesado de los datos**: En este notebook se realiza una exploración, se muestran algunas gráficas que permiten observar las distribuciones de las variables, la matriz de correlación y se escalan los datos numéricos. También para los datos categóricos se realiza una codificación OneHot.
2. **Notebooks donde se entrenan los modelos**: En Notebooks desde el 02 hasta el 06 se entrenan los modelos de Regresión logística, KNN, Random Forest, MLP y SVM.
3. **Notebook de selección de características**: En el notebook 07 se realiza la selección de características con un SFS.
4. **Notebook de prueba de SFS**: En el notebook 08 se realiza nuevamente el entrenamiento de los 2 modelos que presentaron mejor desempeño, con los datos generados en el notebook 7 (data_sfs.csv). A partir de estos entrenamientos se calculan las métricas para comparar.
5. **Notebook de extracción de características**: En el notebook 09 se realiza PCA a los datos que salen del notebook 01 y se realiza una nueva prueba con los datos resultantes de los datos obtenidos aplicando PCA.   
