Entrenamiento de redes profundas

Problema de los gradientes inestables
Las señales de error se desvanecen (vanishing) o explotan (exploding) al propagarse hacia atrás por redes muy profundas, dificultando el ajuste de las primeras capas.

Saturación de la sigmoide
En sus extremos la función se aplana, la derivada tiende a 0 y el gradiente deja de transmitir información útil hacia atrás.

Inicialización de pesos (Glorot/Xavier, ~2010)
La investigación mostró que la señal que entra y sale de cada capa debe conservar aproximadamente la misma varianza ("energía"). Calibrar los pesos correctamente desde el inicio evita que el gradiente se desvanezca o explote desde el primer momento.

Problema de ReLU ("neuronas muertas")
ReLU no se satura en la parte positiva, pero si una neurona recibe siempre valores negativos, su salida y su gradiente quedan en 0 de forma permanente: la neurona "muere". Por eso surgieron variantes y activaciones modernas como GELU, Swish y Mish.

Normalización de datos
Se centran y estabilizan las entradas de cada capa (matemáticamente) para que el algoritmo de entrenamiento no colapse.

Control del gradiente
Se necesita un mecanismo de control absoluto sobre su magnitud para evitar que explote (gradient clipping).

Aprendizaje transferido
Se reutilizan capas de redes ya entrenadas: se congela la base y se ajustan solo las capas superiores para la tarea específica. Esta técnica impulsó el renacimiento de las redes profundas.

Preentrenamiento y regularización
El aprendizaje no supervisado permite que la red deduzca patrones por sí sola; técnicas como apagar neuronas durante el entrenamiento (dropout) evitan que dependa demasiado de neuronas puntuales, favoreciendo modelos más precisos.
