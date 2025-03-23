# Regresion lineal simple
Análisis de regresión que permita construir un modelo predictivo considerando los valores historicos del producto interno bruto (GDP) para México

Cargamos las librerias a utilizar (matplotlib.pyplot, pandas, numpy, pylab y os para cargar los datos a utilizar)
<br>![image](https://github.com/user-attachments/assets/f60b5bff-9f0f-49ab-90bb-ff80976a4191)

Realizamos una visualizacion rapida de la informacion
<br>![image](https://github.com/user-attachments/assets/b1b55b42-4a77-4ea5-bcd1-cb3191545114) ![image](https://github.com/user-attachments/assets/8f680457-a53d-46d9-a8bb-d3d58f63b395)
<br>![image](https://github.com/user-attachments/assets/7cca5d86-20b2-48b3-8450-f62701efee3c)

Utilizando los valores del periodo así como las cantidades reales registradas del GDP obtenemos resultados que no pueden ser estimados y que sabemos que no son ciertos al ver la gráfica, esto puede ser debido a la gran magnitud y diferencia que existen entre los valores en ambas columnas. Esto puede ser solucionado normalizando los datos para poder procesarlos de manera más efectiva.
![image](https://github.com/user-attachments/assets/6d938ca3-c66d-4aee-b063-2c9c44d9fce3)
![image](https://github.com/user-attachments/assets/6acc1b54-676a-4562-893b-9c55a92f8312)

Al normalizar estos valores podemos continuar con el procesamiento
<br>![image](https://github.com/user-attachments/assets/d15389bd-88a9-49b1-b644-85b46583074c)

Ahora vemos que obtenemos valores diferentes que podemos probar y evaluar sus errores
<br>![image](https://github.com/user-attachments/assets/a176bbf5-89d9-4a1b-8504-f01e9d312943)

Con estos nuevos resultados, la gráfica y sin advertencias podemos decir que con un bajo MSE y un alto R2 es un buen ajuste Anteriormente con el rango de los periodos siendo números grandes y cercanos entre sí y los datos del GDP teniendo una diferencia y magnitud tan grandes ocasionaron problemas en la interpretación y procesamiento, pero al normalizar o escalar estos valores obtenemos información digerible lo que nos permite ajustarlo al modelo y hacer predicciones.

<br>![image](https://github.com/user-attachments/assets/130d11a7-e56d-4464-b9e3-73131cddce00)

Visualmente vemos que la predicción se ajusta bien a los datos de entrenamiento. 

Ahora podemos utilizar este modelo para realizar una predicción de un nuevo valor como el GDP para el año 2022
<br>![image](https://github.com/user-attachments/assets/b884473e-b6ac-4310-bea8-197d86e65280)

Donde primero tenemos que convertir el dato que queremos introducir a la escala utilizada para procesar los datos y al obtener el resultado debemos devolverlo a la escala real.
Podemos ver que la prediccion para el año 2022 seria de **1,262,948,764,094.6892**
