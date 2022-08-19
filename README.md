# Trabajo Final Diplomatura en Ciencia de Datos con Python
# Instacart-Market-Basket-Analysis

Caso de estudio basado en el problema de Kaggle.

![Market Basket Analysis](./imagenes/supermercado-750x430.jpg)

# Descripción
En este proyecto intentaremos resolver el problema de Instacart Market Basket Analysis

# Dataset empleado
Descargar los archivos necesarios desde:

https://www.kaggle.com/c/instacart-market-basket-analysis/data


# Descripcion de archivos

- Proyecto-JCV-1.ANALISIS_EXPLORATORIO_V1.0.ipynb
    Archivo que contiene el Analisis Exploratorio.

- Proyecto-JCV-2.INGENIERIA_DE_CARACTERISTICAS_v1.0.ipynb
    Archivo que realiza la generación del dataframe que se usara, agregando nuevas características a los datos iniciales.
    Por ejemplo:
           - uxp_times_bought: cuantas veces un usuario compro el mismo producto.
           - uxp_reordered_ratio: relación de reorden del usuario para cada producto.
           - u_num_of_orders: Número total de pedidos realizados por cada usuario.
           - u_avg_prd: promedio de productos comprados por cada usuario.
           - dow_most_orders_u:dow de la mayoría de los pedidos realizados por cada usuario 
           - hod_most_orders_u: hora del día en que cada usuario realiza la mayoría de los pedidos
           - prd_count_p: número de veces que se compró un producto
           - p_reordered_ratio: relación de reorden de productos.

- Proyecto-JCV-3.MODELO_DE_ENTRENAMIENTO_v2.0.ipynb
    Con el dataframe creado se testearan diversos algoritmos para seleccionar el que brinde mejores resultados:
    
    Los algoritmos empleados son:
        1. Logistic Regression
        2. SVM_rbf
        3. SVM_sigmoid
        4. Gaussian Naive Bayes
        5. SVM_linear
        6. Decision Tree
        7. Random Forest
        8. K - Nearest Neighbors.

    Una vez seleccionado el algoritmo, se procede a buscar los mejores parametros para su ejecución con el set de datos de entrenamiento y prueba.

- Proyecto-JCV-4.FINAL_v2.0.ipynb
    Este archivo posee el código que permite predecir que articulos se podran repedir o reordenar.
    Al final del código se genera el archivo para el envio a Kaggle, para la obtención del score o puntaje.


