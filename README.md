# MasterMachine1

## Práctica 1:  estimación del precio de coches usados
Estimar el precio de venta de un coche de segunda mano en base a sus características. Disponer de un algoritmo predictivo capaz de resolver esta tarea puede tener multitud de aplicaciones: sugerir precios en portales de compra-venta online, tasación automática, etc.
Para resolver este problema se ha recopilado un conjunto de datos con ventas históricas de coches usados, incluyendo el precio real al que se vendió.
En este primer problema se pide implementar y entrenar un algoritmo de aprendizaje supervisado que sea capaz de predecir la variable precio. Se considerará que el modelo es satisfactorio si se obtiene un R2 superior a 0.9 en el conjunto de validación.
Adicionalmente, y con el fin de entender mejor y profundizar en los datos disponibles, se pide resolver las siguientes cuestiones:
1. Representar gráficamente la distribución de la variable precio en el conjunto de entrenamiento
2. ¿Cuál es la marca más cara en promedio? ¿Y la más barata?
3. Representar gráficamente la dependencia entre el precio y el kilometraje
4. Calcular las variables más significativas, ya sea mediante un test estadístico o
analizando el modelo entrenado
5. Un amigo quiere vender un audi A7 de 2020 con 5000 km, cambio automático,
combustible híbrido, consumo de 5.5 l/100km y motor 4.0. La tasa de circulación es de 200€. ¿A cuánto debería venderlo?

## Práctica 2: predicción del resultado de una campaña de marketing telefónica

Un banco realiza una campaña de marketing telefónica para ofrecer un depósito a plazo fijo a sus clientes. La campaña se ha llevado a cabo durante 3 años y se han recopilado los datos de la misma. Ahora que se acerca el cuarto año, el banco quiere mejorar los resultados de la campaña y nos pide que desarrollemos una solución para predecir si un cliente contratará su producto o no. De esta forma, se pueden gestionar mejor las llamadas al centrarse en los usuarios con mayor propensión.
El banco ha aglutinado la información en un dataset que contiene variables sobre el cliente, su situación financiera, los datos de la campaña o indicadores macroeconómicos.
Para el segundo problema se pide implementar y entrenar un algoritmo de aprendizaje supervisado que sea capaz de predecir la variable target. El banco considerará que el modelo es satisfactorio si se obtiene una tasa de acierto (accuracy) superior a 0.9 en el conjunto de validación.
Adicionalmente, y para poder entender mejor los datos disponibles, se pide resolver las siguientes cuestiones:
1. Calcular el ratio de conversión (porcentaje de clientes que contratan) de la campaña en el conjunto de entrenamiento
2. ¿Cómo influye el día de la semana de contacto en el resultado de la campaña? ¿Y el mes?
3. Transformar, al menos, las variables estado y resultado_anterior utilizando one-hot encoding
4. Representar gráficamente la curva ROC del modelo y calcular su AUC en el conjunto de validación5. El banco quiere optimizar los costes de la campaña utilizando el modelo que acabas de entrenar. Para ello, te indica que cada llamada que se realiza tiene un coste de 1€ para ellos, y que el beneficio obtenido al contratar el producto es de 100€. Por tanto, el balance neto (beneficios - gastos) de una campaña es:
Balance = 100€ x Clientes que contratan - 1€ x Clientes contactados
Para maximizar el balance se necesita que el mayor número posible de llamadas terminen en contratación. Es decir, que la precisión sea lo más alta posible. Por ejemplo: si se llama a 10 clientes y ninguno contrata el balance es -10€, y si contratan 5 el balance sería 490€.
El banco va a utilizar tu modelo para decidir a qué clientes llama y a cuáles no: llamará sólo a aquellos que tengan una probabilidad de contratación superior a un cierto umbral. Utilizando el conjunto de validación, deberás hallar cuál es el umbral que maximiza el balance de la campaña teniendo en cuenta los beneficios y los gastos.
Nota: El conjunto de validación contiene 8,536 clientes contactados, pero ahora lo que vas a hacer es simular qué hubiera pasado si se utilizase tu modelo. Es decir, para resolver esta pregunta debes calcular tanto el número de clientes contactados, en función de las probabilidades de tu modelo, como los que contratan.
