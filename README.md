# RegresionLinealSimple
El objetivo de esta actividad es efectuar un análisis de regresión que permita construir un modelo predictivo a una base de datos real de manera que genere pronósticos adecuados.

1. Considere los valores históricos del Producto Interno Bruto (GDP) para México de acuerdo a los registros del banco mundial.
La base de datos previa se encuentra contenida en el archivo de Excel “Mexico GDP.xlsx”

2. Mediante una regresión de mínimos cuadrados ajuste los datos del archivo anterior al modelo logístico siguiente:
<img width="297" height="116" alt="image" src="https://github.com/user-attachments/assets/3f21421d-9936-473d-9ff7-8a4a3b458f8b" />
donde X representa el período (año) y Y el PIB. De lo anterior es evidente que debe estimar dos parámetros (Beta1 y Beta2 ). ¿Tuvo algún problema en el proceso de estimación de parámetros? ¿A qué crees que se debe? 

3. Transforme la base de datos previa dividiendo cada observación entre el valor máximo de la columna a la que pertenece. A este proceso se le denomina “Normalización”.

4. Vuelva a intentar el ajuste del problema anterior para las dos nuevas columnas resultantes.
¿Obtuvo resultados satisfactorios en esta ocasión?
Explique a detalle comentando sobre la bonda de ajuste.
¿Cuál sería su pronóstico del PIB (GDP) para México en el 2022?
¿Qué mecanismo de transformación tendría que realizar en dicho caso?  
