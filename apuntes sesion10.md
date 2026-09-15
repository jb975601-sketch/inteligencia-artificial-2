Apuntes mejorados: Predicción con Machine Learning
1. Regresión lineal (fundamentos)
Para aprender, primero hay que definir matemáticamente qué significa equivocarse.
La solución matemática directa calcula los parámetros óptimos que minimizan el error (por ejemplo, el error cuadrático medio).
Un modelo lineal simple puede predecir la satisfacción de vida según el PIB. Al cambiar los parámetros, la línea de predicción también cambia.
2. Método del gradiente (Gradient Descent)
Se calculan las derivadas parciales de la función de costo.
El descenso consiste en dar un paso en la dirección en la que el costo disminuye.
Analogía: La única forma de bajar al valle es mirar hacia el norte e ir bajando “a ciegas”. Con las matemáticas, el proceso se vuelve seguro y controlado.
Existen tres variantes principales, que se diferencian por el tamaño del lote (batch size) y la velocidad:

Batch Gradient Descent: usa todo el conjunto de datos.
Mini-batch Gradient Descent: usa lotes pequeños. Optimiza la velocidad y aprovecha mejor la GPU.
Stochastic Gradient Descent (SGD): usa un solo ejemplo cada vez. “Rebota” mucho, lo que ayuda a escapar de mínimos locales.

Las rutas de los tres algoritmos en el espacio de parámetros son diferentes. El mini-batch avanza de forma más elegante y estable, y es el estándar de oro actual.
3. Regresión polinomial
Es un modelo lineal adaptado a datos más complejos mediante características elevadas (potencias) o combinaciones de las características existentes.
4. Curvas de aprendizaje
Son una herramienta diagnóstica muy útil:

Mesetas altas y muy juntas → diagnostican claramente subajuste (underfitting). El modelo es demasiado simple.
Gran brecha entre la curva de entrenamiento y la de validación → evidencia un sobreajuste grave (overfitting).

5. Regularización y parada temprana
Son técnicas para poner límites al modelo:

Regularización: fuerza a que los parámetros sean lo más pequeños posibles (L1, L2, etc.).
Parada temprana (Early Stopping): detiene el entrenamiento en el punto óptimo de error de validación (antes de que empiece a sobreajustar).

Ambas son tácticas muy usadas a nivel empresarial.

La parada temprana, en particular, es un “hermoso almuerzo gratis”: ahorra tiempo de cómputo y evita el sobreajuste sin necesidad de técnicas más complejas.
6. Modelos de clasificación
¿Cómo adaptar la optimización a clases discretas?
Se usan:

Regresión logística (clasificación binaria)
Softmax (clasificación multiclase)

Ambos permiten que un modelo lineal (o no lineal) produzca probabilidades y se entrene con funciones de costo adecuadas para clasificación.
