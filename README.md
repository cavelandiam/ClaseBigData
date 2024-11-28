# ClaseBigData
Ejercicios realizados para la clase de Big Data

#Clase 4

En la capa 1 y 2 se cambian los filtros a 16 y la función de activación a ReLU
Se agregan 2 capas adicionales model.add(tf.layers.dropout(0.6)); y model.add(tf.layers.batchNormalization());
Se agregó una capa densa de 256 neuronas model.add(tf.layers.dense({ units: 256, activation: 'relu' }));
Se valida por consola los logs de los valores y se evidencia que se queda en un accurancy del 90% console.log(logs.acc);
En la compilación se agregó una validación de datos con la función ADAM optimizer: tf.train.adam(0.0001)
Se cambian los valores de entrenamiento a 62000 y pruebas a 3000
Se identifica que siempre desde la segunda época, se queda congelado el accurancy en el mismo valor 0.899999976158142, se hizo la prueba con 10 épocas

0: 0.8186666369438171 
1: 0.8999999761581421 
2: 0.8999999761581421 
3: 0.8999999761581421 
4: 0.8999999761581421 
5: 0.8999999761581421 
6: 0.8999999761581421 
7:0.8999999761581421 
8: 0.8999999761581421 
9: 0.8999999761581421
