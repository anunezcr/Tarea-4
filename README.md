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
