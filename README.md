# RegresionLinealSimple
El objetivo de esta actividad es efectuar un análisis de regresión que permita construir un modelo predictivo a una base de datos real de manera que genere pronósticos adecuados.

1. Considere los valores históricos del Producto Interno Bruto (GDP) para México de acuerdo a los registros del banco mundial.
La base de datos previa se encuentra contenida en el archivo de Excel “Mexico GDP.xlsx”
Hacemos un gráfico de dispersión para ver la forma de la curva. 
<img width="561" height="442" alt="image" src="https://github.com/user-attachments/assets/5f31ffe9-0c77-4ec5-9358-d85802af573d" />

3. Mediante una regresión de mínimos cuadrados ajuste los datos del archivo anterior al modelo logístico siguiente:
<img width="297" height="116" alt="image" src="https://github.com/user-attachments/assets/3f21421d-9936-473d-9ff7-8a4a3b458f8b" />
donde X representa el período (año) y Y el PIB. De lo anterior es evidente que debe estimar dos parámetros (Beta1 y Beta2 ). ¿Tuvo algún problema en el proceso de estimación de parámetros? ¿A qué crees que se debe? 

4. Transforme la base de datos previa dividiendo cada observación entre el valor máximo de la columna a la que pertenece. A este proceso se le denomina “Normalización”.
Tuvimos problemas al tratar de estimar los parámetros por tanteo ya que se requiere de una normalización previa. Esto debido a que los valores del PIB pueden ser muy grandes comparados con los valores del año y eso distorsiona el cálculo exponencial del modelo logístico.
Normalizamos los datos, después ajustamos el modelo con curve fit y graficamos el modelo ajustado
<img width="563" height="428" alt="image" src="https://github.com/user-attachments/assets/a5ceef10-e3c9-42fb-aaf8-3d05b8a1f469" />

6. Vuelva a intentar el ajuste del problema anterior para las dos nuevas columnas resultantes.

Finalmente realizamos el pronóstico del PIB (GDP) para México en el 2022 y calculamos R2 para determinar la bondad de ajuste. 
En esta ocasión se obtuvieron resultados satisfactorios ya que el modelo se adapta correctamente a los datos, esto se puede apreciar en la forma de la curva y también en la R2 calculada, la cual es de 97.8% Es decir que nuestro modelo tiene bastante precisión, ya que esta métrica indica la diferencia promedio esperada entre los valores predichos por un modelo y los valores reales. El pronóstico del PIB (GDP) para México en el 2022 obtenido fue de 1,255,426,603,076.2312  El mecanismo de transformación que realizamos para dicho aso fue primero normalizar 2022: x_2022_norm = 2022 / x.max() Después usar logistic_model(x_2022_norm, b1, b2) para predecir el valor normalizado. Y finalmente multiplicamos el resultado por y.max() para desnormalizar. 
