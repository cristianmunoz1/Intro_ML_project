# Proyecto del curso Introducción al Machine Learning UdeA
[![Machine Learning](https://img.shields.io/badge/Asignatura-Modelos%20y%20simulación%20de%20sistemas%20II-red)](https://jdariasl.github.io/Intro_ML_2025/intro.html)
[![Semestre](https://img.shields.io/badge/Semestre-2025%201-blue)]()
[![Universidad](https://img.shields.io/badge/Universidad-UdeA-green)]()
[![Carrera](https://img.shields.io/badge/Carrera-Ingeniería%20de%20sistemas-orange)]()


> [!WARNING]  
> Antes de ejecutar la **primera celda del notebook** debe tener cargado en el entorno de trabajo su token de Kaggle, en el archivo 'kaggle.json'. Esto es debido a que el dataset con el que se trabaja está en dicha plataforma. Recuerde cambiar la ruta de su token si es necesario.  

### Ejecución del notebook
Para que el notebook funcione correctamente debe ejecutar en orden las celdas. Ya que al momento de realizar la normalización de los datos y las codificaciones de las variables categóricas el dataframe cambia y representará los datos de manera diferente. 

En el notebook se pueden observar 2 secciones principales:
1. **Sección de Exploración del dataset:** Aquí se verifican cuales son las variables del dataset, cual es su tipo, cual es su distribución, cual es la correlación entre ellas, se hace un conteo de las variables booleanas y se analizan mapas de calor entre las variables booleanas y la variable de salida que representa la probabilidad de una mascota de ser adoptada. 
2. **Sección de preprocesado:** En esta sección se cambia el dataset quitando la columna de PetID la cual no es necesaria para el posterior entrenamiento de los modelos ya que no aporta información, se normalizan las variables numéricas para trabajarlas en un rango de 0 a 1, se codifican con la técnica 'One hot' las columnas categóricas nominales y con un Ordinal Encoder de Scikitlearn las columnas categóricas ordinales. 
