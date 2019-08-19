# Tarea-4

Después de probar distintas combinaciones de cantidad de capas y cantidad de neuronas por capa, la elección fue:

3 capas intermedias

512 neuronas, 128 y 8 respectivamente

Funciones de activación: Relu para la 1era y 3era capa intermedia, tanh para la 2da

Optimizador: adagrad

Usar dropout en todas las intermedia


Otro cambio importante fue el la segmentación del set de training y test. En la versión original tenía una proporción 87.5 - 12.5, con lo que los resultados del test siempre eran bajos (no llegaban al 70%). Cambiando la proporción a 70-30 y con un random state de 9 se logró el mayor score en test, sin tener underfitting ni overfitting

Corriendo el entrenamiento se hizo con 5000 epochs y 225 batch size

El mejor resultado obtenido fue: 75.35% en training y 75% en test

La estrategia fue modificar valores hasta obtener el mejor resultado antes de pasar a otro parámetro, por ejemplo:

Cantidad de capas, quitar, poner capas, cambiar la cantidad de neuronas, con o sin dropout
Llegué a tener 5 capas, pero el resultado empeoraba
Funciones de activación distintas por capas
Distintos optmizadores
Epochs y batch size, llegué a tener hasta 100.000 epochs, sin cambios importantes. Entre 2.000 y 10.000 se mantenía cierta variación
El caso extremo de los resultados obtenidos fue un 83% en training pero con un 52% en test

El éxito del resultado obtenido que considero aceptable, fue el cambio en la proporción del set de training vrs test

Adjunto documento de excel donde documentaba algunas de las pruebas que hacía. Está ordenado de mejor a peor resultado

